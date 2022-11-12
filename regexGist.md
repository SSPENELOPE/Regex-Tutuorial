# Matching E-mail regex 

- This is a description on the process of using a email regex 

## Summary

- The regular expression `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/` is used to validate an email address. 
- The following content below will breakdown the above expression 

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
 Anchors are used to match a position within your regex string. 

 For example the anchors used in our email expression 

- "^" Indicates the start of the regex

- "$" Indicates the end of the regex

### Quantifiers
 Quantifiers indicate that the preceding token that must be matched a certain amount of times. Quatifiers will match as many possible characters as it can

 For example:

- "+" Will match 1 or more of the preceding token

- "{2,6}" Will match the quantity of the previous tokens

### Grouping Constructs
Grouping lets you combine tokens in specific order to allow them to operate together

Groups in the email regex are: 
- ([a-z0-9_\.-]+)
- ([\da-z\.-]+)
- ([a-z\.]{2,6})

Breakdown of the groups
- The first group Checks for lowercase letters, numbers, underscores, hyphens, and periods typed in before the "@" symbol in our email.
- The second group lods for any numbers, lowercase letters, periods or hyphens aftert the "@" but before the period in "email@gmail.com"
- The second group looks for 2 to 6 characters with lowercase letters after the period in our email

### Bracket Expressions
Brackets used in or regex just tell you where in the regex to search for the characters. Think of this as our divider for our start and end points

### Character Classes / Character Escapes
Character classed are what we tell the regex to look for 

For example: 
- a-z, will tell the regex to look for all letter from "a" to "z"
- 0-9, will look for all numbers
- \d, will match any character (0-9) that is equivalent to 0-9

Character Escapes are what we use to break the sequence in which the regex is searching

For example: 

- /., will break the sequence that the regex is looking for

### The OR Operator
Using the "OR" operator, which is depicted as "|" in a regex is used to seperate the regex to tell it that it should look for "this line of code" "or/|" "this line of code

### Flags
Flags in a regex are optional search parameters we can add. For example if we add "/g" to the end of our regex it will turn it into a global search


## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)