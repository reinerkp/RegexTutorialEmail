# Regular Expression (Matching an Email)

In this article we will describe the many components of the Regular Expression that is used for mathching an email 

## Summary

Regular expressions are a criteria of characters that speficies a pattern that you are looking to match. They are not language specific, rather used in every language to search imputed value to make sure that the patterns align. These patterns can help find sequences such as emails, phone numbers, usernames, password, etc to help a developer gather the information that is needed.
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
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
### Anchors
The symbols "^" and "$" are both to be considered anchors. The "^" is considered to be the starting anchor. The starting anchor begins the search for the following character.
The $ anchor closes out the string with the preceding characters that are within.
### Quantifiers
The qualifiers sets the standard for the characters that must match within the brackets. With the email example, in the first bracket we see [a-z0-9_\.-] Within the brachets are the qualifiers. So we can see that in order to meet the limits of this regex it must could include any letter, number, or special character.
### OR Operator
The OR operator is used when you want the string to meet all the given requirements that are in the pattern. For example if you want (123) to be used either all together or one indivually the OR operator can help with that by using a "|", so the expression would become (1|2|3). This is not used in the email example.
### Character Classes
When working with regex, there are defined characters that will always equate for a specific match. For example, in the email regex we see this pattern in the begginning [a-z0-9_\.-]. It starts with allowing any number 0-9 to be entered. A character class instead could enter a "/d" to match any numberical value 0-9.
### Flags
Flags are used to divine additional limits and fuctionality to the structure of the regex. In the email regex no flags are used, although common flags can include global search, case insensitive, or multi-line search.
### Grouping and Capturing
An email has three different main parts to the stucture. The ID or Username (scottsmith), the domain (gmail), and lastly the network (.com). Although a regex is one large expression. It contains subexpression that might each have their own criteria. The subsections and grouping are greated by seperating each group by a parentheses within the main parantheses, such as (()). Within the email expression we can see three different groupings /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/.
### Bracket Expressions
Bracket Expressions are used to define a range of characters that we want to match with. In the email example, the expression [a-z\.] can be seen that we are specifically looking for something that includes any letter between a-z and it can also incluse a period. The main takeaway here, is that we are given that specifc range with the expression that is provided in the brackets.



## Author
Katherine Reiner 

[View my Github!](https://github.com/reinerkp)