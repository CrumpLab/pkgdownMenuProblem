# pkgdownMenuProblem

This is minimal example showing what appears to be a problem the yml for controlling the dropdown navigation for articles.

The yml below should do the following, but it does not: 1) rename the "articles" tab, 2) write a line of text in the article dropdown tab, and 3) re-order the listed articles to show Article2 before Article1. Additionally, deleting one of the articles from the list under menu does not eliminate it from the dropdown navigation.

```
navbar:
  components:
    articles:
      text: New Name for Articles not showing
      menu:
      - text: This Text doesn't show
      - text: Article2
        href: articles/Article2.html
      - text: Article1
        href: articles/Article1.html
```
