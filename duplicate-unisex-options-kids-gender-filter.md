# FLT-GND-001 - Duplicate "Unisex" Options Displayed Under "Gender" Filter in Kids Section

* **Severity:** Low
* **Environment:** Production · macOS Sonoma 14.4 · MacBook Air (Apple M1) · Safari 17.4
* **Reproducibility:** 100%

## Summary
When navigating to the "Kids" section, the "Gender" filter displays two separate, redundant unisex options instead of a single unified filter in both Georgian and English.

## Steps
1. Switch the website language to either Georgian or English.
2. Click on the "Kids" / "ბავშვები" category from the top navigation menu.
3. Go to the left sidebar and expand the "Gender" / "სქესი" filter.
4. Observe the list of available gender filter options.

## Actual
Under the "Gender" / "სქესი" filter in the Kids section, two separate unisex options are listed (e.g., "უნისექსი" and "უნისექსი (ბავშვი)" in Georgian, or "Unisex" and "Unisex (Kids)" in English).

## Expected
Regardless of the selected language, there should be a single unified "Unisex" option under the "Gender" filter for the Kids section grouping all unisex children's products without duplicate entries.

## Notes
Functional Correctness / Filter & Data Logic. Redundant or split filter attribute values in the Kids catalog across both locales.
