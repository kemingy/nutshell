# Nutshell

![pages](https://github.com/kemingy/nutshell/workflows/pages/badge.svg)

A theme for [Zola](https://www.getzola.org/) based on [Even](https://github.com/getzola/even).

[Live demo](https://kemingy.github.io/nutshell/)

## Features

* KaTeX with inline `$math$` and `$$equation$$`
* Support mobile
* Categories
* Archive
* Pagination[x]

## Install

Download it to your `themes` direction:

```sh
mkdir -p themes
cd themes
git clone https://github.com/kemingy/nutshell.git
```

Enable it in your `config.toml` with taxonomies:

```toml
theme = "nutshell"

taxonomies = [
    {name = "categories", rss = true},
]
```

After that, create `content/blogs/_index.md` with config:

```md
+++
paginate_by = 20 # numbers of posts in one page
sort_by = "date" # sort posts by date
+++
```

Add your posts to `content/blogs/` folder.

Copy `themes/nutshell/content/*.md` to your `content/`:

```sh
cp themes/nutshell/content/*.md content/
```

If you don't need these, you can redefine your `theme_menu` in your `config.toml`:

```toml
theme_menu = [
    {url = "$BASE_URL", name = "Home"},
    {url = "$BASE_URL/categories", name = "Categories"},
    {url = "$BASE_URL/archive", name = "Archive"},
    {url = "$BASE_URL/about", name = "About"},
    {url = "$BASE_URL/projects", name = "Projects"},
]
```
