# cheatsheet

## RegEX

https://regex101.com/

## ^[\d{16,16} -]+$ to find all numbers that have 16 digits, and may include a hyphen (-).

The string uses the ^ symbol to look for the beginning of the line.
[ is the opening of the character set to look for these values.

\d is used to match the digits.

{16} is a quantifier (it matches the exact digits 16 times).

The space between } and – tells the expression to look for a space.

'-' tells the expression to look for a hyphen.

] is the closing of the character set.

'+' matches one or more of the preceding values.

The string then looks for the end of the line using the $ symbol.


## ^[AMHF].*$ to find all names, countries, and states beginning with A, M, H, and F.

The string uses the ^ symbol to look for the beginning of the line.

[AMHF] matches the single character (uppercase).

.*$ completes the string until the end of the line.

## ^\(\d+\).*$ to find all phone numbers.

The string uses the ^ symbol to look for the beginning of the line.

\( the backslash escapes the character; the curved bracket (open parenthesis) matches that symbol.

\d matches a single digit.

+\) continues matching digits until the curved bracket (closing parenthesis) symbol is found.

.*$ completes the string until the end of the line.

## ^3[47]\d{13}$ to find all American Express credit cards

American Express card numbers start with 34 or 37 and have a total of 15 digits.

The string uses the ^ symbol to look for the beginning of the line.

3 is the number 3 at the beginning.

[47] matches either the number 4 or 7.

\d{13} matches 13 digits.

$ is the end of line.

## to find all Visa credit cards

^4[0-9]{12}(\d{3})?$

The string uses the ^ symbol to look for the beginning of the line.

4 is the number 4 at the beginning.

[0-9]{12} matches 12 numbers, from 0 to 9 (like \d).

(\d{3})? groups another 3 digits, and the question mark indicates that this group does not necessarily need to be present.

$ is the end of line.

## to find all emails in the document

^[\w._-]+@[\w._-]+\.[\w]{2,}$


The string uses the ^ symbol to look for the beginning of the line.

[\w._-]+@ matches any character, digit, dot, underline, or hyphen (the plus sign continues the search until interrupted by the @ sign).

[\w._-]+\. matches every character, digit, dot, underline, or hyphen until it reaches a dot.

[\w]{2,} after the dot matches any alphanumeric character with two or more characters.




