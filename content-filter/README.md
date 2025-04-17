# Content Filter

## Github Search Filters

### Subscribe

- https://raw.githubusercontent.com/xymoryn/ubo-filters/main/content-filter/github-search-filters.txt
- https://cdn.jsdelivr.net/gh/xymoryn/ubo-filters/content-filter/github-search-filters.txt

### Rule

```adblock
github.com##[data-testid="results-list"] > div:has(a[href^="/{username}/"])
```

### Acknowledgements

This filter was inspired by or based on the following projects:

- [Github搜索净化](https://github.com/BonjourFeng/Github-Search-Purification) by [BonjourFeng](https://github.com/BonjourFeng)

## Miscellaneous  Filters

### Subscribe

- https://raw.githubusercontent.com/xymoryn/ubo-filters/main/content-filter/misc-filters.txt
- https://cdn.jsdelivr.net/gh/xymoryn/ubo-filters/content-filter/misc-filters.txt

### Rule

- [:matches-attr()](https://github.com/gorhill/uBlock/wiki/Procedural-cosmetic-filters#subjectmatches-attrarg)
- [:has-text()](https://github.com/gorhill/uBlock/wiki/Procedural-cosmetic-filters#subjecthas-textneedle)

```adblock
pixiv.net##[data-gtm-novel-id]:matches-attr('data-gtm-label'=/(?:[^\/]*\/){4}/):upward(li)

addons.mozilla.org##.Card-contents li:has(a:has-text("{keyword}"))
```