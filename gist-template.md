# Regex-Project

## Summary
The top line is a regex or regular expression.
```
$ ^[0-9 a-z A-Z -_]{4,20}$
$ Pa_$$w-0rdsAr3Gr3At1
```
The password above is a mix of characters, symbols, and numbers. The length of the string is 4-20 characters.
It is an example of a password that the regex would be able to approve.

Read below for short written tutorials on regex.

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
---

### Quantifiers
A quantifier, `{num, num}`, is an indicator that the proceeding token needs to match a certain number of times.

A regex example is provided below:
```
^[a-z]{3,20}$
```
---

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

---

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
---

### Flags
Regex can have flags that can affect the way a search is interpreted. There are also 6 different expressions that can be used.

`i` - ignore case / will make the whole expression case-INsensitive.

`/aBc/i would still match AbC`

`m` - multiline / 

`u` - unicode / 

`g` - global search / will match all occurences which means it will be tested against all possible matches in a string.

`/expression/g`

`s` - dotall / will match any character, including newline, (`.`). However, in JavaScript, you will have to use a catch-all character class, `[\S\s]`. To find out more [click here.](https://riptutorial.com/regex/example/18156/dotall-modifier)

`(.*?)`

`y` - sticky / will only match from the lastIndex position and also ignores the global flag if it is set.

---

### Grouping and Capturing
Grouping creates a capture group when you put multiple characters together.

`(lol)` - 
It will only search for the grouped characters.

---

### Bracket Expressions
Brackets match characters inside the brackets. It could be a range of characters as well.

`[aeiou]` -
This will find all vowels.

`[a-z]` -
This will find letters a through z.

---

### Greedy and Lazy Match
The `greedy` quantifier uses an algorithm that tries to match the pattern at that position, and if there is no match it will go to the next position.

`".+"` - This will find all strings in quotations.

The `lazy` quantifier makes the preceding quantifier lazy which will cause it to match as few characters as possible to fufill the search.

`".+?"` - This will look for the first quote and then look for any character then look for another quote. If it doesn't find the quote it will search for another character and so on until it finds the last quote.

---

### Boundaries
`Boundaries` are used to find characters that are in a word and near a non-word character, such as a space, or a position at the start/end of a a string.

```
l\b
```
This will match the character `l` and then search for the character at the start and end of all strings.

---

### Back-references
`Back-references` will match the same text used previously matched by a capturing group.

```
^([A-Z][a-z0-9])\b\1$
```
Using the `\1` will call back to the first capturing group and match the same exact group.

---

### Look-ahead and Look-behind
A `look-ahead`, `(?=)` will search and match the preceding terms only if the look-ahead was matched first. Otherwise, it will skip it.

Example:
```
b(?=oot)
```

A `look-behind`, `(?<=)` will do the same as a look-ahead but it will look-behind. It will match a pattern if there's something before it.

Example:
```
(?<=Boo)t
```

---

## Author
I'm Paul Vera, a full stack developer, and I would like you to start using regex!

If you have questions, email me directly.


Email: paul88vera@gmail.com

GitHub: [github.com/paul88vera](https://www.github.com/paul88vera)
