# Jekyll IS

```mermaid
graph BT
  ial["is-ial-parser v0.8.0"]
  kramdown["is-kramdown-hooked (0%)"]
  tocs["jekyll-is-tocs (0%)"] --> kramdown
  images["jekyll-is-images (0%)"] --> ial
  images --> kramdown
  announcer["jekyll-is-announcer (0%)"] --> meta
  pdf["jekyll-is-pdf (0%)"] --> images
  meta["jekyll-is-meta (0%)"] --> images
  feed["jekyll-is-feed (0%)"] --> meta
  span["jekyll-is-span (0%)"] --> ial
  index["jekyll-is-index (0%)"] --> span
  span --> kramdown
  robots["jekyll-is-robots (0%)"]

click ial "https://github.com/jekyll-is/is-ial-parser"
click kramdown "https://github.com/jekyll-is/is-kramdown-hooked"
click announcer "https://github.com/jekyll-is/jekyll-is-announcer"
click images "https://github.com/jekyll-is/jekyll-is-images"
click robots "https://github.com/jekyll-is/jekyll-is-robots"
click meta "https://github.com/jekyll-is/jekyll-is-meta"
click pdf "https://github.com/jekyll-is/jekyll-is-pdf"
click tocs "https://github.com/jekyll-is/jekyll-is-tocs"
click feed "https://github.com/jekyll-is/jekyll-is-feed"
click index "https://github.com/jekyll-is/jekyll-is-index"
click span "https://github.com/jekyll-is/jekyll-is-span"

classDef green fill:#DFD
classDef gray fill:#EEE
classDef blue fill:#DDF

class ial blue
class kramdown green
class images gray
class announcer gray
class pdf gray
class span gray
class index gray
class feed gray
class meta gray
class robots gray
class tocs gray
```

## Gems

### ✔ [is-ial-parser](https://github.com/jekyll-is/is-ial-parser)

Universal Inline Attribute List (IAL) parser for Kramdown and Jekyll plugins.

[![GitHub License](https://img.shields.io/github/license/jekyll-is/is-ial-parser)]([LICENSE](https://github.com/jekyll-is/is-ial-parser/blob/main/LICENSE))
[![Gem Version](https://badge.fury.io/rb/is-ial-parser.svg)](https://badge.fury.io/rb/is-ial-parser)

### ☑ [is-kramdown-hooked](https://github.com/jekyll-is/is-kramdown-hooked)

Extensible Kramdown parser with inner hooks.

[![GitHub License](https://img.shields.io/github/license/jekyll-is/is-kramdown-hooked)]([LICENSE](https://github.com/jekyll-is/is-kramdown-hooked/blob/main/LICENSE))
[![Gem Version](https://badge.fury.io/rb/is-kramdown-hooked.svg)](https://badge.fury.io/rb/is-kramdown-hooked)

