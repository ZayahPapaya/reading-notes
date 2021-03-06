# Table of Contents

[Regex](regex.md)
[Class 01](class-01.md)
[Class 02](class-02.md)
[Class 03](class-03.md)
[Class 04](class-04.md)
[Class 05](class-05.md)
[Class 06](class-06.md)
[Class 07](class-07.md)
[Class 08](class-08.md)

## What is Regex?

- Regular expressions, often shortened to "regex" or "regexp", are patterns that help programmers match, search, and replace text.
- Regular expressions are very powerful, but can be hard to read because they use special characters to make more complex, flexible matches.
- A regular expression can be a single character, or a more complicated pattern.
- Regex is a means of identifying patterns in strings. When you search for patterns in a string, you can use this search pattern(the Regex pattern) to describe what you are searching for.
- We commonly use Regex to validate input, replace character patterns with other characters, refer to character patterns in a string or to parse through data collected with web scraping(data science/machine learning).
- Regex is used in almost all programming languages...JavaScript, Java, VB, C#, C / C++, Golang, Python, Perl, PHP, Ruby, R, and many others!

- DOCS:
  - <https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions>
  - <https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/RegExp>
  - <https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions/Cheatsheet>
  - <https://www.w3schools.com/jsref/jsref_obj_regexp.asp>
  - <https://www.w3schools.com/js/js_regexp.asp>
  - <https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/#regular-expressions>
  - <https://medium.com/factory-mind/regex-tutorial-a-simple-cheatsheet-by-examples-649dc1c3f285>
  - <https://medium.com/factory-mind/regex-cookbook-most-wanted-regex-aa721558c3c1>

- Check out Regex101 to test out your Regex pattern!
  - <https://regex101.com/>
  - NOTE: If you are using regex101 to test your patterns, you MUST change the Flavor (look to the left of the page to find the "Flavor") to ECMAScript(JavaScript) FIRST!!

- SYNTAX: `/pattern/modifier(s);`
  - VOCABULARY EXPLAINED:
    - The pattern to search for:   bananas
    - A regular expression:   `/bananas/`
    - A globally matched regular expressions:  `/bananas/g`

- MODIFIERS/FLAGS: used to perform case-insensitive and global searches. A Regex pattern usually comes within this form `/abc/`, where the search pattern is delimited by two slash characters `/`. At the end we can specify a flag with these values (we can also combine them each other):
  - `g`: Perform a global match (find all matches rather than stopping after the first match)
  - `i`: Perform case-insensitive matching
  - `m`: Perform multiline matching - when enabled `^` and `$` will match the start and end of a line, instead of the whole string

- BRACKETS: used to find a range of characters
  - `[abc]` Find any character between the brackets
  - `[^abc]` Find any character NOT between the brackets
  - `[0-9]` Find any character between the brackets (any digit)
  - `[^0-9]` Find any character NOT between the brackets (any non-digit)

- CAPTURING GROUPS: a way to treat multiple characters as a single unit. They are created by placing the characters to be grouped inside a set of parentheses.
  - `(dog)` Groups together the characters 'd', 'o', 'g'.
  - `(x|y)` Find any of the alternatives specified

- METACHARACTERS: are characters with a special meaning
  - `.` Find a single character, except newline or line terminator
  - `\w` Find a word character
  - `\W` Find a non-word character
  - `\d` Find a digit
  - `\D` Find a non-digit character
  - `\s` Find a whitespace character
  - `\S` Find a non-whitespace character
  - `\b` Find a match at the beginning/end of a word,
    - beginning like this: `/\bHello/`
    - end like this: `/Hello\b/`
  - `\B` Find a match, but not at the beginning/end of a word

- QUANTIFIERS: Indicate numbers of characters or expressions to match.
  - `n*` Matches any string that contains zero or more occurrences of n
  - `^n` Matches any string with n at the beginning of it
  - `n?` Matches any string that contains zero or one occurrences of n
  - `n$` Matches any string with n at the end of it
  - `n+` Matches any string that contains at least one n

- REGEXP OBJECT METHODS: patterns are used with the `exec()` and `test()` methods of RegExp
  - `test()`
    - <https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/RegExp/test>
    - The `test()` method executes a search for a match between a regular expression and a specified string.
    - Returns true or false.
    - Syntax: `pattern.test(str)`

- STRING OBJECT METHODS: `match()`, `matchAll()`, `replace()`, `replaceAll()`, `search()`, and `split()` methods
  - `match()`
    - <https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/match>
    - The `match()` method retrieves the result of matching a string against a regular expression.
    - Returns an Array whose contents depend on the presence or absence of the global (g) flag, or null if no matches are found.
      - If the g flag is used, all results matching the complete regular expression will be returned, but capturing groups will not.
      - if the g flag is not used, only the first complete match and its related capturing groups are returned. In this case, the returned item will have additional properties as described below.
      - Syntax: `str.match(pattern)`
  - `replace()`
    - <https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/replace>
    - The `replace()` method returns a new string with some or all matches of a pattern replaced by a replacement.
      - The pattern can be a string or a RegExp.
      - The replacement can be a string or a function to be called for each match.
      - Only the first occurrence will be replaced.
      - The original string is left unchanged.
    - Returns a new string, with some or all matches of a pattern replaced by a replacement.
    - Syntax: `str.replace(pattern, replacer)`

`let string = 'The rain in Spain falls mainly in the plain'`
`let pattern = /([A-Za-z]in)\b/g`
`console.log(pattern.test(string))`
`true`
(The r**ain** in Sp**ain** falls mainly in the pl**ain**)

`pattern = /\b[a-z]/gmi`
`console.log(string.match(pattern))`
`['T','r','i','S','f','m','i','t','p']`

`pattern = /\b\w/gi`
`console.log(string.replace(pattern, '-'))`
`-he -ain -n -pain -alls -ainly -n -he -lain`
