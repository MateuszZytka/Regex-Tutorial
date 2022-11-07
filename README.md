# Regex-Tutorial

A regular expression, otherwise known as a Regex, is a sequence of characters that specify a search pattern in text. Regex tends to be used when searching for text or when validating inputs. Different coding languages have different syntaxes for writing regular expression. Common regex examples are used to validate emails, urls, or matching an HTML tag. 

## Summary

This tutorial is going to explain the use of regex to match emails using the expression `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`. This regex is useful when validating emails using applications such as Node or MongoDb. 

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

A Regex is composed of several components. A regex does not require all the available components to work. This regex `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/` has the following components: 

Anchors ^ $  
Captures and Groups ([a-z0-9_\.-]+)  
Quantifiers + {}  
Bracket Expressions [ ]  
Character Classes [\d]  

### Anchors

The anchors used in this regex are the characters `^`, `$`, and `(m)`. They all serve a different purpose, the character `^` indicates the beginning of the string while the `$` indicates the end of the string. The `(m)` anchor specifies that multiline is not enabled. 

In this regex we have the anchor `^` that signifies the start of the string, along with the anchor `$` that signifies the end of the string. 

### Quantifiers

A quantifier is placed after an element, it specifies how many times the element is allowed to repeat. In this regular expression the `+` character is what connects the seperate strings, the email name, email service and the doamin extension. Another quantifier that is used is the `{2,6}`. This quantifier only allows a range of 2 to 6 characters. 

### Grouping Constructs

Grouping constructs are the part of the regex that is enclosed in the parentheses (). In the validating an email regex we use three different groups that allow us to search for emails that inclues a username, email service and the domain extension. Using the quantifier `+` we are able to search for a string that contains all three of our grouping constructs. 

### Bracket Expressions

The characters within square brackets [] represent the character we want to match. These chartacters are known as the positive character group, also known as a pattern - bracket expressions. In the first part of this regex expression `[a-z0-9_\.-]` we are looking for any characters between a-z, 0-9 and include the special characters `.-`. The second part `[\da-z\.-]` is only searching for the special characters `.-` along with letters from a-z(case sensitive) and a single digit from 0-9. The last section `[a-z\.]` is only searching for character between a-z and the special character `.`.

### Character Classes

The only character class in this expression is `/d`. This matches a single character from 0-9, as such it will match the number "5" but not "55".


## Author

You can view my projects at https://github.com/MateuszZytka 
