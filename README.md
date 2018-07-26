# <a href="https://vickylai.com/introduction/" target="_blank" rel="noopener">Introduction theme for Hugo</a>
[![Build Status](https://travis-ci.com/vickylai/hugo-theme-introduction.svg?branch=master)](https://travis-ci.com/vickylai/hugo-theme-introduction)

A minimal, smooth-scrolling theme for Hugo. Can be configured as a single page site or full-featured site with many sections.

![Main page screenshot](https://github.com/vickylai/hugo-theme-introduction/blob/master/images/screenshot.png)

Features:
- Minimalist home page
    - About section with profile photo
    - Contact section with option to show your local timezone
    - Optional Projects and Blog sections
- Light and Dark themes
- Browser friendly CSS fade-in effect for some pizzaz
- Smooth scroll-to-section navigation
- Responsive and fast

# Quick start

## Get the theme

From the root of your Hugo site:
```sh
$ cd themes
$ git clone https://github.com/vickylai/hugo-theme-introduction.git introduction
```

## Configure your site

From the exampleSite, copy `config.toml` to the root folder of your Hugo site and change the fields as you like.

Important bits:

1. Set `baseURL` to your site's domain and give your site a `title`
1. Add your `firstName` and `tagLine`
1. Set the desired `introHeight` for your main page (use "medium", "large", or "fullheight")
1. Choose a "light" or "dark" `themeStyle`
1. Set your `avatar` image
1. Choose whether or not to `showBlog` on the main page
1. Choose whether or not to `showProjects` on the main page
1. Input your social site urls and font-awesome icon names - use as many as you like

## Create About and Contact pages

Run:
```sh
$ hugo new about.md
$ hugo new contact.md
```
Then edit the markdown files with the content you'd like shown in your main page's About and Contact sections.

## Preview your site locally

Use Hugo's built-in server to see your site in action as you make changes.

```
$ hugo server -t introduction
```

Visit `localhost:1313` in your browser to see a live preview of your site.

## Blog posts

To create a new blog post, run:
```
$ hugo new blog/your-post-title.md
```

## Projects

To create a new project entry, run:
```
$ hugo new projects/your-project-name.md
```

### Project front matter

Project parameters look like this:
```
---
title: "Design"
date: 2017-11-13T12:21:16-05:00
image: "img/plant.jpg"
external_link: ""
weight: 2
---
```

Projects are ordered on the main page by `weight` first, then by `date`.

The `image` will show up on the main page and in the project's details view. If you don't specify an image, the `placeholderimg` from your site's `config.toml` file will be used.

If you don't specify a `title`, only the photo will show. You can still add content to the file to "caption" the image, and this will show in the popup. (Great way to create a simple gallery!)

If you leave `external_link` empty, clicking on a project on your main page will pop up a window with the project's details. If you specify a url instead, clicking on the project on your main page will take you to that url.

# Contributing

Pull requests for bug fixes and suggestions are welcome.

Contributors are listed in [CHANGELOG.md](https://github.com/vickylai/hugo-theme-introduction/blob/master/CHANGELOG.md). Thank you so much! 🖤

# License
Copyright (C) 2018 Vicky Lai

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU Affero General Public License as
published by the Free Software Foundation, either version 3 of the
License, or (at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU Affero General Public License for more details.

You should have received a copy of the GNU Affero General Public License
along with this program.  If not, see <https://www.gnu.org/licenses/>.
