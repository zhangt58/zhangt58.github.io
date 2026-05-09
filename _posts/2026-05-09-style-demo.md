---
layout: post
title: Style Demo
categories: [demo]
tag: demo
---

## H2 Heading

### H3 Heading

#### H4 Heading

##### H5 Heading

###### H6 Heading

---

## Body Paragraphs

This is a regular body paragraph. It should feel clean and readable, not monospaced.

Here's a paragraph with **bold text**, *italic text*, ~~strikethrough~~, and a [hyperlink](https://example.com) to verify link styling with the cyan underline accent.

---

## Lists

### Unordered List

- First item with `inline code` snippet
- Second item with **bold** and *italic*
- Third item with a [link](https://example.com)

### Ordered List

1. Step one — with `some code`
2. Step two
3. Step three

### Definition List

Term 1
:   Definition of term 1

Term 2
:   Definition of term 2 with `inline code`

---

## Inline Code

Here is some `inline code` in the middle of a sentence. It should render in JetBrains Mono with a subtle cyan-tinted background and border, distinct from the surrounding body text.

Another example: run `pip install numpy` to install NumPy.

---

## Code Blocks

### Python

```python
def fibonacci(n: int) -> list[int]:
    """Generate Fibonacci sequence up to n terms."""
    if n <= 0:
        return []
    if n == 1:
        return [0]

    sequence = [0, 1]
    while len(sequence) < n:
        sequence.append(sequence[-1] + sequence[-2])
    return sequence

for i, val in enumerate(fibonacci(10)):
    print(f"F({i}) = {val}")
```

### Shell

```bash
$ cd /home/tong/workspace/zhangt58.github.io
$ git status
On branch main
Your branch is up to date with 'origin/main'.
nothing to commit, working tree clean
```

### HTML

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Document</title>
</head>
<body>
    <h1>Just a test</h1>
</body>
</html>
```

---

## Blockquotes

> This is a blockquote. It should render in JetBrains Mono with a cyan left border and a prompt character prepended.

> Nested or multi-line blockquotes:
>
> > Even deeper nesting should maintain the monospace styling and cyan accent throughout.

---

## Tables

| Method   | Status | Description             |
|----------|--------|-------------------------|
| `GET`    | 200    | Retrieve a resource     |
| `POST`   | 201    | Create a new resource   |
| `PUT`    | 200    | Update an existing item |
| `DELETE` | 204    | Remove a resource       |
| `PATCH`  | 200    | Partially update        |

---

## Horizontal Rule

---

## Images

![Sample image](https://placehold.co/800x400/0d1117/00bcd4?text=Sample+Image)

*Figure caption with citation*[^1]

[^1]: This is an image caption / footnote rendered by Chirpy.

---

## Keyboard Keys

Press `Ctrl` + `C` to copy, `Ctrl` + `V` to paste, and `Esc` to cancel.

---

## Footnotes

Here is a sentence with a footnote reference[^2]. And another one with a second footnote[^3].

[^2]: This is the first footnote. It appears at the bottom of the post.
[^3]: This is the second footnote. Footnotes use the standard Chirpy styling.

---

## URLs

URLs can be made in a handful of ways:

* A named link to [Example](https://example.com)
* An inline URL like <https://github.com/zhangt58>
* A reference-style link to [Markdown Guide][1]

[1]: https://www.markdownguide.org/

---

*That covers all the visual styles on the blog — headings in Montserrat Bold/Uppercase, body in Inter, code/meta/tags/TOC/blockquotes/tables in JetBrains Mono, with cyan accent throughout.*
