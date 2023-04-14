# Regex in Javascript

Let's break down the regex '/^([a-zA-Z0-9]+-)*[a-zA-Z0-9]+@[a-zA-Z0-9]+\.[a-zA-Z]{2,}$/g' into its particular components and see what each part does!

## Table of Contents

- Delimiters '/' and '/g'
- Caret '^' - Start of Line
- Capturing Group '([a-zA-Z0-9]+-)*'
- Character Class '[a-zA-Z0-9]+'
- At Symbol '@'
- Domain Name '[a-zA-Z0-9]+'
- Dot '\.'
- Top-level Domain '[a-zA-Z]{2,}'
- '$' - End of Line

### '/' and '/g': These are delimiters used to define the begining and end of this regex pattern. The 'g' at the end denotes "global" and shows that the regex should match all occurrences in the input string, rather than stopping at the first match.

### '^': This is a caret symbol that stands for the beginning of a line in the input string. It assures that the regex pattern starts matching from the beginning of the string.

### '([a-zA-Z0-9]+-)*': This is a capturing group enclosed in parentheses. It matches 1 or more occurrences of alphanumeric characters followed by a hyphen, and allows for 0 or more reiteration of the pattern. The asterisk outside the capturing group indicates that this group can repeat 0 or more times.

### '[a-zA-Z0-9]+': This is a character class that matches 1 or more occurrences of alphanumeric characters (letters or digits).

### '@': This matches the '@' symbol, which is a required character in a email address.

### ['a-zA-Z0-9]+': This is another character class that matches 1 or more occurrences of alphanumeric characters (letters and digits). This represents the domain name in the email address.

### '\.': This matches a dot (.) character. The backslash '\' is a escape character used to treat the dot as a literal character, rather than a special character with its entire meaning.

### '[a-zA-Z]{2,}': This is a character class that matches 2 or more occurrences of uppercase or lowercase alphabetical characters. It represents the top-level domain in the email address.

### '$': This is a dollar sign that denotes the end of a line in the input string. This ensures that the regex pattern ends matching at the end of the string.

### https://regex101.com/

## Mikaela McConkey
