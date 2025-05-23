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
