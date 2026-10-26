# Manual Test Cases

These tests apply to the current browser demonstration. They do not validate physical sensors, AI quality grading or live prices.

| ID | Test | Expected result |
|---|---|---|
| TC-01 | Open `index.html` in a modern browser | Interface loads without installation |
| TC-02 | Select each listed crop | Selected crop is reflected in the report |
| TC-03 | Enter a valid moisture value from 0 to 100 | Report shows the entered value |
| TC-04 | Leave moisture blank | Interface requests a valid reading |
| TC-05 | Enter a negative moisture value | Interface rejects the input |
| TC-06 | Enter moisture above 100 | Interface rejects the input |
| TC-07 | Select different visual observations | Report reflects the selected observation |
| TC-08 | Inspect price section | Clearly states that no verified live price is connected |
