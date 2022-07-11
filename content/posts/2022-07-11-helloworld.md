---
title: New website
date: 2022-07-11
lastmod: 2022-07-12
tags: ["hugo", "www", "website"]
draft: false
---

## Welcome to my new personal website!

First of all, this website is built with [**Hugo**](https://gohugo.io/), which 
is a static website generator framework. In short, the developer (me) needs to 
only supply Hugo with static markdown documents, and it generates ready HTML 
documents that I can then upload to my web server. Simple and easy!

If you want to check out the old website which used javascript to 
pseudo-generate itself, you can find it from 
[here](http://jussihi.kapsi.fi/old).

## Building websites with Hugo

If _you_ want to build websites with Hugo, the first thing you need is the 
Hugo framework itself. Hugo can be installed on most linux distributions from 
the official application repository, for example on Arch Linux Hugo can be 
installed from pacman:
```
# pacman -S hugo
```

Now that you have Hugo installed, you can start off by creating your own 
websites! If you want to start from ground-up, you should follow 
[the official documentation](https://gohugo.io/documentation/) from Hugo's 
website.

However, you most likely just want to have something deployed quickly without 
too much hassle for yourself. In this case, you can try a ready-made 
_Hugo theme_. This is the approach I chose. The theme this website is built on 
is called "Serial Programmer", and can be found from 
[here](https://github.com/sharadcodes/hugo-theme-serial-programmer).

With a ready theme one can simply deploy a local test server with the hugo 
framework by running 
```
$ hugo server
```
in the root directory of the theme folder. This is the folder that contains 
the `config.toml` file. You might need to edit the configuration file before 
starting the local test server!

Now it's time to fiddle around and create new content for the theme. This is 
done by creating markdown-formatted files, which is then parsed by Hugo. Once 
you are happy with the outcome, you can generate the static website by running 
```
hugo
```
in the root directory. This will generate a `public` folder. The contents of 
this folder can now be uploaded to the web server. Your new website is done!

The Hugo code for this website can be found 
[from my Github](https://github.com/jussihi/jussihi.kapsi.fi)!