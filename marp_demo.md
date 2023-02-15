---
marp: true
theme: gaia
class: gaia
author: Petr Ankudinov
size: 16:9
paginate: true
math: mathjax
---

# Just Another Marp Demo <!-- fit -->

<div style="text-align: center;"><br><br>Marp is very simple to write!</div>

![bg](https://fastly.picsum.photos/id/413/720/576.jpg?hmac=1scuUq-W26w3-YZUggyGJyj6fkV8m2zCYaocFmZ052o)

<!-- Do not add page number on this slide -->
<!--
_paginate: false
-->

---

# What is Marp

<style scoped>section {font-size: 30px;}</style>

- A framework to write slides in Markdown
- Check [Marp documentation](https://marp.app/)
- There are alternatives to Marp. For example [Slidev](https://sli.dev/)
- Advantages of Marp:
  - has VSCode extension`*`
  - very simple
- Disadvantages:
  - no support for some advanced features, like animations

<br>

> `*`: TBH Slidev has VSCode extension as well.

---

# Multiple H1 headers, HTML tags <!-- fit -->

<style scoped>section {font-size: 21px;}</style>

- Using multiple H1 headers and HTML tags requires Markdown linter adjustment
- Here is an example of linter settings as code block with highlighting:

```json
{
    "markdownlint.config": {
        "default": true,
        // allow multiple H1s for Marp
        "MD025": false,
        "MD033": {
            "allowed_elements": [
                "div",
                "span",
                "style",
                "br"
            ]
        }
    },
    "markdown.marp.enableHtml": true
}
```

- `enableHtml` required to enable all HTML elements in Marp

---

# Spot Directives

<!-- _backgroundColor: #004643 -->
<!-- _color: #abd1c6 -->

- It is possible to change the background colour and text colour for a single slide
- Or adjust style for any other element if necessary

---

# Working with Pictures

![bg blur:4px](https://fastly.picsum.photos/id/519/720/576.jpg?hmac=GGcVzYOxQlagVRGL3eA7V4ez6mRsc_xan0mWqNTN5dM)
![bg](https://fastly.picsum.photos/id/24/720/576.jpg?hmac=2l2ISqSEDngDB0p1hldccCFV0pcNzfnz3oxZZkJq0AE)
![bg sepia](https://fastly.picsum.photos/id/49/720/576.jpg?hmac=L9I_9gudh4-ltYjnzaYfghBZaMUMUluJTTAtuxQtUiM)

- The alignment can be changed by using `vertical` <span style="color: black;">keyword</span>.
- And let's add some emojis here: `😄 ⏫ 👍 🚀 🎱`

---

# Just a Table

| Table &emsp;&emsp;| Layout&emsp;&emsp; | Example&emsp;&emsp; |
|:------|:------:|--------:|
|⬅️ left | centred | right ➡️ |
