# FLT-VOL-001 – Duplicate Values in the "Volume" Filter Due to Inconsistent Formatting

* **Severity:** Medium
* **Environment:** Production · macOS Sonoma 14.4 · MacBook Air (Apple M1) · Safari 17.4
* **Reproducibility:** 100% (Always)

## Summary
In the Personal Care category, the "Volume" filter displays duplicate options for the same volume due to inconsistent formatting (e.g., "150 ml", "150 მლ", "150მლ/ML"), and selecting one option returns only products matching that exact string rather than all matching products.

## Preconditions
The user is on the homepage.

## Steps
1. Navigate to the Personal Care category.
2. Open the "Volume" filter.
3. Review the listed options and select different variations of the same volume (e.g., "150 ml" vs. "150 მლ").

## Actual
Duplicate volume entries with inconsistent formatting appear in the "Volume" filter, and selecting a specific variation returns only products matching that exact text instead of all products with that volume.

## Expected
Each volume should appear once in a standardized format (e.g., "150 მლ") and display all matching products regardless of how the underlying volume text was entered.

## Notes
Functional Correctness / Filter & Data Consistency. Suggested fix: standardize existing volume values in the catalog/database and restrict the admin input field to a dropdown or predefined units instead of free text.
