# Material

Material is a theme for Hugo.

## Features

- Responsive design.
- Automatic dark theme.
- Show related pages.
- Supported languages: :us:, :es:

## Installation

In the folder of your Hugo site:

```sh
git submodule add https://github.com/alcarazzam/hugo-material.git themes/material
```

In your `hugo.toml`:

```toml
theme = 'material'
```

## Configuration

Example configuration file:

```toml
baseURL = 'https://example.org/'
languageCode = 'en-us'
defaultContentLanguage = 'en'
title = 'My New Hugo Site'
theme = 'material'

enableRobotsTXT = true

[pagination]
  pagerSize = 10

[taxonomies]
  tag = 'tags'
  series = 'series'

[menus]
[[menus.main]]
  name = 'Tags'
  pageRef = '/tags/'
  weight = 10
[[menus.footer]]
  name = 'Example'
  url = 'https://example.com/'
  weight = 10

[params]
  showRelated = true
  footerHtml = "Copyright 2024. All rights reserved."
  me = 'https://example.com'
  logo = '/logo.png'

  [params.author]
    email = 'example@example.com'
    name = 'Me'
    mastodon = '@example@example.com'
```

## Roadmap

- [x] Customize theme.
- [ ] Archive page.
- [ ] LaTeX/TeX support.

## License

[MIT License](LICENSE).
