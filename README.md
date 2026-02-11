# ethiopia-food-prices-analysis
Spreadsheet analysis of Ethiopian food prices with currency conversion and error resolution.
# Ethiopia Food Prices Spreadsheet Analysis

This project demonstrates:

- Circular dependency errors in spreadsheets
- Cross-tab referencing issues
- Fixing missing tab names in formulas
- Using absolute cell references
- Currency conversion using exchange tables

## Formula Used
=K2/Conversion!$B$199

This formula converts Birr price to USD using a fixed exchange rate stored in the Conversion tab.

## Key Concepts Demonstrated

- Circular dependency errors
- Incorrect sheet references
- Absolute vs relative references
- Currency conversion in Excel
# Spreadsheet Error Explanation

## Circular Dependency Error

A circular dependency error occurs when formulas depend on each other directly or indirectly.

## Incorrect Tab Reference

The error occurred because:

- The formula referenced cells in another tab.
- The tab name was not included.
- Some references pointed to non-existing cells.

To fix this:

1. Add the tab name before the cell reference:
Conversion!B199
2. Use absolute reference:
Conversion!$B$199

This locks the exchange rate cell so all rows use the same value.

After correcting this:
- USD Price column errors were resolved
- Total quantity price errors were resolved
