# Jekyll IS

Modular extensions for Jekyll: HTML + LaTeX, without double parsing, through AST manipulations.

## Module Graph

```mermaid
graph RL
  ial["is-ial-parser v0.8.0"]
  kramdown["is-kramdown-hooked v0.8.0"]
  statics["is-static-files (0%)"]
  span["jekyll-is-span (0%)"] --> ial
  span --> kramdown
  index["jekyll-is-index (0%)"] --> span
  abbr["jekyll-is-terms (0%)"] --> index
  images["jekyll-is-images (0%)"] --> ial
  images --> kramdown
  images --> statics
  tocs["jekyll-is-tocs (0%)"] --> images
  tocs --> index
  meta["jekyll-is-meta (0%)"] --> images
  feed["jekyll-is-feed (0%)"] --> meta
  robots["jekyll-is-robots (0%)"]
  announcer["jekyll-is-announcer (0%)"] --> statics
  act-announce["action-announce (0%)"] --> announcer
  publish["action-jekyll-publish (0%)"] --> act-announce
  pdf["jekyll-is-pdf (0%)"] --> images

click ial "https://github.com/jekyll-is/is-ial-parser"
click kramdown "https://github.com/jekyll-is/is-kramdown-hooked"
click announcer "https://github.com/jekyll-is/jekyll-is-announcer"
click act-announce "https://github.com/jekyll-is/action-announce"
click publish "https://github.com/jekyll-is/action-jekyll-publish"
click images "https://github.com/jekyll-is/jekyll-is-images"
click robots "https://github.com/jekyll-is/jekyll-is-robots"
click meta "https://github.com/jekyll-is/jekyll-is-meta"
click pdf "https://github.com/jekyll-is/jekyll-is-pdf"
click tocs "https://github.com/jekyll-is/jekyll-is-tocs"
click feed "https://github.com/jekyll-is/jekyll-is-feed"
click index "https://github.com/jekyll-is/jekyll-is-index"
click span "https://github.com/jekyll-is/jekyll-is-span"
click abbr "https://github.com/jekyll-is/jekyll-is-terms"
click statics "https://github.com/jekyll-is/is-static-files"

classDef green fill:#DFD
classDef gray fill:#EEE
classDef blue fill:#DDF

class ial blue
class kramdown blue
class images gray
class announcer green
class act-announce green
class publish gray
class pdf gray
class span gray
class index gray
class feed gray
class meta gray
class robots gray
class tocs gray
class abbr gray
class statics green
```

## Gems

### ✔ [is-ial-parser](https://github.com/jekyll-is/is-ial-parser)

Universal Inline Attribute List (IAL) parser for Kramdown and Jekyll plugins.

[![GitHub License](https://img.shields.io/github/license/jekyll-is/is-ial-parser)]([LICENSE](https://github.com/jekyll-is/is-ial-parser/blob/main/LICENSE))
[![Gem Version](https://badge.fury.io/rb/is-ial-parser.svg)](https://badge.fury.io/rb/is-ial-parser)

### ✔ [is-kramdown-hooked](https://github.com/jekyll-is/is-kramdown-hooked)

Extensible Kramdown parser with inner hooks for enhanced Markdown processing in Jekyll.

[![GitHub License](https://img.shields.io/github/license/jekyll-is/is-kramdown-hooked)]([LICENSE](https://github.com/jekyll-is/is-kramdown-hooked/blob/main/LICENSE))
[![Gem Version](https://badge.fury.io/rb/is-kramdown-hooked.svg)](https://badge.fury.io/rb/is-kramdown-hooked)

### ☑ [jekyll-is-announcer](https://github.com/jekyll-is/jekyll-is-announcer)

Announcing new blog posts (to Telegram channel).

[![GitHub License](https://img.shields.io/github/license/jekyll-is/jekyll-is-announcer)]([LICENSE](https://github.com/jekyll-is/jekyll-is-announcer/blob/main/LICENSE))
[![Gem Version](https://badge.fury.io/rb/jekyll-is-announcer.svg)](https://badge.fury.io/rb/jekyll-is-announcer)

<!-- ☐ -->
