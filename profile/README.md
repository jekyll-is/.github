# Jekyll IS

```mermaid
graph BT
  ial["is-ial-parser (80%)"]
  kramdown["is-kramdown-hooked (0%)"]
  images["jekyll-is-images (0%)"] --> ial
  images --> kramdown
  announcer["jekyll-is-announcer (0%)"] --> meta
  pdf["jekyll-is-pdf (0%)"] --> images
  meta["jekyll-is-meta (0%)"] --> images
  feed["jekyll-is-feed (0%)"] --> meta
  span["jekyll-is-span (0%)"] --> ial
  index["jekyll-is-index (0%)"] --> span
  span --> kramdown
  tocs["jekyll-is-tocs (0%)"] --> kramdown
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

class ial green
class kramdown gray
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
