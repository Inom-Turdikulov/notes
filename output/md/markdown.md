---
canonical_url: https://daringfireball.net/projects/markdown/
date: 2023-03-13
tags:
- outline
- markdowntip
---

> Markdown is a text-to-HTML conversion tool for web writers. Markdown allows
> you to write using an easy-to-read, easy-to-write plain text format, then
> convert it to structurally valid XHTML (or HTML).
>
> [John Gruber](https://daringfireball.net/projects/markdown/)

You can also convert markdown to tons of other formats, including PDF, using
[pandoc](./pandoc.md).

I use Markdown as my primary format for all my [notes](./notes%20types.md).

## Basics (which I use)

A paragraph is simply one or more consecutive lines of text, separated by one or
more blank lines. Normal paragraphs should not be indented with spaces or tabs.


---

Atx-style headers (h1, h2, h3, h4, h5, h6) are created by prefixing the line
with `#` characters from one to six.

# H1 header - `# H1 header`


---

Blockquotes are indicated using email-style `>` angle brackets.

> This is a blockquote. - `> This is a blockquote.`


---

For phrase emphasis I use:


- _italic_ - `*italic*`
- ~~stroke~~ - `~~stroke~~`
- **bold** - `**bold**`
- ==highlight== - `==highlight==`
- <u>underline</u> - `<u>underline</u>`
- <sup>superscript</sup> - `<sup>superscript</sup>`
- <sub>subscript</sub> - `<sub>subscript</sub>`
- <var>variable</var> - `<var>variable</var>`
- <mark>mark</mark> - `<mark>mark</mark>`
- <cite>cite</cite> - `<cite>cite</cite>`
- <ins>inserted</ins> - `<ins>inserted</ins>`


---

For lists, I use `-` as lists marker for unordered lists and `1.` for ordered:


- First item - `- First item`
- Second item - `- Second item`

  This is paragraph between list items.


- Third item - `- Third item`
  - Indented item - ` - Indented item`
  - Indented item - ` - Indented item`
    1. Indented item - ` 1. Indented item`
    2. Indented item - ` 2. Indented item`

- Fourth item - `- Fourth item`

1. First item - `1. First item`
2. Second item - `2. Second item`
3. Third item - `3. Third item`
   1. Indented item - ` 1. Indented item`
   2. Indented item - ` 2. Indented item`
4. Fourth item - `4. Fourth item`

Tables can be created using `|` and `---`:

Formatting:

| foo | bar |
| --- | --- |
| baz | bim |

```markdown
| foo | bar |
| --- | --- |
| baz | bim |
```


Minimal syntax:

|foo|bar|
|-|-|
|baz|bim|

```markdown
|foo|bar|
|-|-|
|baz|bim|
```


## TODO


- [ ] [https://daringfireball.net/projects/markdown/basics](https://daringfireball.net/projects/markdown/basics)
- [ ] [https://daringfireball.net/projects/markdown/syntax](https://daringfireball.net/projects/markdown/syntax)
- [ ] [https://github.github.com/gfm/](https://github.github.com/gfm/)