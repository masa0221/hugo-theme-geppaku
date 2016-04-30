Hugo ashen simple theme
=============================

## Installation

```
$ mkdir themes
$ cd themes
$ git clone https://github.com/masa0221/hugo-ashen-simple-theme hugo-ashen-simple-theme
```
See the Hugo documentation for more information.


### Post

```md
+++
date = "2016-04-30T16:44:45+09:00"
draft = false
title = "Hugo first step"
slug = "hugo-first-step"
categories = ["tech"]
tags = ["hugo"]
+++
```

## Config

Example of config.toml file:
```toml
baseurl = "http://your-site-here"
languageCode = "en-us"
title = "your site title"
theme= "hugo-ashen-simple-theme"
googleAnalytics = ""

[author]
    # If you want to display author information set these
    name = "Your name"
    # Please set account ids
    twitter  = "your twitter id"
    linkedin = "your linkedin id"
    github   = "your github id"

[params]
    # Please set id when you want to add to feature for comment
    # @see https://disqus.com
    disqus = "your disqus shortname"

    [params.sharebutton]
        # If you want to display share buttons set these
        twitter  = true
        facebook = true
        # hatena   = true # hatena is Japanese social media
        google   = true
        pocket   = true
        # Please set id when you want to display facebook
        facebookAppId = "337448966278514"

    [params.adsense]
        # If you want to display Google adsense set these
        # 1. Create file written of the adsense tag into the directory "layout/partials"
        # 2. Please set file path name omitted "layout"
        sidebar = "adsense/sidebar.html"
        content = "adsense/content.html"
```
