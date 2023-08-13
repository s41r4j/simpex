# Regex _cheatsheet_

<br>

### Anchors

|    |                                                         |
| -- | ------------------------------------------------------- |
| ^  | Start of string, or start of line in multi-line pattern |
| \A | Start of string                                         |
| $  | End of string, or end of line in multi-line pattern     |
| \Z | End of string                                           |
| \b | Word boundary                                           |
| \B | Not word boundary                                       |
| \< | Start of word                                           |
| \> | End of word                                             |

<br>

### Character Classes

|    |                   |
| -- | ----------------- |
| \c | Control character |
| \s | White space       |
| \S | Not white space   |
| \d | Digit             |
| \D | Not digit         |
| \w | Word              |
| \W | Not word          |
| \x | Hexadecimal digit |
| \O | Octal digit       |

<br>

Quantifiers

> Add a ? to a quantifier to make it ungreedy

|   |           |       |           |
| - | --------- | ----- | --------- |
| * | 0 or more | {3}   | Exactly 3 |
| + | 1 or more | {3,}  | 3 or more |
| ? | 0 or 1    | {3,5} | 3, 4 or 5 |

<br>

### Escape Sequences

> "Escaping" is a way of treating characters which have a special meaning in regular expressions literally, rather than as special characters

|    |                            |
| -- | -------------------------- |
| \  | Escape following character |
| \Q | Begin literal sequence     |
| \E | End literal sequence       |

<br>

### Common Metacharacters

> The escape character is usually `\`

| ^ | [ | . | $ |
| - | - | - | - |
| { | * | ( | \ |
| + | ) |   |   |
| < | > |   |   |

<br>

### Special Characters

|      |                     |
| :--- | ------------------- |
| \n   | New line            |
| \r   | Carriage return     |
| \t   | Tab                 |
| \v   | Vertical tab        |
| \f   | Form feed           |
| \xxx | Octal character xxx |
| \xhh | Hex character hh    |

<br>

### Groups and Ranges

> Ranges are inclusive

|         |                                    |
| :------ | ---------------------------------- |
| .       | Any character except new line (\n) |
| (a\|b)  | a or b                             |
| (...)   | Group                              |
| (?:...) | Passive (non-capturing) group      |
| [abc]   | Range (a or b or c)                |
| [^abc]  | Not (a or b or c)                  |
| [a-q]   | Lower case letter from a to q      |
| [A-Q]   | Upper case letter from A to Q      |
| [0-7]   | Digit from 0 to 7                  |
| \x      | Group/subpattern number "x"        |

<br>

### Pattern Modifiers

> PCRE modifier

|     |                                          |
| :-- | ---------------------------------------- |
| g   | Global match                             |
| i * | Case-insensitive                         |
| m * | Multiple lines                           |
| s * | Treat string as single line              |
| x * | Allow comments and whitespace in pattern |
| e * | Evaluate replacement                     |
| U * | Ungreedy pattern                         |

<br>

### String Replacement

> Some regex implementations use `\` instead of `$`

|     |                           |
| --- | ------------------------- |
| $n  | nth non-passive group     |
| \$2 | "xyz" in /^(abc(xyz))$/   |
| \$1 | "" ixyzn /^(?:abc)(xyz)$/ |
| $`  | Before matched string     |
| $'  | After matched string      |
| $+  | Last matched string       |
| $&  | Entire matched string     |

<br>

### POSIX

|            |                                |
| ---------- | ------------------------------ |
| [:upper:]  | Upper case letters             |
| [:lower:]  | Lower case letters             |
| [:alpha:]  | All letters                    |
| [:alnum:]  | Digits and letters             |
| [:digit:]  | Digits                         |
| [:xdigit:] | Hexadecimal digits             |
| [:punct:]  | Punctuation                    |
| [:blank:]  | Space and tab                  |
| [:space:]  | Blank characters               |
| [:cntrl:]  | Control characters             |
| [:graph:]  | Printed characters             |
| [:print:]  | Printed characters and spaces  |
| [:word:]   | Digits, letters and underscore |

<br>

### Assertions

|            |                         |
| ---------- | ----------------------- |
| ?=         | Lookahead assertion     |
| ?!         | Negative lookahead      |
| ?<=        | Lookbehind assertion    |
| ?!= or ?<! | Negative lookbehind     |
| ?>         | Once-only Subexpression |
| ?()        | Condition [if then]     |
| ?()\|      | Condition [if then else]|
| ?#         | Comment                 |

<br>
<hr>
<br>

### References/Resources:

<br>

| cheatsheets                                                                                  |
| -------------------------------------------------------------------------------------------- |
| https://www.rexegg.com/regex-quickstart.html                                                 |
| https://www.datacamp.com/cheat-sheet/regular-expresso                                        |
| https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_expressions/Cheatsheet |
| https://gist.github.com/vitorbritto/9ff58ef998100b8f19a0                                     |
| https://cheatography.com/davechild/cheat-sheets/regular-expressions                          |

<br>

| regex editors        |
| -------------------- |
| https://regex101.com |
| https://regexr.com/  |
| https://www.regextester.com/ |