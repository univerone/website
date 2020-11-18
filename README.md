# website

Our homepage mlmodelci.com

## 1. Prequisities

### 1. Requirements

You should have the following tools installed.

- Ruby
- RubyGems
- GCC and Make

You can refer to <https://jekyllrb.com/docs/installation/> for more details.

### 2. Install the jekyll and bundler gems

```shell
gem install jekyll bundler
```

## 2. Contribution guidelines

### 2.1 Modify site settings

There are some configurations should be set in `_config.yml` based on this project

- title: The title of this project, which will be displayed in both navbar and homepage header area.
- description: The basic description of this project, which will be displayed in homepage header area.
- baseurl: The subpath of this website, by deafult is empty.
- url: The base hostname & protocol for your site, e.g. <http://example.com>
- git_address: The github repo url of this project.
- paper_address: The relevant paper url of this website.
- git_edit_address: The github url prefix for each markdwon file.

### 2.2 Add site logo

Here are two places to set your logo:

- `favicon.ico`
- `assets/img/logo.png`

### 2.3 Modify index page

You should modify the `index.html` file based on this project.

### 2.4 Edit doc pages

For each page under `_doc` folder, you should edit it by the following way.

#### 2.4.1 Front matter and content

All pages should have title at least in front matter.
Example as follows:

```yaml
---
title: Welcome
---

<page contents...>

```

you can refer to <https://jekyllrb.com/docs/front-matter/> for more details.

#### 2.4.2 Add Images

You should place any images, files or other resources under `assets` folder,
then you can use relative path from the website root of your file to include it in a markdwon file, such as:

```raw
![some screenshot](/assets/screenshot.jpg)
```

you can refer to <https://jekyllrb.com/docs/posts/#including-images-and-resources> for more details.

### 3. Test the website locally

You can run this jekyll project locally with the following command:

```shell
bundle exec jekyll serve
```

Then open your browser and naviagte to <http://localhost:4000> for preview.

### 4. Update github-pages gem

If the local version of `github-pages` gem is out of the date with `github-pages` gem in Github web server, there may be difference between local preview and published website, so the `github-pages` gem should be regularly updated.

```shell
bundle update github-pages
```
