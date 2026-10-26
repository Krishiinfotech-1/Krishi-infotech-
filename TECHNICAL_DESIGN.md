# Technical Design Document — Krishi FairCheck

## 1. Purpose

Explore a farmer-friendly workflow combining crop moisture information, preliminary quality screening and verified market-price information before sale.

## 2. Current architecture

```text
Farmer / operator
      |
      v
Browser interface (HTML + CSS + JavaScript)
      |
      +--> Crop and market selection
      +--> Manually entered moisture reading
      +--> User-selected visual observation
      |
      v
Preliminary demo report
```

This is the architecture of the current demonstration only. There is no backend, sensor connection, AI model or live market data integration.

## 3. Proposed future architecture

```text
Crop sample
   |
   +--> Calibrated moisture sensor
   |
   +--> Crop-specific image/quality assessment
              |
              v
       Validation / review layer
              |
              v
   Farmer-facing screen / mobile interface
              |
              +--> Verified market-price service
              |
              v
 Report with crop, market, timestamp, units,
 moisture reading, preliminary quality and caveats
```

## 4. Data and safety requirements

- Keep crop, grade, market, date/time and unit explicit.
- Show the source and timestamp of every price.
- Avoid comparing prices across incompatible grades or units.
- Clearly distinguish measured readings from user-entered values.
- Treat quality output as preliminary until validated.
- Avoid storing personal data unless necessary and consented to.

## 5. Validation plan

1. Select one crop and define applicable quality parameters with an agricultural expert.
2. Compare sensor readings with a trusted calibrated reference.
3. Evaluate quality-assessment performance on labelled samples.
4. Verify market-price freshness and consistency against the source.
5. Run usability tests with farmers and record feedback.

## 6. Current limitations

The existing code is a static browser demo. The physical device and future integrations are proposals, not completed features.
