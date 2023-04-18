---
title: "Setting Up a Hugo Blog"
date: 2023-04-18
author: "John Doe"
tags: ["hugo", "blogging"]
---
Hugo is a popular open-source static site generator written in Go (also known as Golang). It allows you to create fast and flexible websites, blogs, and other types of web content without the need for a dynamic server-side language or database. Hugo generates static HTML files that can be served directly by a web server, resulting in lightning-fast page load times and improved performance.

## Step 1: Install Hugo

The first step is to install Hugo on your local machine. Hugo is available for Windows, macOS, and Linux platforms. You can download the latest version of Hugo from the official Hugo website at https://gohugo.io/getting-started/installing/.

Follow the installation instructions for your operating system to install Hugo.

## Step 2: Create a New Hugo Site

Once Hugo is installed, you can create a new Hugo site by running the following command in your terminal or command prompt:



This will create a new Hugo site in a directory named `myblog`. You can replace `myblog` with the name of your blog or website.

## Step 3: Choose a Hugo Theme

Hugo provides a wide range of themes that you can use for your blog or website. You can choose a theme from the official Hugo theme directory at https://themes.gohugo.io/. To install a Hugo theme, you can either download the theme manually and extract it into the `themes` directory of your Hugo site, or you can use the Hugo theme manager to install the theme directly.

For example, to install the popular "Ananke" theme, you can run the following command in your terminal or command prompt:


This will add the Ananke theme as a submodule in your Hugo site and set it as the default theme in your `config.toml` configuration file.

```
cd myblog
git init
git submodule add https://github.com/budparr/gohugo-theme-ananke.git themes/ananke
echo 'theme = "ananke"' >> config.toml
```

## Step 4: Create Your First Blog Post

Next, you can create your first blog post using Hugo's built-in command:


This will create a new Markdown file for your first blog post in the `content/posts` directory of your Hugo site.

You can edit the generated Markdown file to write your blog post using Markdown syntax. You can also add front matter to the top of the Markdown file to provide metadata for your blog post, such as title, date, author, etc.

For example, a typical front matter for a blog post might look like this:

```
---
title: "My First Blog Post"
date: 2023-04-18
author: "John Doe"
tags: ["hugo", "blogging"]
---
```
### Step 5: Customize Your Blog
You can customize various aspects of your Hugo blog by modifying the config.toml configuration file in the root directory of your Hugo site. The configuration file allows you to set options such as the site title, description, language, theme, and more.

You can also create custom layouts, partials, and CSS styles to customize the appearance of your blog. Hugo uses the Go template language for templating, so you may need to learn some basic Go template syntax to customize your blog's layout.

Since you will be playing around with markdown here is a cheatsheet - https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet#code

