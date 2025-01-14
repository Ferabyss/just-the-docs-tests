---
title: Default
parent: Order
nav_order: 1
has_children: true
---

# Default Order

When `nav_order` fields are omitted, the pages are ordered alphabetically by their titles.

By default, all Capital letters come before all lowercase letters;
you can add `nav_sort: case_insensitive` in the configuration file to ignore the case).

Digits precede letters, and numeric titles are ordered lexicographically:
`10` precedes `2` (in contrast to explicit numeric `nav_order` values).

1.  Check that the titles of the children of this page are shown in the order:
    ```
    2
    10
    A
    Aa
    aa
    ```

{: .note }
The default order of numeric titles depends on which version of Jekyll is used
to build the site: 
the default build on GitHub Pages uses Jekyll 3.9 and gives lexicographic order,
but when using Jekyll 4, `2` precedes `10`. ❌
