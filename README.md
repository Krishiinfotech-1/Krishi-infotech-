# Krishi FairCheck

**Team:** Krishi Infotech  
**Theme:** Rural Development & Livelihoods  
**Concept:** A proposed physical device to measure crop moisture and provide a preliminary crop-quality assessment, connected to a mobile interface for verified market-price information.

## Current prototype status

This repository currently contains a browser-based workflow demonstration built with HTML, CSS and JavaScript. It is **not** connected to a physical moisture sensor, a validated AI grading model, or a live market-price API. The interface is intended to communicate the planned workflow, not to provide an official crop assay or a real market quote.

## Run locally

1. Download or clone this repository.
2. Open `index.html` in a modern browser.
3. Use the form to explore the demonstration workflow.

No package installation or environment variables are required for the current static prototype.

## Proposed workflow

1. Select crop and reference market.
2. Enter a moisture reading from a separate meter.
3. Record a visual observation.
4. Generate a preliminary report.
5. In a future version, retrieve dated market prices from a verified source.

## Planned technical architecture

- **User interface:** HTML, CSS, JavaScript
- **Future sensor layer:** calibrated crop-specific moisture sensor
- **Future quality assessment:** crop-specific model validated against recognised standards, with human review where necessary
- **Future market data:** verified source with market, date, unit and grade context
- **Future mobile integration:** responsive web interface, with Kannada-friendly language and accessibility

## Limitations and responsible use

- The current interface is a demonstration only.
- Manual moisture entry is not a sensor measurement performed by this software.
- No AI crop classifier is implemented in the current version.
- No live market-price feed is connected.
- Outputs must not be presented as official quality certification or proof of buyer misconduct.
- Any future sensor, grading model or price feed must be validated before real-world use.

## Project files

- `index.html` — browser-based demonstration
- `TECHNICAL_DESIGN.md` — architecture, workflow and limitations
- `sample_data.csv` — clearly labelled illustrative test inputs, not real market data
- `TEST_CASES.md` — manual test cases
- `LICENSE` — MIT License

## Future development

1. Choose one crop for an initial pilot.
2. Test a calibrated moisture sensor against a trusted reference.
3. Validate quality parameters with qualified agricultural/market experts.
4. Connect an authorised market-price source and show the timestamp, market and units.
5. Conduct usability testing with farmers, including Kannada-language support.
