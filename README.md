# pkgdownMenuProblem

This is minimal example showing what appears to be a problem the yml for controlling the dropdown navigation for articles.

For example, the yml for this site in `_pkgdown.yml`, is shown below. Under menu, the articles 1 and 2 are supposed to be listed in reverse order (2 then 1), and additional lines of text are supposed to be inserted between the links to each article in the dropdown navigation. Neither of these things appear to work. Additionally, deleting one of the articles from the list under menu does not eliminate it from the dropdown navigation.

```
navbar:
  structure:
    left:
    - home
    - intro
    - reference
    - articles
    - tutorials
    - news
    right: github
  components:
    home:
      icon: fa-home fa-lg
      href: index.html
    reference:
      text: Reference
      href: reference/index.html
    articles:
      text: Articles
      menu:
      - text: This Text doesn't show
      - text: Article2
        href: articles/Article2.html
      - text: Article1
        href: articles/Article1.html
      - text: This isn't added either

```


