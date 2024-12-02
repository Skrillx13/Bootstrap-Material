---
layout: docs
title: Installation
description: Easily install Bootstrap Material as a Hugo theme.
group: getting-started
toc: true
---

Bootstrap Material is a powerful framework for [Hugo](https://gohugo.io), a static site generator. It is complete with theming, plugins, extensions, and is batteries included, meaning it has a lot of built-in features. Bootstrap-Material is built with [Bootstrap](https://getbootstrap.com) components, and is based on [MKDocs Material](https://squidfunk.github.io/mkdocs-material/).

## 1. Install Hugo

*Read the official [Hugo installation docs](https://gohugo.io/installation/) for more information.*

Install Hugo with a Package Manager. For MacOS and Linux, use the [Homebrew](https://brew.sh) Package Manager. For Windows, use the [Chocolatey](https://chocolatey.org) Package Manager. 

{{< callout info >}}
The commands below install Hugo extended, which is always the recommended edition for Hugo as it offers advanced features.
{{< /callout >}}

### MacOS/Linux

``` sh
brew install hugo
```

### Windows

``` sh
choco install hugo-extended
```

Afterwards, check that you have installed Hugo by running `hugo version` in a terminal.

## 2. Creating the site

Create a new Hugo site by running `hugo new site mysite` in your desired directory. Replace `mysite` with a name of your choice. Run `hugo new site .` if you wish for the site to be in your exact directory. 

This will create the following structure:

``` text
.
├── hugo.toml
├── archetypes
├── assets
├── content
├── data
├── i8n
├── layouts
├── static
└── themes
```

{{< callout info >}}
You can rename `hugo.tml` to `hugo.yml` or `config.yml` if you prefer YAML syntax over TOML. For this Documentation we use YAML over TOML.
{{< /callout >}}

The themes folder is what we are focussing on, it's where themes are stored, and can be accessed by Hugo.

## 3. Using the Theme

Now, we will be installing and using the theme. Run the referenced commands at the base of your Hugo site. **Run then one-by-one not all at once.**

### Method 1. Git Clone

``` sh
git clone https://github.com/Skrillx13/Bootstrap-Material themes/Bootstrap-Material --depth=1
cd themes/Bootstrap-Material
git pull
```

### Method 2. Git Submodule

``` sh
git submodule add --depth=1 https://github.com/Skrillx13/Bootstrap-Material.git themes/Bootstrap-Material
git submodule update --init --recursive
git submodule update --remote --merge
```

### Method 3. Download a ZIP

Download Bootstrap-Material source as a ZIP file from Github Releases and extract in your themes directory at yoursite/themes/Bootstrap-Material. Here's a link to our [Latest Release](https://youtu.be/xvFZjo5PgG0?si=rpOOmqX0MdoDPXIX).

After installing the theme, reference the theme in your configuration file.

``` yml
theme: ["Bootstrap-Material"]
```

Congragulations! You have created a Hugo site with the Bootstrap-Material theme installed.