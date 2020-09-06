# Spartan Style

Custom theme for Hugo, forked from [simple-style](https://github.com/yanlinlin82/simple-style) with the mission of being simple, clean and redeable, focusing on the content.

## Changes

- Removed github corner.
- Removed search bar on single pages.
- Removed content navigation on single pages.
- Rebuilded metadata, added og:* tags and dynamic metadata to improve SEO.
- Rebuilded baseof with footer bar and blog subtitle.
- Added 100px logo.
- Added dynamic params for links, text etc.
- Changes on CSS, mainly text-align and justify text.
- Date changes, removed hours from posts by default.
- Changes on /posts & /tags, data format, description removed from the list and group by publish date.


## License

This project is licensed under [MIT, copyright (c) 2020 Daniel Cano](https://github.com/u915/Spartan-Style/blob/master/LICENSE)

## Supported Parameters

`config.toml` example

```
[params]
# Hugo common variables
baseurl = ""
title = ""
author = ""
copyright = ""
languageCode = "" #example en-us

# Google analytics
# googleAnalytics = ""

# Theme to use
theme = "spartan-style"

# Pagination
paginate = 10
paginatePath = "page"

# Taxonomies
[taxonomies]
  tag = "tags"
  category = "categories"

# Menu
[menu]
  # Header
  [[menu.main]]
    url = "/"
    name = "Index"
    weight = 1
  [[menu.main]]
    url = "/posts/"
    name = "Posts"
    weight = 2
  [[menu.main]]
    url = "/tags/"
    name = "Tags"
    weight = 3

  # Footer
  [[menu.footer]]
    url = ""
    name = "GitHub"
    weight = 1
  [[menu.footer]]
    url = ""
    name = "Linkedin"
    weight = 2
  [[menu.footer]]
    url = "/posts/index.xml"
    name = "RSS"
    weight = 3
  [[menu.footer]]
    url = "/sitemap.xml"
    name = "Sitemap"
    weight = 4


# Links format
[permalinks]
  posts = "/posts/:year/:month/:title/"

[params]
# General
datefmt  = "2006-01-02"
subtitle = ""

# Metadata
description = "" 
ogdescription = ""
ogurl = ""
ogtitle = ""

keywords = ""
referrer = ""
author = ""


# Footer and license with copyright enabled
licensepage = "/license/"
licensetext = ""
licenselink = "https://creativecommons.org/licenses/by-nc-sa/4.0/"


# Blog images
favicon = "/images/favicon.png"
bloglogo = "/images/logo_small.png" #prepared to 100px

# CSS 
csslocation = "/css/main.css"
```
