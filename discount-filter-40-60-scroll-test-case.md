# TC-FLTR-001 – Verify Discount Range Filter (40–60%) Accuracy During Scroll

* **Module / Scope:** Functional Testing – Product Filtering & Pagination
* **Priority:** Medium
* **Environment:** Web (Desktop / Safari)

## Preconditions
The user is on the sales/discount section of the e-commerce platform, where product cards display their respective discount percentages.

## Test Steps
1. Open the sales/discount section.
2. Select the **40–60%** discount filter option.
3. Scroll down through the displayed product list to load additional items.
4. Check the discount percentages displayed on all product cards during and after scrolling.

## Expected Result
Only products with a discount falling strictly within the **40%–60%** range should be displayed in the filtered results, including when additional items are loaded during scrolling.
