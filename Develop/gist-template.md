# Regex Tutorial on Matching an Email

Regular expressions are used to search for specific, particular patterns of characters. They can also be used to replace character(s) if necessary. The Expression, or Regex, here checks for a valid email address. 

## Summary

The Regex considered here checks for an email address: /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)

## Regex Components

### Anchors
The anchors used to contain this regular expression are: ^ to start, and $ to finish.

### Quantifiers
In this example, we used + to communicate there is another sequence to be matched as a greedy quantifier. We used {2,6} as another quantifer to specify the input should be a minimum of 2 characters to a maximum of 6 characters.

### Character Classes
In this regular expression, the character class /d is used, which in Javascript classifies the use of any digit from 0 to 9.

### Grouping and Capturing
Three groups are captured here. Group 1 is the username portion [a-z0-9_\.-]. The second group captures e-mail service being used [\da-z\.-]. Finally, the third group captures the domain extension (.com, .org, etc.) [a-z\.]{2,6}

### Bracket Expressions
Much like the groups in this example, there are also 3 bracket expressions. The information in the bracket expressions is opened and closed between brackets like this []. This indentifies which information is allowed to be matched.

Bracket Expression #1: [a-z0-9_\.-] - includes case sensitive characters from a-z, numbers from 0-9 an underscore, periods and hyphens.

Bracket Expression #2: [\da-z\.-] - includes all digits, case sensitive characters from a-z, periods and hyphens

Bracket Expression #3: [a-z\.] - includes case sensitive characters from a-z and periods.

### Greedy and Lazy Match
In this example we have only used greedy quantifiers + and {}, meaning that it will allow the match to expand as long as it neess to go. If these quantifiers were lazy quantifiers, they would appear as +? or {}?, this will direct the system to make the shortest match.

## Author

My name is Evan Kuck. I am a full-stack web developer.