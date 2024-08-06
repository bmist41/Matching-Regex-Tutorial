# SSN Matching Regex

Brief description of your project and its purpose.

## Table of Contents
  - [Introduction to Regex](#introduction-to-regex)
  - [Basic Syntax](#basic-syntax)
 
  - [Anchors](#anchors)
  - [Quantifiers](#quantifiers)
  - [Groups and Ranges](#groups-and-ranges)
  - [Special Characters](#special-characters)
  - [Lookaheads and Lookbehinds](#lookaheads-and-lookbehinds)
  - [Common Use Cases](#common-use-cases)
  - [Character Classes](#character-classes)
  - [Conclusion](#conclusion)


### Introduction to SSN Regex

This pattern matches a Social Security number format, ensuring it starts at the beginning of a line (^), has three digits (\d{3}), a hyphen (-), two digits (\d{2}), another hyphen (-), and ends with four digits (\d{4}$).

### Anchors

Purpose of Anchors are used to specify the position in the text.

- ^: Matches the start of a string.
    -Example: ^hello matches "hello" at the start of a string.
- $: Matches the end of a string.
    -Example: world$ matches "world" at the end of a string.

### Quantifiers

Purpose of Quantifiers are to specify the number of occurrences of a character or group to match.

- *: Matches 0 or more occurrences.
    - Example: a* matches "", "a", "aa", etc.
- +: Matches 1 or more occurrences.
    Example: a+ matches "a", "aa", etc.
- ?: Matches 0 or 1 occurrence.
    - Example: a? matches "" or "a".
- {n}: Matches exactly n occurrences.
    - Example: a{3} matches "aaa".
- {n,}: Matches n or more occurrences.
    - Example: a{2,} matches "aa", "aaa", etc.
- {n,m}: Matches between n and m occurrences.
    - Example: a{2,4} matches "aa", "aaa", or "aaaa".

### Grouping Constructs

Grouping constructs allow you to group parts of a regex pattern.

- (abc): Matches the exact sequence "abc".
    - Example: (dog|cat) matches "dog" or "cat".

### Bracket Expressions

The purpose of Bracket expressions is to define a set of characters to match.

- [abc]: Matches any one of the characters a, b, or c.
    - Example: [aeiou] matches any vowel.
- [^abc]: Matches any character except a, b, or c.
    - Example: [^0-9] matches any non-digit character.
- [a-z]: Matches any lowercase letter.
    - Example: [a-z] matches "a" to "z".

### Character Classes

The purpose of Character classes is to match specific sets of characters.

- \d: Matches any digit.
    - Example: \d matches "0" to "9".
- \D: Matches any non-digit.
    - Example: \D matches any character except "0" to "9".
- \w: Matches any word character (alphanumeric plus underscore).
    - Example: \w matches "a" to "z", "A" to "Z", "0" to "9", and "_".
- \W: Matches any non-word character.
  -Example: \W matches any character except "a" to "z", "A" to "Z", "0" to "9", and "_".
- \s: Matches any whitespace character.
    - Example: \s matches spaces, tabs, and line breaks.
- \S: Matches any non-whitespace character.
    - Example: \S matches any character except spaces, tabs, and line breaks.

### OR operator
The purpose of the OR operator is it allows matching one of several patterns.

- (a|b): Matches either "a" or "b".
    - Example: (dog|cat) matches "dog" or "cat".

### Flags

The purpose of Flags are to modify the behavior of the regex pattern.

- i: Case-insensitive matching.
    - Example: /abc/i matches "abc" and "ABC".
- g: Global matching (find all matches).
    - Example: /abc/g finds all occurrences of "abc".
- m: Multi-line matching.
    - Example: /^abc/m matches "abc" at the start of each line.


### Conclusion


