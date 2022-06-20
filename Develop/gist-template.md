# Regex Breakdown
RegEx stands for Regular Expression. Regular Expression is a search pattern used by developers. This search string is a pattern in a series of characters. They can be used to find and replace strings in a given document, used in search engines, or for input validation.

## Summary
RegEx is a tool that can help in finding all the emails in the document. Instead of going combing through the document and looking for each email individually, we could create regex expression to find them all. In this tutorial, we will be looking at a regular expression that can be used to match or find emails and identify the different components of regex.

    /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

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
Anchors help identify positions of characters. The caret `^` defines the beginning of the string. The dollar sign `$` defines the end of the string.

`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

### Quantifiers
Quantifiers match. The plus `+` will match one or more of the preceding token. It will look for a match with `[a-z0-9_\.-]`. Two numbers with curly brackets `{2,6}` will match from two to six from the previous token. Finally, with `[a-z\.]` it will also look for a match.

### OR Operator
The pipe `|` symbol is an example of an OR operator. It matches the expression before or after it. However, there are none in this example.

### Character Classes
Character classes match a character from a specific set. 
In our example `[a-z0-9_\.-]` will match any character within the square brackets. It will go through: a-z or 0-9. This will match any letter or number contained within the set range and is also handled as case sensitive.
This is also will work with the `\d` in `[\da-z\.-]`, matching to any digit 0-9.

### Flags
Flags will always follow the closing forward slash of an expression, and change how it is interpreted. This tutorial does not have any flags but an example of one would be using  `i` to flag the search as case-insensitive.

### Grouping and Capturing
Grouping tokens are a way to work on multiple characters as a single capture group. You can create them by surrounding the characters you want to group up with (). This allows you to check the entire group for a match, and lets you even use quantifiers on them.
With this example, there are three groups `([a-z0-9_\.-]+) ([\da-z\.-]+) ([a-z\.]{2,6})`

### Bracket Expressions
Bracket Expressions are a special character class. It is enclosed by a bracket `[]` matching any single character within the brackets. 

### Greedy and Lazy Match
Quantifiers such as  `+ * ? and {}` are greedy operators, so they match as much as they can. While Lazy Match creates the shortest string.

### Boundaries
Boundaries are the places between characters, like a wall between any adjacent characters. There are two types of Boundaries, Word and Non-Word.
If using A boundary you would need to input `\b` symbol.

### Back-references
Back-referencing is the reference of a captured match, save in memory, by a captured group.

### Look-ahead and Look-behind
"Lookarounds" is a term combining look-ahead and look-behind. When you use "Lookarounds", it will match to a group of characters either before or after a pattern, but it will not be included as part of the result. Look-ahead is for groups after the pattern and look-behind is for groups that are before the pattern.

## Author

Thank you viewing this quick tutorial!
My name is Stephanie Ramos Rodriguez, I am currently a student in the UCR Extension Coding Bootcamp working towards becoming a software developer. Below is the link to my GITHUB with projects dating back to my first work in Tech!  

[![GitHub Profile](https://img.shields.io/badge/github_profile-000?style=for-the-badge&logo=ko-fi&logoColor=white)](https://github.com/stephrrcodes)