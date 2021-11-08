# REGEX_EXPLAINED

This REGEX (REGULAR EXPRESSION) explanation is being created to help users understand the sequence of special charaters used to verify a search term. REGEXs are patterns used to match character combinations in strings. When used in code, REGEX can find certain patterns of characters or replace a character or sequence within a string. They are also used to validate input data.

## Summary

I will be explaining the REGEX used to match Hex Values. Hex Values are used to determine color using the hexidecimal color code format. Hex Value REGEX have 2 types, Hex Triplet Format (#000000 or #FFFFFF) and Shorthand Hex Format (#000 or #FFF).

Example:    
/^#?([a-f0-9]{6}|[a-f0-9]{3})$/

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

### Anchors
`/^`#?([a-f0-9]{6}|[a-f0-9]{3})`$/`

The highlighted portion of the above example indicate what we call anchors. Anchors are used at the start and end of an expression NOT to match characters. `^` matches the position before the first charcater. `$` matches the position after the last character.

### Quantifiers
/^#`?`([a-f0-9]`{6}`|[a-f0-9]`{3}`)$/

The highlighted text of the above example indicate what we call quantifiers. Quantifers are used to indicate how many characters are to be expected for a match to be found. In our example, the `?` idicates the expression to match 0 or 1 time. As mention in the summary above, we have 2 formats of Hex Values. In our Hex Value REGEX we have `{6}` and `{3}` this indicates that the length of the component preceding these quantifiers should be 6 and 3.

Hex Triplet Format (#000000 or #FFFFFF)
<br />
Shorthand Hex Format (#000 or #FFF)

### OR Operator
/^#?([a-f0-9]{6}`|`[a-f0-9]{3})$/

The "or" operator in the above REGEX is defined using the `|` symbol. The or operator indicates that it could be either of the components that we are seperating witht the `|`. 

An easier way to read the above REGEX would be: <br />
 /^#?([a-f0-9]{6}`or`[a-f0-9]{3})$/ 

### Character Classes
/^#?([a-f0-9]{6}|[a-f0-9]{3})$/

Character Classes are a part of our REGEX to signify the type of characters to expect. In the above example, the character classes are set within brackets `[]`. Our example included 2 character classes, `[a-f0-9]` and `[a-f0-9]` which search for the same value. The values being `a-f` (searching for letter a-f) and `0-9` (searching for number 0-9).

### Flags

### Grouping and Capturing

### Bracket Expressions

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
