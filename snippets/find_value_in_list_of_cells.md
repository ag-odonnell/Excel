# if looking for a value in the values of a list of cells.
* =IF(COUNTIF(B:B, A2), "Found", "Not Found")
* Count Found
  * =IF(COUNTIF(B:B, A2), 1, 0)
* Count NOT Found
  * =IF(COUNTIF(B:B, A2), 0, 1)
# ✅ Scenario: You want to know if each value in Column A exists in Column B
Let’s say:
* List 1 is in A2:A10
* List 2 is in B2:B100
## 🟡 Option 1: Use COUNTIF (Simplest and Most Common)
In cell C2, enter:
* =IF(COUNTIF(B:B, A2), "Found", "Not Found")
Copy this down. It will return "Found" if the value in A2 is anywhere in column B.
## 🟡 Option 2: Use ISNUMBER + MATCH (Also Good)
* =IF(ISNUMBER(MATCH(A2, B:B, 0)), "Found", "Not Found")
MATCH returns the row number if found, or #N/A if not. ISNUMBER checks that.
## 🟡 Option 3: Highlight Matches with Conditional Formatting
* Select the range A2:A10.
* Go to Home > Conditional Formatting > New Rule > Use a formula to determine...
* Enter:
  * =COUNTIF(B:B, A2)>0
* Set a format (like fill color) and click OK.

# Can also: extract matches, filter, or do a two-way match (like return common values only).
