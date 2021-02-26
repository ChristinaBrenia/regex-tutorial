# Title (replace with your title)

Introductory paragraph (replace this with your text)

## Summary

Briefly summarize the regex you will be describing and what you will explain. Include a code snippet of the regex. Replace this text with your summary.

For this tutorial, I will be walking you through the regular (or Regex) for matching a Hex Value. The Regex expression for matching a hex value is /^#?([a-f0-9]{6}|[a-f0-9]{3})$/

The table of contents below breaks down the 

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
In a Regex expression, Anchors provide you information about the expression but are not involved in the symbols that make up the process. 

In our Regex expression /^#?([a-f0-9]{6}|[a-f0-9]{3})$/ there are two anchors. The symbols ^ and $ are both anchors. Both of these anchors have two different meanings. 

The ^ anchor marks the begining of the string
The $ anchor marks the end of the string

Both of these anchors continue to have the same meaning in other regex expressions.

### Quantifiers

Two quantiriers are within the regex expression /^#?([a-f0-9]{6}|[a-f0-9]{3})$/

The quantifier ? is greedy. Greedy means that the character that comes before is equal to 0 or 1, and is optional in a search. The character that comes before the ? is the #. This means that during the search, a # may or may not be present.

The quantifier {} is located within the regex expression twice. Once as {6} and once as {3}. This expresses the amount of characters that is nneded. For example, we will look at what comes before the {6} in the first half of the regex. This is [a-f0-9]. The {6} dictates that there must be 6 of [a-f0-9] characters. So, aaaaaa would be appropiate as well as 000000 would also be appropiate. 

The {3} quantifier works in the same way but with three characters. So, aaa would be appropiate for the {3} quantifier. 

### OR Operator

### Character Classes

### Flags

### Grouping and Capturing

### Bracket Expressions

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
