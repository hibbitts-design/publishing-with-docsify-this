![](images/pawel-czerwinski-EIfU0IUqZw8-unsplash.jpg ':class=banner-image')

# Markdown Publishing with Docsify&#8288;&#8211;&#8288;This

An introduction to Markdown publishing using the open source [Docsify-This.net](https://docsify-this.net/) project.

## Markdown

### What is Markdown? 
Markdown is a syntax to format the display of content stored as plain text - similar but simpler than HTML formatting

### Why Markdown? 

* System-independent
* Text only format (perfect for version control)
* Separation of content vs. presentation
* Human-readable (i.e. more than HTML)
* Can also contain HTML snippets

### Markdown Examples

```
# Your H1 Text Here  
## Your H2 Text Here  

_your italic text here_  

**your bold text here**  

* your unordered list item here  

  1. your numbered (and indented) list item here   

[link title](www.google.com)  
```
Tip: To ensure a new paragraph after text in markdown, put two spaces after the end of the line

## Publishing with Markdown

* Markdown Converters
  * For example, [Pandoc](https://pandoc.org/)
* Markdown Static Site Builders
  * For example, [Jekyll](https://jekyllrb.com/)
* Markdown Dynamic Renderers
  * For example, [Docsify](https://docsify.js.org)

## Docsify-This

[Docsify-This](https://github.com/hibbitts-design/docsify-this) is an open source Web app, built using the [Docsify Open Publishing Kit](https://github.com/hibbitts-design/docsify-open-publishing-starter-kit), that can quickly display online Markdown files as web pages (i.e. no file uploads or build processes).   

_Being open source, you can even host your own Docsify-This instance! No platform lock-in here._

### Example Docsify-This Usage Scenarios

* Publish your Markdown files as standalone web pages, with no website setup or build process required
* Visually style your standalone web pages using a point-and-click Web Page Builder
* Share existing GitHub-hosted Markdown files as standalone web pages, with an optional 'Edit this Page' link
* Seamlessly embed constraint-free Markdown/HTML, which you have authored, into other platforms (e.g. LMS or CMS)
* Reuse existing Markdown content by seamlessly embedding it within other platforms (e.g. LMS or CMS)
* Utilize the supported URL parameters when embedding content to match each destination platform better visually

### Docsify-This Web Page Builder

To use the Docsify-This **Web Page Builder** enter the URL for an online Markdown file and tap the ???View as Standalone Web Page??? button. The Markdown file will then  be rendered as a standalone Web page with it???s own URL that can then be copied and shared.

![Docsify-This Web Page Builder](images/docsify-this-web-page-builder.png ':class=image-75-border')  
_Figure 1. Docsify-This Web Page Builder_

### Example Docsify-This URL

```html
https://docsify-this.net/?basePath=https://raw.githubusercontent.com/hibbitts-design/docsify-this-one-page-article/main&homepage=home.md
```

![Docsify-This Rendered Markdown File](images/docsify-this-rendered-markdown-file.png ':class=image-75-border')  
_Figure 2. Docsify-This Rendered Markdown File_

Docsify-This rendered Web pages are also perfect for embedding, with the ability to visually style Docsify-This pages to the destination platform.

### Docsify-This URL Editing

You can also render other Markdown files in the same repository by directly editing the Docsify-This URL parameter **homepage**, for example:

```html
https://docsify-this.net/?basePath=https://raw.githubusercontent.com/hibbitts-design/docsify-this-one-page-article/main&homepage=anotherfile.md
```

### Docsify-This Web Page Styling

[URL Parameters](https://docsify-this.net/#/?id=page-appearance-url-parameters) (any Markdown file)  
For example, `font-family`, `font-size`, `link-color` and `line-height`  

[Markdown CSS Classes](https://docsify-this.net/#/?id=supported-markdown-css-classes)  
For example, `badge`, `banner-image`, `button`, and `row` & `column`

### Embedding Docsify-This Pages

#### Example Docsify-This Redirect Tool URL 

![Docsify-This Module](images/docsify-this-page.png ':class=image-75-border')  
_Figure 3. Docsify-This External URL (used with the Redirect Tool), for example https://canvas.sfu.ca/courses/76289/external_tools/36154_

```html
url=https://docsify-this.net/?basePath=https://raw.githubusercontent.com/paulhibbitts/cmpt-363-222-pages/main&homepage=resources.md&edit-link=https://github.com/paulhibbitts/cmpt-363-222-pages/blob/main/resources.md&font-family=Lato%20Extended,Lato,Helvetica%20Neue, Helvetica,Arial,sans-serif&font-size=1&hide-credits=true
```

#### Example Docsify-This External URL 

![Docsify-This Module](images/docsify-this-module.png ':class=image-75-border')  
_Figure 4. Docsify-This External URL (used as a Canvas LMS Module), for example https://canvas.sfu.ca/courses/76289/modules/items/2816273_

```html
https://docsify-this.net?basePath=https://raw.githubusercontent.com/paulhibbitts/cmpt-363-222-pages/main&homepage=week-01.md&toc-narrow=true&font-family=Lato%20Extended,Lato,Helvetica%20Neue,Helvetica,Arial,sans-serif&font-size=1&hide-credits=true
```

#### Example Docsify-This iFrame HMTL

![Docsify-This iFrame](images/docsify-this-iframe.png ':class=image-75-border')  
_Figure 5. Docsify-This iFrame (within the Canvas LMS Homepage), for example https://canvas.sfu.ca/courses/76289_

```html
<p><iframe style="overflow: hidden; border: 0px #ffffff none; margin-top: -26px; background: #ffffff;" src="https://docsify-this.net/?basePath=https://raw.githubusercontent.com/paulhibbitts/cmpt-363-222-pages/main&homepage=home.md&font-family=Lato%20Extended,Lato,Helvetica%20Neue,Helvetica,Arial,sans-serif&font-size=1&hide-credits=true" width="800px" height="950px" allowfullscreen="allowfullscreen"></iframe></p>
```

## Git and GitHub

### Git

Git is a free and open source distributed version control system,  originally created by Linus Torvalds in 2005 for development of the Linux kernel. 

#### Version Control

Version control supports the management of changes, called revisions, to files??? especially useful for pure text files.

![Local Version Control](images/local.png ':class=image-75')  
_Figure 6. Local Version Control (source: https://git-scm.com)_

#### Collaboration

As a distributed version control system, Git also support collaboration with multiple contributors.

![Distributed Version Control](images/distributed.png ':class=image-75-border')  
_Figure 7. Distributed Version Control (source: https://git-scm.com)_

### GitHub

GitHub is an online Git service, providing point-and-click means to create and manage Git repositories.

In addition to supporting the hosting of Git repositories, online editing of repository content such as Markdown files (using the filename extension .md) is also provided.

![GitHub Markdown File](images/github-markdown-file.png ':class=image-75-border')  
_Figure 8. GitHub Markdown File_

### GitHub Desktop
  
* Locally Store Git/GitHub Repositories  
* **Push** and **Pull** Repository Changes  

![GitHub Desktop](images/github-desktop-screenshot-mac.png ':class=image-75-border')  
_Figure 9. GitHub Desktop Mac (source: https://desktop.github.com)_

### Docsify-This + GitHub Markdown Files 

To fully leverage the benefits of version control, and potentially collaboration, store your Docsify-This Markdown pages within a GitHub repository and use GitHub Desktop to push/pull changes

![Docsify-This + GitHub Markdown Files](images/docsify-this-github.png ':class=image-75-border')  
_Figure 10. Docsify-This + GitHub Markdown Files Workflow_

## Additional Resources

* Markdown Format
  * [Markdown Guide](http://markdownguide.org)
  * [Markdown Cheatsheet](http://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
* Markdown Editors
  * [VSCode](https://code.visualstudio.com/)
  * [Pulsar Beta (was Atom.io)](https://pulsar-edit.dev/)
  * [Typora](https://typora.io/)
* GitHub Desktop
  * [GitHub Desktop App](https://desktop.github.com/)
  * [An Introduction to Version Control Using GitHub Desktop](http://programminghistorian.org/en/lessons/retired/getting-started-with-github-desktop)