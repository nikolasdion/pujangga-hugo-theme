# Pujangga Hugo Theme

A minimal [Hugo](https://gohugo.io/) theme for my poetry blog [pujangga](https://pujangga.nikolasdion.com/).

This theme is based on [smol](https://github.com/colorchestra/smol) by [morph](https://morph.sh), which in turn is based on [Blank](https://github.com/Vimux/Blank) by [Vimux](https://github.com/Vimux). The colour palette is based on [Rosé Pine](https://rosepinetheme.com/)

## Installation

In the root of your Hugo project, run:

```sh
git submodule add https://github.com/nikolasdion/pujangga-hugo-theme themes/pujangga
```

Next, open `config.toml` in the base of the Hugo site and ensure the theme option is set to `pujangga`.

```toml
theme = "pujangga"
```

Lastly, add the following lines to your `config.toml` to set site parameters and make use of all the menu entries in the header and footer sections if you need them.

```toml
# Parameters
[params]
subtitle = "Your blog subtitle goes here!"
dateFmt = "02 January 2006"

# Header
[menu]
[[menu.main]]
identifier = "posts"
name = "Posts"
url = "/posts/"
weight = 1

[[menu.main]]
identifier = "categories"
name = "Categories"
url = "/categories/"
weight = 2

[[menu.main]]
identifier = "tags"
name = "Tags"
url = "/tags/"
weight = 3

# Footer
[[menu.footer]]
name = "Github"
url = "https://github.com/example"
weight = 1

[[menu.footer]]
name = "Another link"
url = "https://example.com/"
weight = 2
```

## Optional features

### Custom copyright text

Add `copyright = "Your text here"` - in the `config.toml`` to change the copyright notice in the footer.

### Image captions

You can add captions to images (technically using `<figcaption>` HTML tags) by adding titles, like so: `![Alt text here](/path/to/image.png "Put your caption here!")`.
