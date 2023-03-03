# How Do You Read Regular Expressions? (Regex)

What are regular expressions? Simply put, They are literals that can be used to verify if strings meet a certain criteria. If the strings compared to them match the criteria, they will return true. This is very useful for verifiying that you are taking in the correct data, such as emails, passwords, urls, etc. 

## Summary

```
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
```

The regex statement above that I will be going over is going to match an email. If this statement is checked against an email, it will return true. 

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

Regex is made up of components contained within square brackets ( [ ] ). These components all check parts of the string to verify that they meet the criteria within the square brackets. 

### Anchors

Regex has two "anchors", "$" and "^". 

^ is used to verify the string BEGINS with the matching criteria.

^ is used to verify the string ENDS with the matching criteria.

### Quantifiers

Quantifiers allow you to set two limits on the amount of characters in your string. 

### OR Operator

The OR operator ( | ) allows you to check if the string meets one critieria, OR it meets another. If the string meets EITHER of the criteria, it will return true.

### Character Classes

Character classes are predefined sets of characters that regex recognizes to shorten the length of your expressions. An example of this could be something like, "\d" would match any Arabic numeral digit.

### Flags

Flags are placed at the end of your regex expression. They allow for us to define certain rules and limits for our expression checking, such as the flag "m" which checks for multi-line inputs versus single line inputs. 

### Grouping and Capturing

To group a pair of regex expressions, you can use parenthesis, "()". This will allow your expression to only return true if both expressions are true. 

### Bracket Expressions

Bracket expressions are anything inside of square brackets ([]), they are also referred to as "positive character groups". This is because inside our brackets, we include the inputs we want the regex to match. 

### Greedy and Lazy Match

Greedy Match refers to things like quantifiers, that will match as many instances in the regex statement as they can.

Lazy Match refers to the opposite, matching as FEW instances as possible. 

### Boundaries

Boundaries are often confused with anchors. Something like, "\b" is a boundary. Both define a way for our regex expression to be interpreted. Boundaries are used in examples to find things like words. 

### Back-references

Regex back-references are used to match the same expressions that were previously matched in the statement. One common example of this usage would be for matching HTML tags.

### Look-ahead and Look-behind

Look ahead and Look behind statements, otherwise known as "lookaround" are very simple matches. They will only return a match or no match.

## Author

Maximilian Holzmann, Minnesota Bootcamp Student. [Github](https://github.com/MaxHolzmann)
