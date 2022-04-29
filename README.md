# Jekyll Materialize Template for ESMValTool

This template is used for the new built ESMValTool website which is a fork of the [minima][1] and hosted with Github-Pages.

## System Requirements
These requirements are necessary for all operating systems which are the following:
  1. Ruby - click [here](https://www.ruby-lang.org/en/documentation/installation/) for installation directions.
  2. Bundler - click [here](https://bundler.io/) for installation directions.

## Repository Structure

The structure of the repository can be seen below with its explanation
```
.
├── 404.html
├── about.markdown
├── about.md
├── assets
│   ├── images
│   ├── main.scss
│   └── materialize.scss
├── calendar.md
├── CODE_OF_CONDUCT.md
├── _config.yml
├── fonts
│   └── roboto
├── Gemfile
├── Gemfile.lock
├── _includes
│   ├── disqus_comments.html
│   ├── footer.html
│   ├── google-analytics.html
│   ├── header.html
│   ├── head.html
│   └── script.html
├── index.md
├── js
│   ├── init.js
│   ├── jquery.min.js
│   └── materialize.min.js
├── _layouts
│   ├── default.html
│   ├── home.html
│   ├── page.html
│   └── post.html
├── LICENSE
├── license.md
├── LICENSE.txt
├── _posts
│   ├── 2022-02-02-11-slides-that-convinced-Boris-Johnson-about-global-warming.md
│   └── 2022-04-25-everyone-is-back-from-vacation.md
├── README.md
├── references.md
├── _sass
│   ├── main.scss
│   └── materialize
│       ├── components
│       └── materialize.scss
├── screenshot.png
├── _site
└── team.md
```

|Folder/File|Description|
|:----|:----|
|`_config.yml`| Stores configuration data which can be configured from the command line, however it is easier to specify them in this file so that it is not forgotten|
|`_includes`| This folder contains partials that can be mixed and matched by the layouts and posts for reuseability.|
|`_layouts`| This folder contains the templates that are used for each type of page.|
|`_posts`| This is where the blog posts or news can be created. The naming convention should be YEAR-MONTH-DAY-title.md. The links can be customized for each post. The post will be automatically included in the website|
|`_sass`| This folder contains sass partials that can be imported into the `main.scss`, which will be processed into a single stylesheet `main.css` that defines the style used by the website.|
|`_site`| This is where the generated site will be placed once jekyll is done transforming the website|
|`js`| This folder contains the javascript files used for the website|
|`index.html/index.md` or other markdown files| Other than the blog posts, this is where the contents of the website are created.|

More explanation regarding the other folders can be found [here](https://jekyllrb.com/docs/structure/).

## Content Writing

Website pages can be added by creating a new markdown file (`.md`) in the root directory. The markdown file should begin with its specification. For example, the development team page contains the following specifications:

```
---
layout: page
title: Development Team
url: /team.html
---
```

The `layout` tag sets the layout used for the page. The layouts that can be used is located in the `_layouts` folder. The `title` tag sets the title of the page and the `url` tag sets the link used for the page. 

The website content is written with the markdown syntax, where the guide can be found [here](https://www.markdownguide.org/basic-syntax/). However, the markdown syntax can be combined with the HTML syntax also when it is necessary.

## Customizations

Customizations of the website can be done by configuring the `.html` files located in the `_layouts` or in the `_includes` folder. Customizations guides can be found in the documentation of the website, [here](https://materializecss.com/getting-started.html).

As an example, the color of the header is changed from the default color by adding a `class` inside the `nav` tag.

```
<nav class="blue darken-4" role="navigation">
```
The `blue darken-4` specifies the color palette used for the header.

## Editing and Adding Pages

The pages in this website are located inside the markdown (`.md`) files in root. Edits can be done by customizing the text inside the markdown files and new pages can be added by creating new markdown files.

To show the new pages, it must be sure that these pages are linked inside the website. This can be done by linking the pages in the header of the website, which can be done by adding them in the `_includes/header.html` file or link them in any other files.

# Additional Resources

1. [Github Pages documentation](https://docs.github.com/en/pages)
2. [Jekyll documentation](https://jekyllrb.com/docs/)


# License

The theme is available as so I use this source [MIT License][2].

[Materialize][3] a  modern responsive front-end framework based on Material Design

Copyright © 2019 Marco Damiani. Powered by <a href="http://jekyllrb.com">Jekyll</a>

[1]: https://github.com/jekyll/minima
[2]: https://opensource.org/licenses/MIT
[3]: http://materializecss.com/
