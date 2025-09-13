# Regular Expressions in Python (Summary)

Python uses the **`re` module** to work with regex.

## Common Functions
- `re.match(pattern, string)` → checks for a match at the beginning of the string.
- `re.search(pattern, string)` → searches the whole string.
- `re.findall(pattern, string)` → returns all matches as a list.
- `re.sub(pattern, repl, string)` → replaces matches with replacement text.
- `re.split(pattern, string)` → splits by the regex pattern.

## Meta-characters
- `.` → any character except newline  
- `^` → start of string  
- `$` → end of string  
- `[]` → character set (e.g., `[aeiou]`)  
- `|` → OR  
- `()` → grouping  

## Quantifiers
- `*` → 0 or more  
- `+` → 1 or more  
- `?` → 0 or 1  
- `{n}` → exactly n  
- `{n,}` → n or more  
- `{n,m}` → between n and m  

## Special Sequences
- `\d` → digit  
- `\D` → non-digit  
- `\w` → word char  
- `\W` → non-word char  
- `\s` → whitespace  
- `\S` → non-whitespace  
- `\b` → word boundary  

## Example
```python
import re

text = "My phone number is 123-456-7890."
print(re.findall(r"\d{3}-\d{3}-\d{4}", text))
# Output: ['123-456-7890']

