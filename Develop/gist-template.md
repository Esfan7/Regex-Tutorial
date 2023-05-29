# Learn Regex fast
In this tutorial you will be taught the basics of regex and how it can be implemented in your code. The easiest way to under regex is to know it is used for descrbing patterns. You will see it used to validate specific strings or text in a document.

## Summary

You often see regex used in search engines, word processors, and text editors below we have multiple examples on how you would use regex components to do certain task.

This is a regex for a name
''''
/^[a-zA-z]{2,}$/
''''

"^" means must start with 
[a-zA-Z] and contains a character from a - z and A-Z
{2,} means atleast 2 characters


## Table of Contents

- [Learn Regex fast](#learn-regex-fast)
  - [Summary](#summary)
  - [Table of Contents](#table-of-contents)
  - [Regex Components](#regex-components)
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
  - [Author](#author)

## Regex Components


### Anchors
^ $ //start, end

### Quantifiers
a* //0 or more //optional
a+ //1 or more //i need atleast 1
a? //0 or 1 //optional but not more than 1a
a{5} //atleast 5
a{2,} //atleast 2 to infinity
 
### OR Operator
ab|cd	match ab or cd

### Character Classes
- //match between two letters
. //match if there is a line break

### Flags

/i ignore uppercase 
/g resets the search
. will match everything include a new line


### Grouping and Capturing
(abc) // captures group
(?:abc)	//non-capturing group

### Bracket Expressions
[abc] //match atleast one letter in the bracket

### Greedy and Lazy Match
+ //greedy match wants more
? //optional match  

### Boundaries
\bword\b //must match the entire word exactly
\Bword\B //must not have the word "word"

### Back-references

/(?<quote>['"])(.*?)\k<quote>/g;

Back reference will remember a a regex sequence and you can call it again with <word>

### Look-ahead and Look-behind
(?=abc) // positive lookahead looks for next closes group of (abc) will return true if it conains abc
(?!abc) //negative lookahead this will return true if it doesn't have abc

## Author

[Esfandiar Behbehani is a business major studying at FSU while also studying full-stack development at UCI. At my github you can find many of my other projects and examples.](https://github.com/Esfan7)
