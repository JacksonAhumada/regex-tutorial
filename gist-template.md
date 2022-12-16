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

A Quantifier is a parameter that specifies how many instance of an element must be used in the email to have a successful match. The operator that is used to join the email name, email service and the `.com` is the `+` operator. The `{2,6}` quantifier is used to allow a match range of 2-6 characters when using the character set `[a-z\.]`.

### OR Operator

### Character Classes

The character class that is used in this expression is `\d` shown above. This matches a single character that is a digit from 0-9. Only single digits will match, for example "4" will match but "44" will not.

### Flags

This regex doesn't use Flags! Flags are normally used after the second `/` of our expression but we don't use them here.

### Grouping and Capturing

Group #1 in the expression above is `([a-z0-9_\.-]+)` which matches the name of the users email. The second group is `([\da-z\.-]+)`. This group matches the email service. The final group is `([a-z\.]{2,6})`, this group captures the `.com`.

### Bracket Expressions

This is the character set for bracket expressions, `[a-z0-9_\.-]`. Bracket expressions match any letter a-z and is case sensitive, it also matches a character 0-9 and the "_", "-", and ".". `[\da-z\.-]` matches a single digit from 0-9, a character from a-z, which is case sensitive, and the characters "." and "-". The final bracket expression is `[a-z\.]`, this matches any character a-z, also case sensitive, and the character ".".

### Greedy and Lazy Match

This regex that we are looking at does utilize something called greedy matches. Since the `+` quantifier is included, it will match as many times as possible giving back as needed. An additional quantifier is `{}`, this is used when matching `{2,6}` for the last capture group. 

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
