
# Excel Formulas Cheat Sheet

| Category | Formula | Description |
|----------|---------|-------------|
| **Math & Trigonometry** | `=SUM(A1:A10)` | Adds values in the range |
| | `=AVERAGE(A1:A10)` | Returns average of values |
| | `=ROUND(A1,2)` | Rounds a number to 2 decimal places |
| | `=ROUNDUP(A1,0)` | Rounds a number up |
| | `=ROUNDDOWN(A1,0)` | Rounds a number down |
| | `=POWER(A1,2)` | Returns square of a number |
| | `=SQRT(A1)` | Returns square root |
| | `=ABS(A1)` | Returns absolute value |
| | `=MOD(A1,3)` | Returns remainder |
| | `=PI()` | Returns value of PI |
| | `=RAND()` | Returns random number (0-1) |
| | `=RANDBETWEEN(1,100)` | Returns random number between given range |

| Category | Formula | Description |
|----------|---------|-------------|
| **Statistical** | `=MAX(A1:A10)` | Returns maximum value |
| | `=MIN(A1:A10)` | Returns minimum value |
| | `=MEDIAN(A1:A10)` | Returns median value |
| | `=MODE(A1:A10)` | Returns most frequently occurring number |
| | `=STDEV(A1:A10)` | Returns standard deviation |
| | `=VAR(A1:A10)` | Returns variance |

| Category | Formula | Description |
|----------|---------|-------------|
| **Text** | `=LEN(A1)` | Returns number of characters |
| | `=TRIM(A1)` | Removes extra spaces |
| | `=UPPER(A1)` | Converts text to uppercase |
| | `=LOWER(A1)` | Converts text to lowercase |
| | `=PROPER(A1)` | Converts text to proper case |
| | `=CONCATENATE(A1," ",B1)` | Joins values together |
| | `=TEXT(A1,"MM/DD/YYYY")` | Formats a number/date as text |
| | `=LEFT(A1,5)` | Returns first 5 characters |
| | `=RIGHT(A1,5)` | Returns last 5 characters |
| | `=MID(A1,2,3)` | Extracts substring |
| | `=SEARCH("x",A1)` | Finds position of character |
| | `=REPLACE(A1,1,3,"New")` | Replaces part of text |
| | `=SUBSTITUTE(A1,"old","new")` | Substitutes occurrences of text |

| Category | Formula | Description |
|----------|---------|-------------|
| **Logical** | `=IF(A1>10,"Yes","No")` | Returns conditional result |
| | `=IFERROR(A1/B1,"Error")` | Returns custom error message |
| | `=AND(A1>5,B1<10)` | Returns TRUE if both conditions are met |
| | `=OR(A1>5,B1<10)` | Returns TRUE if any condition is met |
| | `=NOT(A1>10)` | Reverses logical value |

| Category | Formula | Description |
|----------|---------|-------------|
| **Lookup & Reference** | `=VLOOKUP(101,A1:D100,2,FALSE)` | Vertical lookup |
| | `=HLOOKUP(101,A1:D100,2,FALSE)` | Horizontal lookup |
| | `=XLOOKUP(101,A1:A100,B1:B100,"Not Found")` | Modern replacement for VLOOKUP |
| | `=INDEX(A1:C10,2,3)` | Returns value at row/column |
| | `=MATCH(50,A1:A10,0)` | Returns relative position of value |
| | `=OFFSET(A1,2,3)` | Returns reference with offset |
| | `=INDIRECT("A1")` | Returns reference from text |

| Category | Formula | Description |
|----------|---------|-------------|
| **Date & Time** | `=TODAY()` | Returns current date |
| | `=NOW()` | Returns current date & time |
| | `=DAY(A1)` | Returns day from date |
| | `=MONTH(A1)` | Returns month from date |
| | `=YEAR(A1)` | Returns year from date |
| | `=WEEKDAY(A1)` | Returns weekday number |
| | `=EDATE(A1,1)` | Returns date after given months |
| | `=DATEDIF(A1,B1,"D")` | Returns difference in days |
| | `=NETWORKDAYS(A1,B1)` | Returns working days between two dates |
| | `=TIME(12,30,0)` | Returns specific time |
| | `=HOUR(A1)` | Returns hour from time |
| | `=MINUTE(A1)` | Returns minutes from time |
| | `=SECOND(A1)` | Returns seconds from time |

| Category | Formula | Description |
|----------|---------|-------------|
| **Financial** | `=PMT(5%/12,60,30000)` | Loan payment |
| | `=FV(5%/12,60,-500)` | Future value of investment |
| | `=NPV(10%,A1:A10)` | Net present value |
| | `=IRR(A1:A10)` | Internal rate of return |

| Category | Formula | Description |
|----------|---------|-------------|
| **Information** | `=ISNUMBER(A1)` | Checks if value is number |
| | `=ISTEXT(A1)` | Checks if value is text |
| | `=ISBLANK(A1)` | Checks if cell is empty |
| | `=ISERROR(A1)` | Checks if value is error |
