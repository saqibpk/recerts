---
title: ReCert -  Re-Certification for Granular Certificates
nextjs:
  metadata:
    title: ReCert -  Re-Certification for Granular Certificates
    description: ReCert framework is based on the ReCertification of Granular Certificates
---

Granular Certificates (GCs) represent the next generation of Energy Attribute Certificates (EACs), enabling **real-time energy tracking** and improved transparency in renewable energy markets. Unlike traditional EACs, which cover monthly or yearly periods, GCs provide **hourly or even sub-hourly** data for energy generation and consumption.

```json
{
  "certificateId": "GC-20250307-002",
  "issuer": {
    "name": "Granular Energy Authority",
    "country": "Denmark",
    "issuanceDate": "2025-03-07"
  },
  "generator": {
    "id": "GEN-123456",
    "name": "Nordic Wind Farm",
    "location": {
      "country": "Denmark",
      "region": "Jutland"
    },
    "type": "Wind",
    "capacity_kW": 5000
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
    "id": "BUY-789123",
    "name": "GreenTech Solutions",
    "country": "Denmark"
  },
  "validity": {
    "issueDate": "2025-03-07",
    "expiryDate": "2026-03-07"
  },
  "status": "Active"
}
```

Energy Attribute Certificates (EACs) are an older mechanism for tracking renewable energy consumption. However, they **lack time granularity**, meaning they only provide monthly or yearly tracking instead of real-time hourly data. This makes it difficult for businesses and energy buyers to **match their actual consumption with clean energy production** on an hourly basis. Additionally, EACs are prone to **double counting risks** if not properly managed, and they do not support emerging market needs for **real-time energy matching** and **24/7 carbon-free energy** goals.

```json
{
  "certificateId": "EAC-20250307-003",
  "issuer": {
    "name": "Green Energy Authority",
    "country": "Denmark",
    "issuanceDate": "2025-03-07"
  },
  "generator": {
    "id": "GEN-654321",
    "name": "Scandinavian Solar Park",
    "location": {
      "country": "Denmark",
      "region": "Aarhus"
    },
    "type": "Solar",
    "capacity_kW": 3000
  },
  "energyDetails": {
    "productionStart": "2025-03-01T00:00:00Z",
    "productionEnd": "2025-03-07T23:59:59Z",
    "energyGenerated_MWh": 1000,
    "emissionFactor_kgCO2e": 0
  },
  "owner": {
    "id": "BUY-456789",
    "name": "EcoPower Solutions",
    "country": "Denmark"
  },
  "validity": {
    "issueDate": "2025-03-07",
    "expiryDate": "2026-03-07"
  },
  "status": "Active"
}
```

Granular Certificates (GCs) provide a **superior alternative** by ensuring that renewable energy tracking is done in **real-time**, offering better compliance, market flexibility, and transparency in the transition towards a more **sustainable and accountable energy system**.
