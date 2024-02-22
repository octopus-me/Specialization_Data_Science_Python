# Regular Expression Operations

Regular expressions, often abbreviated as `regex`, serve to specify a set of strings that match a particular pattern. The functionalities within the `re` module enable you to verify whether a given string conforms to a specified regular expression.

## Basics of Regular Expressions

Regular expressions can comprise both special and ordinary characters, each serving distinct purposes:

- **Special Characters:**
    - `.` (Dot): Matches any character except newline in the default mode.
    - `^` (Caret): Matches the start of the string.
    - `$`: Matches the end of the string.
    - `*`: Denotes 0 or more repetitions of the preceding regular expression.
    - `+`: Denotes 1 or more repetitions of the preceding regular expression.
    - `?`: Denotes 0 or 1 repetition of the preceding regular expression.
    - `*?`, `+?`, `??`: Quantifiers `*`, `+`, and `?` are greedy by default, matching as much text as possible. Appending `?` after the quantifier makes it non-greedy.
    - `*+`, `++`, `?+`: These quantifiers, when `+` is appended, match as many times as possible without allowing backtracking.
    - `{m}`: Specifies exactly `m` copies of the preceding regular expression to be matched.
    - `{m,n}`: Matches from `m` to `n` repetitions of the preceding regular expression, attempting to match as many repetitions as possible.
    - `{m,n}?`: Matches from `m` to `n` repetitions, attempting to match as few repetitions as possible.
    - `{m,n}+`: Matches from `m` to `n` repetitions, attempting to match as many repetitions as possible without establishing backtracking points.
    - `\`: Either escapes special characters or indicates a special sequence.
    - `[]`: Indicates a set of characters:
        - Characters can be listed individually (e.g., `[amk]`).
        - Ranges of characters are denoted (e.g., `[A-B]`, `[0-9]`).
        - Special characters lose their significance within sets.
    - `|`: Creates a regular expression that matches either of the specified patterns.
    - `(...)`: Matches whatever regular expression is enclosed within parentheses, indicating the start and end of a group.

## Functions

The `re` module offers several functions for regex operations:

- `re.search(pattern, string, flags=0)`: Searches through the string for the first location where the pattern produces a match, returning a corresponding Match object. Returns `None` if no match is found.
- `re.match(pattern, string, flags=0)`: Checks if zero or more characters at the beginning of the string match the pattern, returning a corresponding Match object.
- `re.fullmatch(pattern, string, flags=0)`: Determines if the entire string matches the pattern, returning a corresponding match.
- `re.findall(pattern, string, flags=0)`: Returns all non-overlapping matches of the pattern in the string, presented as a list of strings or tuples.
