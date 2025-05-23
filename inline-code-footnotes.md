## Introduction

**Markdown** is a system-independent markup language that is easier to learn and use than **HTML**.

Some of the key benefits are:

1. Markdown is simple to learn, with minimal extra characters, so it's also quicker to write content.
2. Less chance of errors when writing in markdown.
3. Produces valid XHTML output.
4. Keeps the content and the visual display separate, so you cannot mess up the look of your site.
5. Write in any text editor or Markdown application you like.
6. Markdown is a joy to use!

John Gruber[^1], the author of Markdown, puts it like this:

> The overriding design goal for Markdown’s formatting syntax is to make it as readable as possible. The idea is that a Markdown-formatted document should be publishable as-is, as plain text, without looking like it’s been marked up with tags or formatting instructions. While Markdown’s syntax has been influenced by several existing text-to-HTML filters, the single biggest source of inspiration for Markdown’s syntax is the format of plain text email.
> -- <cite>John Gruber</cite>

| **Zeichenkette** | **Beschreibt**                                           |
|:-----------------|:---------------------------------------------------------|
| `^`              | Zeilenanfang                                             |
| `[abc]`          | "a" oder "b" oder "c"                                    |
| `[^abc]`         | alles außer "a", "b" oder "c" (Negation)                 |
| `^abc`           | test                                                     |
| `[ ^abc]`        | test                                                     |
| `[ ^abc]`        | test                                                     |
| `[^ abc]`        | test                                                     |
| `[a-zA-Z]`       | alle Zeichen von "a" bis "z" und "A" bis "Z" (Range)     |
| `[a-z&&[def]]`   | "d","e" oder "f" (Schnitt)                               |
| `[a-z&&[^bc]]`   | "a" bis "z", außer "b" und "c": `[ad-z]` (Subtraktion)   |
| `[a-z&&[^m-p]]`  | "a" bis "z", außer "m" bis "p": `[a-lq-z]` (Subtraktion) |


```java
^               // Zeilenanfang
[abc]           // "a" oder "b" oder "c"
[^abc]          // alles außer "a", "b" oder "c" (Negation)
^abc            // test
[ ^abc]         // test
[ ^abc]         // test
[^ abc]         // test
[a-zA-Z]        // alle Zeichen von "a" bis "z" und "A" bis "Z" (Range)
[a-z&&[def]]    // "d","e" oder "f" (Schnitt)
[a-z&&[^bc]]    // "a" bis "z", außer "b" und "c": `[ad-z]` (Subtraktion)
[a-z&&[^m-p]]   // "a" bis "z", außer "m" bis "p": `[a-lq-z]` (Subtraktion)
```

[^1]: [Markdown - John Gruber](https://daringfireball.net/projects/markdown/)
