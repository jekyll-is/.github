# Jekyll IS

```mermaid
graph BT
  images[jekyll-is-images] --> ial[is-ial-parser]
  images --> kramdown[is-kramdown-hooked]
  announcer[jekyll-is-announcer] --> meta
  pdf[jekyll-is-pdf] --> images
  meta[jekyll-is-meta] --> images
  feed[jekyll-is-feed] --> meta
  span[jekyll-is-span] --> ial
  index[jekyll-is-index] --> span
  span --> kramdown
  tocs[jekyll-is-tocs] --> kramdown
  robots[jekyll-is-robots]

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
```
