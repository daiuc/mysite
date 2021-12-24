---
title:       "Build your own website with HUGO"
subtitle:    ""
description: ""
date:        2021-12-20 
author:      "Chao Dai"
image:       "/img/balance.jpg"
tags:        ["tips", "tech", "website"]
categories:  ["tech"]
---

# How to build a static personal website/blog with HUGO

![](/img/desertRoad.jpg)

## 1. Install hugo

```{bash}
brew install hugo
```

## 2. Create a new site

```{bash}
hugo new site mysite
```


## 3. Add a theme

```{python}
git init
git submodule 
```

## 4. Config toml

```{toml}
baseurl = "" # set to blank for netlify
```

## 5. Other config considerations

If you need to customize any html file, replicate the directory stucture of `themes/hugo-theme-cleanwhite/layouts` into `layouts`. For instance, I modified the footer from default theme by removing a few lines of code in the `layouts/partials/footer.html` from the theme. 

In addition, I modified `layouts/_default/baseof.html` and added `layouts/partials/analytics-gtag.html` to accomodate Google Anlaytics 4 measurement ID. 

## 6. Publish to github

## 7. Set up Netlify