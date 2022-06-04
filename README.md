# Colonna

[![github pages](https://github.com/ale-depi/hugo-theme-colonna/actions/workflows/gh-pages.yml/badge.svg?branch=master)](https://github.com/ale-depi/hugo-theme-colonna/actions/workflows/gh-pages.yml)

Minimal theme for [Hugo](https://gohugo.io/).

## Credits

Colonna is a Hugo theme based on [Ezhil](https://github.com/vividvilla/ezhil)
and using files and ideas from [Anatole](https://github.com/lxndrblz/anatole).

## Features

* Minimal
* Responsive
* Dark mode (Auto detect from OS)
* Supports tags
* Social media links
* Syntax highlighting
* Twitter cards and opengraph tags support
* Hugo RSS feeds
* Custom CSS/JS

## Installation

From your Hugo site run the following.

```sh
cd themes
git clone https://github.com/ale-depi/hugo-theme-colonna.git
```

For more information read the
[official setup guide](https://gohugo.io/overview/installing/) of Hugo.

## Configuration

```toml
title = "My Website"

baseURL = "http://example.org/"
languageCode = "en-us"
paginate = 5

## Syntax highlighting
pygmentsUseClasses = true
pygmentsCodeFences = true
pygmentsCodefencesGuessSyntax = true

summaryLength = 20

[markup]
  [markup.goldmark]
    [markup.goldmark.renderer]
      unsafe = true

[params]
  author = "Alessandro De Piccoli"
  title = "Colonna"
  subtitle = "Minimal theme"
  disableThemeSwitcher = false
  featherIconsCDN = true
  ## Custom CSS
  ## Add your custom CSS file in assets/css/custom.css
  customCSS = false 

  ## Social links
  ## use 'fab' when brand icons, use 'fas' when standard solid icons.
  [[params.socialIcons]]
    icon = "fas fa-envelope"
    title = "E-mail"
    url = "mailto:alessandro.depiccoli@unimi.it"

  [[params.socialIcons]]
    icon = "fab fa-gitlab"
    title = "GitLab"
    url = "https://gitlab.di.unimi.it/alessandro.depiccoli/"
  
  [[params.socialIcons]]
    icon = "fab fa-github"
    title = "GitHub"
    url = "https://github.com/ale-depi/hugo-theme-colonna/"
  
[menu]
  [[menu.main]]
    name = "Home"
    url = "/"
    weight = 100
  
  [[menu.main]]
    name = "Posts"
    url = "/posts"
    weight = 200
  
  [[menu.main]]
    name = "About"
    url = "/about"
    weight = 300
  
  [[menu.main]]
    name = "Tags"
    url = "/tags"
    weight = 400

[taxonomies]
  tag = "tags"
  series = "series"
```

## Favicon

Add your favicons to `static/icons/`. Currently, you can use:
* `android-chrome-192x192.png`;
* `apple-touch-icon.png` (resolution `180x180`);
* `favicon-16x16.png`;
* `favicon-32x32.png`;
* `favicon.ico` (resolution `64x64`).

## Static page as a home page

If you prefer having a static page as your home page rather than a listing of
the latest posts, in `config.toml` change the value of the variable
`staticHome` to true:

```toml
[params]
  staticHome = true
```

then put what you want into the `_index.md` file located in the content
directory.

