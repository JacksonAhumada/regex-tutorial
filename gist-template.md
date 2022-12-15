# Title (replace with your title)

In this tutorial I want to explain how to use regex to match users emails us the expression `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`. This is used when the validation of users emails for applications or different technologies is needed.

## Summary

A regular expression, or regex for short, is a sequence of characters that specifies a search pattern in text. When using regex for email validation, it makes it possible to check to see if an email address is correctly spelled, has no commas, or spaces, and that all the @s, domain extensions and dots are in the correct place. This tutorial is going to walk through what regex consists of and how it is used to match an email.

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

### Anchor

There are two anchors that are currently used, the `^` character and the `$` character. The `^` character is the first anchor used and it means that a match must occur at the beginning of your string. It means that be beginning of our verified email must abide by the parameters that are set in the brackets `[]`. For example the beginning of our email must match `[a-z0-9_\.-]+)`.

Our second anchor that is used is the `$`. This is servers the same purpose as our `^` character but its used for the end of the email. This is stating that the end of our email must match the parameter that are set in the brackets of our last Character Group `[a-z\.]{2,6})$/`.


### Quantifiers



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
