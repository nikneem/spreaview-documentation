---
title: "Adding Content"
linkTitle: "Adding Content"
weight: 1
description: >
  Add different types of content to your Docsy site.
---

So you've got a new Hugo website with Docsy, now it's time to add some content! This page tells you how to use the theme to add and structure your site content.

## Content root directory

You add content for your site under the **content root directory** of your Hugo site project - either `content/` or a [language-specific](/docs/language/) root like `content/en/`. The main exception here is static files that you don't want built into your site: you can find out more about where you add these below in [Adding static content](#adding-static-content). The files in your content root directory are typically grouped in subdirectories corresponding to your site's sections and templates, which we'll look at in [Content sections and templates](#content-sections-and-templates).

You can find out more about Hugo directory structure in [Directory Structure Explained](https://gohugo.io/getting-started/directory-structure/#directory-structure-explained).

## Content sections and templates

Hugo builds your site pages using the content files you provide plus any templates provided by your site's theme. These templates (or _"layouts"_ in Hugo terminology) include things like your page's headers, footers, navigation, and links to stylesheets: essentially, everything except your page's specific content. The templates in turn can be made up of _partials_: little reusable snippets of HTML for page elements like headers, search boxes, and more.

Because most technical documentation sites have different sections for different types of content, the Docsy theme comes with the [following templates](https://github.com/google/docsy/tree/main/layouts) for top-level site sections that you might need:

- [`docs`](https://github.com/google/docsy/tree/main/layouts/docs) is for pages in your site's Documentation section.
- [`blog`](https://github.com/google/docsy/tree/main/layouts/blog) is for pages in your site's Blog.
- [`community`](https://github.com/google/docsy/tree/main/layouts/community) is for your site's Community page.

It also provides a [default "landing page" type of template](https://github.com/google/docsy/tree/main/layouts/_default) with the site header and footer, but no left nav, that you can use for any other section. In this site and our example site it's used for the site [home page](/) and the [About](/about/) page.

Each top-level **section** in your site corresponds to a **directory** in your site content root. Hugo automatically applies the appropriate **template** for that section, depending on which folder the content is in. For example, this page is in the `docs` subdirectory of the site's content root directory `content/en/`, so Hugo automatically applies the `docs` template. You can override this by explicitly specifying a template or content type for a particular page.

If you've copied the example site, you already have appropriately named top-level section directories for using Docsy's templates, each with an index page ( `_index.md` or `index.html`) page for users to land on. These top-level sections also appear in the example site's [top-level menu](/docs/adding-content/navigation/#top-level-menu).
