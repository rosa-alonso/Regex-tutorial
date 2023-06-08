# Using Regex to Match an Email

This Regex tutorial was written in order to explain how regular expression (otherwise known as regex), can be used to validate emails in technology.

## Summary

Briefly summarize the regex you will be describing and what you will explain. Include a code snippet of the regex. Replace this text with your summary.
The regex expression for matching an email is as follows:

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

Regex uses a set of characters to define search patterns. The way you use Control+F as a keyboard shortcut to find certain keywords on a document or web browser, regex does the same thing, using expressions in order to find patterns within a string. This tutorial in particular explains the components of regex for validating an email.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Author](#author)

## Regex Components

### Anchors

The first anchor in this regex expression is the ^. This comes at the beginning of the string. The second anchor is the $, indicating the end of the string.

### Quantifiers

Quantifiers are used in an expression to indicate the amount of times a specific character should appear. The email regex expression has two: + and {2,6}. the + symbol connects the email name, for example: user123, PLUS email service: @yahoo, PLUS .com. The second quantifier: {2,6}, found near the end of the regex expression, allows for a character range of 2-6, in a character set of a-z.

### Character Classes

Our character class in the regex is the \d. This will match characters that are a single digit 0-9. The backslash is important as it differentiates itself as a character class instead of just the character d.

### Grouping and Capturing

There are three groups found in this expression. The first one being: ([a-z0-9_\.-]+) . This expression is matching the email name. The second capturing group is ([\da-z\.-]+) . This matches the email service (yahoo, gmail, etc.). Our third group is as follows: ([a-z\.]{2,6}) , giving us our .com. As stated in the quantifiers section, the plus symbol connects each of the three groups.

### Bracket Expressions

Finally, bracket expressions are used to validate emails given certain character sets. For example, the first grouping of our regex is ([a-z0-9_\.-]+). The [a-z0-9_\.-] indicates that an email can be any character a-z, have digits 0-9, and any of those given special characters.

## Author

You can view Rosa Alonso's github profile here:
https://github.com/rosa-alonso
