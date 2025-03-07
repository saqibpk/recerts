## Overview of Slicing in Granular Certificates (GCs)
The slicing mechanism enables the division of energy certificates into smaller, transferable units ("slices") while maintaining integrity and preventing double-counting. This concept, inspired by fractional stock trading, ensures granular tracking of energy production/consumption at sub-hourly intervals. Below is a technical breakdown:

---

### How Slicing Works
1. **Initial Issuance**  
   - A GC is created with an **immutable header** (metadata: grid area, time interval, meter ID, energy source).  
   - One initial slice is issued, representing the total energy (e.g., 400 Wh for production or 300 Wh for consumption).

2. **Splitting Slices**  
   - Slices can be split into smaller units (e.g., 400 Wh → 300 Wh + 100 Wh).  
   - Each slice contains:  
     - `quantity`: Energy amount.  
     - `owner`: Pseudonymous public key.  
   - **Invariant**: The sum of all slices must equal the original GC's total energy.

3. **Transfer & Claim Operations**  
   - **Transfer**: Ownership of a slice is updated by associating it with a new public key.  
   - **Claim**: A consumption slice (e.g., 100 Wh) is matched to a production slice (e.g., 100 Wh) to prove green energy usage.  
   - State changes are logged as immutable events on a blockchain via Merkle trees.

```plaintext
Example Workflow:
Production GC (400 Wh) → Split into [300 Wh, 100 Wh]  
Consumption GC (300 Wh) → Split into [200 Wh, 100 Wh]  
Claim: Match 100 Wh consumption slice to 100 Wh production slice.  
Result: Remaining 200 Wh consumption slice can be claimed against other sources.