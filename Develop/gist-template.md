# Title (replace with your title)

For this tutorial, I will be walking you through the regular (or Regex) for matching a Hex Value. The Regex expression for matching a hex value is /^#?([a-f0-9]{6}|[a-f0-9]{3})$/ 

The table of contents below breaks down the tutorial into sections. You can also read the tutorial from top to bottom. 


## Summary

A Regular Expression (also known as Regex) is a sequence of characters used as a template to direct searches. Often, Regex expressions are used in searches looking for search patterns and input validation.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
<!-- - [Flags](#flags) -->
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
<!-- - [Boundaries](#boundaries) -->
<!-- - [Back-references](#back-references) -->
<!-- - [Look-ahead and Look-behind](#look-ahead-and-look-behind) -->

## Regex Components

### Anchors
In a Regex expression, Anchors provide you information about the expression but are not involved in the symbols that make up the process. 

In our Regex expression /^#?([a-f0-9]{6}|[a-f0-9]{3})$/ there are two anchors. The symbols ^ and $ are both anchors. Both of these anchors have two different meanings. 

The ^ anchor marks the beginning of the string.
The $ anchor marks the end of the string.

Both of these anchors continue to have the same meaning in other regex expressions.

### Quantifiers

Two quantiriers are within the regex expression /^#?([a-f0-9]{6}|[a-f0-9]{3})$/

The quantifier ? means that the character that comes before is equal to 0 or 1 and is optional in a search. The character that comes before the ? is the #. This means that during the search, a # may or may not be present.

The quantifier {} is located within the regex expression twice. Once as {6} and once as {3}. This expresses the number of characters that are needed. For example, we will look at what comes before the {6} in the first half of the regex. This is [a-f0-9]. The {6} dictates that there must be 6 of [a-f0-9] characters. So, aaaaaa would be appropriate as well as 000000 would also be appropriate. 

The {3} quantifier works in the same way but with three characters. So, aaa would be appropriate for the {3} quantifier.

### OR Operator

There is one OR operator within the regex expression /^#?([a-f0-9]{6}|[a-f0-9]{3})$/

The | is the or operator. Its name is self-explanatory as the or operator is saying the expression can be one way OR another way within the confines of the quantifiers. So, in our regex expression, we are searching for a hex code of either three characters OR 6 characters. 

As you can see, the | marks the middle of the regex expression separating the [a-f0-9]{6} and [a-f0-9]{3}

### Character Classes

In the regex expression /^#?([a-f0-9]{6}|[a-f0-9]{3})$/ we have a set of the same character classes. The character classes are [a-f0-9] 

Character classes are located within the [ ]. Character classes are characters we want to match in a search. Character classes can stand alone or be hyphened. In our regex expression, the hyphen means "through." So, our regex expression can use the characters a through f and 0 through 9. This means we are using all the numbers and letters in between 0 and 9 and a through f. 

<!-- ### Flags -->

### Grouping and Capturing

In the regex /^#?([a-f0-9]{6}|[a-f0-9]{3})$/ the grouping is done by the () 
This grouping encapselates character classes and treats them as a single unit.

In other words, the () dictate that [a-f0-9] as a string that is contained. 

### Bracket Expressions

In the regex /^#?([a-f0-9]{6}|[a-f0-9]{3})$/ the grouping is done by the () 
This grouping encapselates character classes and treats them as a single unit.

In other words, the () dictate that [a-f0-9] is a string that is contained. 

### Greedy and Lazy Match

In our regex expression /^#?([a-f0-9]{6}|[a-f0-9]{3})$/ we will look at the quantifier {}. This quantifier is greedy. Meaning, we are matching the longest possible string. 

A lazy match is marked by a ? as in the example expression b.+?l. Here the expression would match the shortest possible string. So, 
the match would be bel. Whereas a greedy match would appear as b.+l and would match bell.

In our regex expression /^#?([a-f0-9]{6}|[a-f0-9]{3})$/ we are matching greedy as there is not an appended ? within the quantifier {}

<!-- ### Boundaries -->

<!-- ### Back-references -->

<!-- ### Look-ahead and Look-behind -->

## Author

My name is Christina Brenia, and I am exploring Javascript, Node.js, Database, CSS, HTML, and other web development languages and techniques. 

My Github profile can be found here: https://github.com/ChristinaBrenia?tab=repositories