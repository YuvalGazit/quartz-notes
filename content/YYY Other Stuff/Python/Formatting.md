---
{}
---
# String Formatting

|   |   |
|---|---|
|**Symbol**|**Description**|
|b|Format an integer in binary.|
|c|Given a number, display the character that has that code.|
|d|Display a number in decimal (base 10).|
|e|Display a float value using the exponential format.|
|E|Same as e, but use a capital “E” in the exponent.|
|f|Format a number in fixed-point form.|
|g|General numeric format: use either f or g, whichever is appropriate.|
|G|Same as “g”, but uses a capital “E” in the exponential form.|
|n|For formatting numbers, this format uses the current local setting to insert separator characters.|
|o|Display an integer in octal format.|
|s|Used for string format.|
|x|Display an integer in hexadecimal (base 16). Digits greater than 9 are displayed as lowercase characters.|
|X|Display an integer in hexadecimal (base 16). Digits greater than 9 are displayed as uppercase characters.|
|%|Display a number as a percentage: its value is multiplied by 100, followed by a “%” character.|

# String Formatting Example Table

|   |   |   |   |
|---|---|---|---|
|**Number**|**Format**|**Output**|**Description**|
|3.1415926|{:.2f}|3.14|2 decimal places|
|3.1415926|{:+.2f}|+3.14|2 decimal places with sign|
|-1|{:+.2f}|-1.00|2 decimal places with sign|
|2.71828|{:.0f}|3|No decimal places|
|5|{:0>2d}|05|Pad number with zeros (left padding, width 2)|
|5|{:x<4d}|5xxx|Pad number with x's (right padding, width 4)|
|10|{:x<4d}|10xx|Pad number with x's (right padding, width 4)|
|1000000|{:,}|1,000,000|Number format with comma separator|
|0.25|{:.2%}|25.00%|Format percentage|
|1E+09|{:.2e}|1.00e+09|Exponent notation|
|13|{:10d}|13|Right aligned (default, width 10)|
|13|{:<10d}|13|Left aligned (width 10)|
|13|{:^10d}|13|Center aligned (width 10)|
