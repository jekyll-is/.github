# Jekyll IS

Modular extensions for Jekyll: HTML + LaTeX, without double parsing, through AST manipulations.

## Module Graph

```mermaid
graph RL
  ial["is-ial-parser<br>v0.8.0"]
  kramdown["is-kramdown-hooked<br>v0.8.0"]
  statics["is-static-files<br>v0.8.0"]
  span["jekyll-is-span<br>(0%)"] --> ial
  span --> kramdown
  index["jekyll-is-index<br>(0%)"] --> span
  abbr["jekyll-is-terms<br>(0%)"] --> index
  images["jekyll-is-images<br>(0%)"] --> ial
  images --> kramdown
  images --> statics
  tocs["jekyll-is-tocs<br>(0%)"] --> images
  tocs --> index
  meta["jekyll-is-meta<br>(0%)"] --> images
  feed["jekyll-is-feed<br>(0%)"] --> meta
  robots["jekyll-is-robots<br>(0%)"]
  announcer["jekyll-is-announcer<br>v0.8.0"] --> statics
  announcer --> ial
  act-announce["action-announce<br>(0%)"] --> announcer
  publish["action-jekyll-publish<br>(0%)"] --> act-announce
  pdf["jekyll-is-pdf<br>(0%)"] --> images

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
class statics blue
```

## Gems

### Background utilities (not a plugins)

#### ✔ [is-ial-parser](https://github.com/jekyll-is/is-ial-parser) 
[![GitHub License](https://img.shields.io/github/license/jekyll-is/is-ial-parser)]([LICENSE](https://github.com/jekyll-is/is-ial-parser/blob/main/LICENSE)) 
[![Gem Version](https://badge.fury.io/rb/is-ial-parser.svg)](https://badge.fury.io/rb/is-ial-parser)

*Universal Inline Attribute List (IAL) parser for Kramdown and Jekyll plugins.*

`is-ial-parser` is a Ruby gem designed to parse Inline Attribute Lists with support for extensions, quoting, interpolation, and type conversion. 
It helps process attribute strings typically embedded in markdown or static site generators like Jekyll, enabling enhanced control over element attributes, 
classes, IDs, and custom extensions.

#### ✔ [is-kramdown-hooked](https://github.com/jekyll-is/is-kramdown-hooked)
[![GitHub License](https://img.shields.io/github/license/jekyll-is/is-kramdown-hooked)]([LICENSE](https://github.com/jekyll-is/is-kramdown-hooked/blob/main/LICENSE))
[![Gem Version](https://badge.fury.io/rb/is-kramdown-hooked.svg?d=1)](https://badge.fury.io/rb/is-kramdown-hooked)

*Extensible Kramdown parser with inner hooks for enhanced Markdown processing in Jekyll.*

`is-kramdown-hooked` is a flexible Ruby gem that extends the standard Kramdown Markdown parser by adding customizable post-parse hooks. These hooks enable developers 
to inject custom processing steps on the Abstract Syntax Tree (AST) after the default parsing, allowing for advanced Markdown manipulation and seamless integration 
into Jekyll sites or other Ruby projects using Kramdown.

#### ✔ [is-static-files](https://github.com/jekyll-is/is-static-files)
[![GitHub License](https://img.shields.io/github/license/jekyll-is/is-static-files)]([LICENSE](https://github.com/jekyll-is/is-static-files/blob/main/LICENSE))
[![Gem Version](https://badge.fury.io/rb/is-static-files.svg)](https://badge.fury.io/rb/is-static-files)

*Custom StaticFile descendants for Jekyll.*

`is-static-files` is a Ruby gem that extends Jekyll's static file handling capabilities by providing a custom `StaticFile` class. It allows you to manage static files 
that either come from a source file or from dynamic content held directly in memory. This flexibility enables programmatically generating or modifying static file content 
during the Jekyll build process.

### Announcer

#### ✔ [jekyll-is-announcer](https://github.com/jekyll-is/jekyll-is-announcer)
[![GitHub License](https://img.shields.io/github/license/jekyll-is/jekyll-is-announcer)]([LICENSE](https://github.com/jekyll-is/jekyll-is-announcer/blob/main/LICENSE))
[![Gem Version](https://badge.fury.io/rb/jekyll-is-announcer.svg?d=1)](https://badge.fury.io/rb/jekyll-is-announcer)

*Announcing new blog posts (to Telegram channel).*

`jekyll-is-announcer` is a Ruby gem for Jekyll that automates announcing new blog posts to external services, currently supporting Telegram channels and IndexNow.


<!-- ☐ ☑ -->
