---
_schema: default
title: Bookshop Components
post_hero:
  heading: Bookshop Components
  date: 2025-05-08T10:03:53+12:00
  author: T Richardson
  image: /images/blog/featured-image-1.jpg
  image_alt: A child working at a computer, seen from behind.
tags:
  - bookshop
  - components
  - live editing
thumb_image_path: /images/blog/blog-thumb-1.jpg
thumb_image_alt: A birds eye view of a group of people working on laptops around a table.
seo:
  page_description: >-
    A post describing what Bookshop does in a Hugo site using CloudCannon as a
    CMS.
  canonical_url:
  featured_image: /images/blog/featured-image-1.jpg
  featured_image_alt: A child working at a computer, seen from behind.
  author_twitter_handle:
  open_graph_type: article
  no_index: false
---
[Bookshop](https://github.com/CloudCannon/bookshop/blob/main/guides/hugo.adoc) is a piece of tooling that provides a component development workflow for static websites, and aids in the creation of a page-building interface in the CloudCannon CMS.

Bookshop is fully open-source and is available on GitHub at CloudCannon/bookshop. As a tool that integrates into your codebase, we want to ensure you aren't vendor-locked to our platform. Sites built using Bookshop remain fully portable and can be built or hosted anywhere on the web.

Build custom components that non-technical editors can use in a page building experience in CloudCannon.

To add a new component run `npm run new-component <name>` in the root of your repository.

## What does Bookshop bring to Hugo?

Bookshop defines conventions for writing static components for Hugo. Using these conventions, Bookshop provides an ergonomic way to build pages out of your components, build and browse these components locally, and generate rich live editing experiences in CloudCannon.

## What does Bookshop bring to CloudCannon?

Once you have connected your site to CloudCannon, Bookshop's live editing features use your component files to generate CloudCannon configuration as part of your site build. Under the hood Bookshop creates CloudCannon Structures for each of your components, allowing your team to add and remove component objects in the CMS.

Next, when your site is loaded into CloudCannon's Visual Editor, an additional Bookshop script is loaded. This script loads your component files into the browser, alongside a Bookshop engine that understands these components. Using this, Bookshop can subscribe to data in the CMS using the CloudCannon Visual Data Preview API to render changes to your components live on the page.

Finally, after rendering components, the Bookshop script tags them with CloudCannon Visual Data Bindings. These data bindings allow you to click on elements directly in the Visual Editor and add, edit, or rearrange them visually.