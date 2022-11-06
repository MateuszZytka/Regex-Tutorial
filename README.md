# Regex-Tutorial



A regular expression, otherwise known as a Regex, is a sequence of characters that specify a search pattern in text. Regex tends to be used when searching for text or when validating inputs. Different coding languages have different syntaxes for writing regular expression. Common regex examples are used to validate emails, urls, or matching an HTML tag. 

## Summary

This tutorial is going to explain the use of regex to match emails using the expression `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`. This regex is useful when validating emails using applications such as Node or MongoDb. 

Briefly summarize the regex you will be describing and what you will explain. Include a code snippet of the regex. Replace this text with your summary.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)
- [Character Escapes](#character-escapes)

## Regex Components

### Anchors

The anchors used in this regex are the characters `^`, `$`, and `(m)`. They all serve a different purpose, the character `^` indicates the beginning of the string while the `$` indicates the end of the string. The `(m)` anchor specifies that multiline is not enabled.  

### Quantifiers

A quantifier is placed after an element, it specifies how many times the element is allowed to repeat. In this regular expression the `+` character is what connects the seperate strings, the email name, email service and the doamin extension. Another quantifier that is used is the `{2,6}`. This quantifier only allows a range of 2 to 6 characters. 

### Grouping Constructs



### Bracket Expressions

### Character Classes

### The OR Operator

### Flags

### Character Escapes

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
