# FLT-GEN-002 - Men's Jacket Displayed Under "Plus Size" Filter in Women's Jackets Category

* **Severity:** Medium
* **Environment:** Production · macOS Sonoma 14.4 · MacBook Air (Apple M1) · Safari 17.4
* **Reproducibility:** 100%

## Summary
When filtering by "Plus Size" inside the "Women's jackets" category, a men's jacket appears among the returned product results.

## Steps
1. Navigate to the "Women's jackets" category.
2. Select the "Plus Size" filter option.
3. Review the filtered product results.

## Actual
A men's jacket is displayed in the product results under the "Women's jackets" category with the "Plus Size" filter applied.

## Expected
Only women's jackets matching the "Plus Size" filter should be displayed, with no men's items appearing in the results.

## Notes
Functional Correctness / Filter & Data Logic. Likely incorrect gender or category/attribute assignment on the product item in the catalog.
