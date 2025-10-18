# Markdown Cheat Sheet

*Made by Maximilian Jäger*

---

## Basic Formatiing
### 1. Headings
One can create Headings by using "#" / stringing up to 6 "#" after another or use HTML like `<h1>` 
example:
```markdown
# Heading 1
## Heading 2
### Heading 3
#### Heading 4
##### Heading 5
###### Heading 6
```
### 2. Paragraphs & Line Breaks
Paragraphs are created by leaving one line empty and to do a line break you can leave 2 spaces at the end or use `<br>`
```markdown
Paragraph

Linebreak with 2 spaces at the end  
Other way to do a paragraph <br>
```
### 3. Bold
Use `**` or `__` to create **bold** __text__

### 4. Italic
Use `*` or `_` to *create* _italics_

### 5. Bold + Italic
***Here*** you just do ___either___ `***` or `____`

### 6. Strikethrough
Use `~~` to create ~~strikethrough~~ text

### 7. Inline Code
Use single "`" for inline code

Python has the `print()` function

---

## Lists

### 1. Unordered Lists
You can use `-`, `*` or `+` before the list item
- Test -
+ Test +
* Test *

### 2. Ordered Lists
Instead of `-` etc. use `1.`, `2.` and so on
1. Test
2. Test
3. Test

### 3. Nested Lists
Indent the under lying items by using 2 spaces
```markdown
- Item 1
  - Item 2
    - Item 3
```
- Item 1
  - Item 2
    - Item 3

---

## Links & Images

### 1. Inline Links
Format -> `[text](URL/Link)` -> [Github](https://github.com/)

### 2. Reference-Style Links
Define a Link ID and use it multiple times
```markdown
[Google][google-url]

[Google-url]: google.com
```
[Google][google-url]

[google-url]: https://www.google.com/

### 3. Images
Format -> `![alternative text](image URL/Link)` 

![Wikipedia Icon](https://upload.wikimedia.org/wikipedia/commons/thumb/8/80/Wikipedia-logo-v2.svg/103px-Wikipedia-logo-v2.svg.png)

### 4. Image + Link Combination
Format -> `[![alt text](image URL)](URL)`

[![Wikipedia Icon](https://upload.wikimedia.org/wikipedia/commons/thumb/8/80/Wikipedia-logo-v2.svg/103px-Wikipedia-logo-v2.svg.png)](https://www.wikipedia.org/)

---

## Code & Technical Content

### 1. Inline Code
Format -> 1 backtick "``"
`code`

### 2. Fenced Code Blocks
Format -> 3 backticks "```"
```
print("Hello World")
```

### 3. Syntax Highlighting
Format -> "```language name"
```python
print("Hello World")
```

---

## Quotes & Notes

### 1. Blockquotes
Format `> Quote`
> Life, uh, finds a way

### 2. Nested Blockquotes
Format `>> Nested Quote`
> Life, uh, finds a way
>> Jurassic Park

### 3. Blockquotes with Formatting
Italics, Bold etc. in a Blockquote
> **Quote:** *Life, uh, finds a way* by ***Dr. Ian Malcom***

---

## Tables

### 1. Basic Tables
Use `|` for columns and `-` for headers
```markdown
| Name | Age | 
|------|-----|
|Tim   |18   |
|Doro  |21   |
```
| Name | Age | 
|------|-----|
|Tim   |18   |
|Doro  |21   |

### 2. Alignment
Use `:` to alignt text
```markdown
|Left | Center | Right |
|:----|:------:|------:|
|A    |B       |C      |
```
|Left | Center | Right |
|:----|:------:|------:|
|A    |B       |C      |

### 3. Complex Tables
```markdown
| Feature | Description |
|----------|--------------|
| **Bold** | Highlights text |
| `Code` | Inline code |
| [Link](https://example.com) | Clickable link |
```
| Feature | Description |
|----------|--------------|
| **Bold** | Highlights text |
| `Code` | Inline code |
| [Example](https://example.com) | Clickable link |

---

## Task Lists

### Checkboxes
Format -> `- [ ]` incomplete task -> `- [x]` complete task
```markdown
- [ ] incomplete
- [x] complete
```
- [ ] incomplete
- [x] complete

---

## Dividers & Layout

### 1. Horizontal rules
Format -> `---`, `***` or `___`
---
***
___

### 2. Line Breaks
Format 2 Spaces at the end `  ` or `<br>`
```markdown
Line one  
Line two <br> Line Three  
```
Line one  
Line two <br> Line Three  

---

## Online and Collaborative Editors
### Markdown-based editors
- [Dillinger](https://dillinger.io/)
- [HackMD](https://hackmd.io/)

---

## Platform/Tool Specific: GitHub
### 1. Task Lists
```markdown
- [x] Write Markdown Cheat Sheet
- [ ] Finish the Course
```
- [x] Write Markdown Cheat Sheet
- [ ] Finish the Course

### 2. Mentioning Users
Format -> `@username` To mention someone

### 3. Automatic Linking of Issues/PRs
Format -> `#number` to reference an issue or pull request

### 4. Emoji Shortcodes
Format `:emoji_name:`  
`:tada:` -> 🎉

---

