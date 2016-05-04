+++
date = "2016-05-03T11:03:05+09:00"
draft = false
title = "How to install Geppaku theme"
slug = "how-to-install-geppaku-theme"
categories = ["technology"]
tags = [
  "Hugo",
  "Hugo theme",
  ]
+++
Geppaku is bluish white theme for [Hugo](http://gohugo.io/).  
It is color name in Japan. Chinese character is "月白".

> 月白（げっぱく）とは、月の光を思わせる薄い青みを含んだ白色のことです。
<small>via http://irocore.com/geppaku/</small>

Geppaku is the white color including a thin blue that reminiscent of the light of the moon.  
(If that translate is wrong, please inform me using PullRequest.)

## Screenshot
### Index page
![list](/images/2016/05/03/list.png)

### Post page
![post](/images/2016/05/03/screenshot.png)


## Installation

```
$ mkdir themes
$ cd themes
$ git clone https://github.com/masa0221/hugo-theme-geppaku hugo-theme-geppaku
```
See the Hugo documentation for more information.


### Config

Example of config.toml file:
```toml
baseurl = "http://your-site-here/"
languageCode = "en-us"
title = "your site title"
theme= "hugo-theme-geppaku"
googleAnalytics = "" # Optional
disqusShortname = "" # Optional

[author]
    # If you want to display author information set these
    # This is Optional values
    name = "Your name"

    # Please set account ids
    # This is Optional values
    twitter  = "your twitter id"
    linkedin = "your linkedin id"
    github   = "your github id"

[params]
    [params.sharebutton]
        # If you want to display share buttons set these
        # This is Optional values
        twitter  = true
        facebook = true
        # hatena   = true # hatena is Japanese social media
        google   = true
        pocket   = true
        # Please set id when you want to display facebook
        facebookAppId = "your app id"

    [params.adsense]
        # If you want to display Google adsense set these
        # This is Optional values
        # 1. Create file written of the adsense tag into the directory "layouts/partials"
        # 2. Please set file path name omitted "layouts/partials"
        sidebar = "adsense/sidebar.html"
        content = "adsense/content.html"
```
You can delete optional parameter.
Please delete unnecessary parameter.


### New Post
#### Create markdown file
```sh
hugo new post/2016/05/hello-hugo.md
```

#### Example of the toml file

```
+++
date = "2016-04-30T16:44:45+09:00"
draft = false
title = "Hello Hugo!"
slug = "hello-hugo"
categories = ["tech"]
tags = [
  "hugo",
  "golang",
  ]
+++
Hello Hugo!
```
