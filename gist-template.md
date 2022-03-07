# Regex-Project

## Summary
The top line is a regex or regular expression.
```
$ ^[0-9 a-z A-Z -_]{4,20}$
$ Pa_$$w-0rdsAr3Gr3At1
```
The password above is a mix of characters, symbols, and numbers. The length of the string is 4-20 characters.
It is as example password that the regex would be able to approve.

---

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

---

## Regex Components

### Anchors
An regex anchor allows you to match a position before, (`^` - carat anchor matches the beginning of the text), or after, (`$` - dollar anchor matches the end of the text), a string of characters.

A regex example is provided below:
```
^[a-z]$
```

### Quantifiers
A quantifier, `{num, num}`, is an indicator that the proceeding token needs to match a certain number of times.

A regex example is provided below:
```
^[a-z]{3,20}$
```

### OR Operator
An `OR operator` or a `|` symbol is exactly what it sounds like, it's a logical "or" operator. This "or" that.

A regex example is provided below:
```
^I like (cats|dogs), but not (lions|wolves).$
```
This will match four different strings.

`I like cats, but not lions.`

`I like cats, but not wolves.`

`I like dogs, but not lions.`

`I like dogs, but not wolves.`

### Character Classes
A `character class` or `character set ` allows you to match a certain set of characters within a square bracket.

A regex single character class example is below:
```
^gr[ae]y$
```
This will accept, `gray` or `grey`.

Another way you can use this is to create a range of characters using a hyphen (`-`).
A regex range character class example is below:
```
^[a-z]$
```

### Flags


### Grouping and Capturing


### Bracket Expressions


### Greedy and Lazy Match


### Boundaries


### Back-references


### Look-ahead and Look-behind

---

## Author
I'm a full stack developer that would like your to start using regex! 

If you have questions, email me directly.


email: paul88vera@gmail.com

github: [paul88vera](https://www.github.com/paul88vera)
