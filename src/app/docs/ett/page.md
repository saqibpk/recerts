---
title: Granular Certificates (GC) 
nextjs:
  metadata:
    title: Granular Certificates (GC) 
    description: Comprehensive guide on Granular Certificates (GC), their structure, real-time tracking, and benefits.
---

Granular Certificates (GCs) represent the next generation of Energy Attribute Certificates (EACs), enabling **real-time energy tracking** and improved transparency in renewable energy markets. Unlike traditional EACs, which cover monthly or yearly periods, GCs provide **hourly or even sub-hourly** data for energy generation and consumption.

---

## Introduction to Granular Certificates (GC)

Granular Certificates (GCs) ensure more precise accounting of renewable energy use by providing timestamped data for each unit of electricity generated. This enables businesses to match their consumption with clean energy on an **hour-by-hour basis**, improving their ability to meet 24/7 sustainability goals.

### Key Features of GCs

- **Hourly Energy Tracking** – Ensures real-time verification of energy production and usage.
- **Enhanced Transparency** – Provides more granular data than traditional EACs.
- **Improved Market Efficiency** – Supports 24/7 carbon-free energy initiatives.
- **Blockchain Integration** – Many GCs are stored on decentralized networks for security and traceability.

---

## Structure of a Granular Certificate (GC)

A GC includes detailed metadata about energy generation at specific time intervals. Below is an example of a GC in JSON format:

```json
{
  "certificateId": "GC-20250307-001",
  "issuer": {
    "name": "Granular Energy Authority",
    "country": "Denmark",
    "issuanceDate": "2025-03-07"
  },
  "generator": {
    "id": "GEN-789123",
    "name": "Scandinavian Solar Park",
    "location": {
      "country": "Denmark",
      "region": "Aarhus",
      "latitude": 56.1629,
      "longitude": 10.2039
    },
    "type": "Solar",
    "capacity_kW": 3000
  },
  "granularEnergyData": [
    {
      "timestamp": "2025-03-07T00:00:00Z",
      "energyGenerated_kWh": 50,
      "emissionFactor_kgCO2e": 0
    },
    {
      "timestamp": "2025-03-07T01:00:00Z",
      "energyGenerated_kWh": 45,
      "emissionFactor_kgCO2e": 0
    }
  ],
  "owner": {
    "id": "BUY-789456",
    "name": "GreenTech Solutions",
    "country": "Denmark"
  },
  "validity": {
    "issueDate": "2025-03-07",
    "expiryDate": "2026-03-07"
  },
  "status": "Active",
  "blockchain": {
    "transactionId": "0x123abc789def456",
    "network": "Ethereum",
    "contractAddress": "0x789def123abc456ghi"
  }
}
```

---

## Benefits of GCs

### Advancements Over Traditional EACs

- **Time-Specific Matching** – Ensures hourly or sub-hourly alignment of energy production and consumption.
- **Enables 24/7 Carbon-Free Goals** – Organizations can match clean energy use with real-time data.
- **Market Flexibility** – Supports **dynamic pricing** and **new trading mechanisms** for renewable energy.

### Environmental and Business Impact

- **Stronger Commitment to Sustainability** – Helps companies prove their use of clean energy around the clock.
- **Increases Renewable Energy Adoption** – Encourages real-time energy production and usage synchronization.
- **Enhances Energy Market Transparency** – Reduces reliance on estimated or averaged data, making energy markets more efficient.

---

## Conclusion

Granular Certificates (GCs) are a significant improvement over traditional EACs, offering **real-time tracking**, **enhanced transparency**, and **stronger compliance with 24/7 renewable energy initiatives**. By leveraging blockchain technology and timestamped energy data, GCs pave the way for a **more accurate, transparent, and accountable energy future**.
