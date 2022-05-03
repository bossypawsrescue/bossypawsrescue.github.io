# :construction: Bossy Paws Rescue [:link:](https://bossypawsrescue.github.io/) :dog: :cat:

[![pages-build-deployment](https://github.com/bossypawsrescue/bossypawsrescue.github.io/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/bossypawsrescue/bossypawsrescue.github.io/actions/workflows/pages/pages-build-deployment)

This is the website for the organization. It is constructed using [:link:Github Pages](https://docs.github.com/en/pages) which uses [:link:Jekyll](https://jekyllrb.com/docs/) under the hood to statically generate the website. The following are some common use cases in order to make changes to the website.

## Modify an exisiting page

Depending on the which page, you should be able to find it based off of the URL. For instance, the `/contact-us` page is located in the main project folder at `contact-us.md`. The only exception is the home page which is called `index.md`. This is unfortunately just a quirk of Jekyll that can not be changed. 

Making a change to a file is as easy as

1. Open it in Github
2. Edit it
    - Jekyll renders out pages using the markdown (.md) file format. This is the Github version of markdown which has some specific features for Github and Jekyll. Helpful information can be found at https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax to help figure out how to write things. Markdown is a file format that eventually gets rendered into HTML. This means, in addition to markdown text, you can also just write plain HTML.
3. Commit the changes
    - This is going to be the most confusing part for anyone who is not familiar with Git. The basic idea is that every change is tracked in Git via a [commit](https://github.com/bossypawsrescue/bossypawsrescue.github.io/commits). This ensures that everyone is aware of what has changed and any negative changes could be removed or at least identified. You just have to provide a helpful message in the text field and `Commit changes` to the code. This will make the changes visible for others to see and will kick off Jekyll to rebuild and deploy the website. This can be viewed at https://github.com/bossypawsrescue/bossypawsrescue.github.io/actions

## Add a new page

Adding a new page is easy since you just have to create a new markdown file in the project. This can be done from the `Add file -> Create new file` button. You can then provide a file name which will correspond to the URL that the page gets published to. For instance, `<file name>.md` will be published to `/<file-name>` on the website.

After commiting the changes, you will also need to reference the new page either in an existing page or in the `layout`. More information on editing a `layout` is in the following section.

## Customize what is shown on each page

Jekyll uses a `layout` templating system where the templates for pages reside in the [_layouts](_layouts) folder. By default, Jekyll will use the `default` layout which corresponds to the `default.html` file. This file has content that should be included on every page of the website. This means things that are in the header, navigation, and footer. It acts as the skeleton for pages so they can inject their content when rendered. 

For example, the `{{ content }}` tag tells Jekyll that we would like to inject the page's `content` at the specified location. A page's `content` is anything that is written after the front matter in the markdown file. More information about front matter at https://jekyllrb.com/docs/front-matter/, but it is essentially the information inside of the triple dash block.

```md
---
title: "This is a page"
---
```
