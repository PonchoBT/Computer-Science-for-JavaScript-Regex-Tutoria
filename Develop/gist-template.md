## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Boundaries](#boundaries)
- [Back-references](#back-references)
- [Look-ahead and Look-behind](#look-ahead-and-look-behind)

## Regex Components

```bash
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
```

### Anchors

'^' at the beginning and '$' at the end of the regular expression denote the start and end of the text, respectively. This means that the string must start and end exactly with the defined pattern.

### Quantifiers

'{2,6}' after '[a-z\.]' indicates that this group must have a character length between 2 and 6, inclusive. This restricts the number of characters the email address domain can be.

### OR Operator

An OR operator ('|') is not used explicitly in this regular expression. Instead, character classes ('[...]') are used to define valid character ranges.

### Character Classes

'[a-z0-9_\.-]': This group defines the valid characters for the username in the email address. Includes lowercase letters, digits 0 through 9, and the characters '_', '-', and '.'.

'[\da-z\.-]': This group defines the valid characters for the domain name in the email address. Includes digits ('\d'), lowercase letters, and the characters '-' and '.'.

### Flags

Flags are not used in this regular expression.

### Grouping and Capturing

Parentheses '()' are used to define groups of characters. In this case, there are three defined groups:
The first group captures the username.
The second group captures the domain name.
The third group captures the extent of the domain.

### Bracket Expressions

Square brackets '[]' are used to define character classes. They are used in various parts of the regular expression to define the allowed character ranges.

### Greedy and Lazy Match

This regular expression uses greedy matching, meaning it will try to find as many matches as possible.

### Boundaries

No specific limits are used in this regular expression.

### Back-references

No back-references are used in this regular expression.

### Look-ahead and Look-behind

No look-ahead or look-behind searches are used in this regular expression.