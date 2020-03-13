# Nutshell

![pages](https://github.com/kemingy/nutshell/workflows/pages/badge.svg)

A theme for [Zola](https://www.getzola.org/) based on [Even](https://github.com/getzola/even).

[Live demo](https://kemingy.github.io/nutshell/)

## Features

* KaTeX with inline `$math$` and `$$equation$$`
* Support mobile
* Categories
* Archive
* Pagination

## Install

Download it to your `themes` direction:

```sh
mkdir -p themes
cd themes
git clone https://github.com/kemingy/nutshell.git
```

enable it in your `config.toml` with taxonomies:

```
theme = "nutshell"

taxonomies = [
    {name = "categories", rss = true},
]
```
