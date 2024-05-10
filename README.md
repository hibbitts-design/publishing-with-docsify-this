<img src="images/pawel-czerwinski-EIfU0IUqZw8-unsplash.jpg" width="910" height="250" class="banner-image">

# Markdown Publishing with Docsify&#8288;&#8211;&#8288;This

An introduction to Markdown publishing using the open source [Docsify-This.net](https://docsify-this.net/) project.

## Markdown

### What is Markdown? 
[Markdown](https://en.wikipedia.org/wiki/Markdown) is a markup language used to format the display of content stored as plain text - similar but simpler than HTML&nbsp;formatting  

### Why use Markdown? 

* System-independent
* Text only format (perfect for version control)
* Separation of content vs. presentation
* Human-readable (i.e. more than HTML)
* Can also contain HTML snippets
* Large number of editor and publishing apps

### Markdown Examples

```
# Your H1 Text Here  
## Your H2 Text Here  

_your italic text here_  

**your bold text here**  

* your unordered list item here  

  1. your numbered (and indented) list item here   

[link title](https://www.google.com)  

![Image Alt Text](imagefile.jpg)  

Tip: To ensure a new paragraph after text in markdown, put two spaces after the end of the line

```

Looking for a more detailed overview of Markdown? Check out the [Markdown Cheat Sheet – How to Write in Markdown with Examples](https://www.freecodecamp.org/news/markdown-cheat-sheet/).

## Publishing with Markdown

* Markdown Converters
  * For example, [Pandoc](https://pandoc.org/)
* Markdown Static Site Builders
  * For example, [Jekyll](https://jekyllrb.com/)
* Markdown Dynamic Renderers
  * For example, [Docsify](https://docsify.js.org)

## Docsify-This

[Docsify-This](https://github.com/hibbitts-design/docsify-this) is an open source Web app, built using the [Docsify Open Publishing Kit](https://github.com/hibbitts-design/docsify-open-publishing-starter-kit), that can quickly display online Markdown files as web pages (i.e. no file uploads or build processes).   

_Being open source, you can also host your own Docsify-This instance, with the possibility of even a custom domain! No platform lock-in here._

### Example Docsify-This Usage Scenarios

* Publish your Markdown files as standalone web pages, with no website setup or build process required
* Visually style your standalone web pages using a point-and-click Web Page Builder
* Share existing GitHub-hosted Markdown files as standalone web pages, with an optional 'Edit this Page' link
* Seamlessly embed constraint-free Markdown/HTML into other platforms (e.g. LMS or CMS)
* Utilize the supported URL parameters when embedding content to match each destination platform better visually

### Docsify-This Web Page Builder

To use the Docsify-This **[Web Page Builder](https://docsify-this.net/)** enter the URL for an online Markdown file and tap the ‘Publish as Standalone Web Page’ button. The Markdown file will then be rendered as a standalone Web page with it’s own URL that can then be copied and shared.

<img src="images/docsify-this-web-page-builder.jpg" width="910" height="682" class="image-border" alt="Docsify-This Web Page Builder"><br>
<figcaption><em>Figure 1. Docsify-This Web Page Builder</em></figcaption>

### Example Docsify-This URL Created by the Web Page Builder

```html
https://docsify-this.net/?basePath=https://raw.githubusercontent.com/hibbitts-design/docsify-this-one-page-article/main&homepage=home.md
```

<img src="images/docsify-this-rendered-markdown-file.jpg" width="910" height="682" class="image-border" alt="Docsify-This Rendered Markdown File"><br>
<figcaption><em>Figure 2. Docsify-This Rendered Markdown File</em></figcaption>

Docsify-This rendered Web pages are also perfect for embedding, with the ability to visually style Docsify-This pages to the destination platform.

### Manual Docsify-This URL Editing

You can also render other Markdown files in the same repository by directly editing the Docsify-This URL parameter **homepage**, for example:

```html
https://docsify-this.net/?basePath=https://raw.githubusercontent.com/hibbitts-design/docsify-this-one-page-article/main&homepage=anotherfile.md
```

### Docsify-This Web Page Appearance

#### URL Parameters

The visual appearance of any Markdown file displayed by Docsify-This can be altered by using the provided set of [URL Parameters](https://docsify-this.net/#/?id=page-appearance-url-parameters). For example, **font-family**, **font-size**, **link-color** and **line-height**   

```
https://docsify-this.net/?basePath=https://raw.githubusercontent.com/hibbitts-design/docsify-this-one-page-article/main&homepage=home.md&font-family=Open%20Sans,sans-serif
```

#### Markdown CSS Classes

If you can edit the Markdown file that is displayed by Docsify-This the visual appearance can be further altered by using a set of provided [Markdown CSS Classes](https://docsify-this.net/#/?id=supported-markdown-css-classes). For example:  

**button**  

[Required Reading Quiz due Jun 4th](https://canvas.sfu.ca/courses/44038/quizzes/166553 ':class=button')

```markdown
[Required Reading Quiz due Jun 4th](https://canvas.sfu.ca/courses/44038/quizzes/166553 ':class=button')
```

**banner-image**  

<img src="images/12650723674_d5c85af332_k.jpg" width="910" height="250" class="banner-image" alt="UX - User Experience">

```markdown
![UX - User Experience](images/12650723674_d5c85af332_k.jpg ':class=banner-image')
```

#### Custom Markdown CSS Classes

<style>
.markdown-section .mybutton, .markdown-section .mybutton:hover {
  cursor: pointer;
  color: #CC0000;
  height: auto;
  display: inline-block;
  border: 2px solid #CC0000;
  border-radius: 4rem;
  margin: 2px 0px 2px 0px;
  padding: 8px 18px 8px 18px;
  line-height: 1.2rem;
  background-color: white;
  font-family: -apple-system, "Segoe UI", "Helvetica Neue", sans-serif;
  font-weight: bold;
  text-decoration: none;
}
</style>

In addition to the Markdown CSS classes supported by Docsify-This, you can also define your own custom classes within your displayed Markdown files, for example:

[Custom CSS Class Button](# ':class=mybutton')

CSS in Markdown file:  
```css
<style>
.markdown-section .mybutton, .markdown-section .mybutton:hover {
  cursor: pointer;
  color: #CC0000;
  height: auto;
  display: inline-block;
  border: 2px solid #CC0000;
  border-radius: 4rem;
  margin: 2px 0px 2px 0px;
  padding: 8px 18px 8px 18px;
  line-height: 1.2rem;
  background-color: white;
  font-family: -apple-system, "Segoe UI", "Helvetica Neue", sans-serif;
  font-weight: bold;
  text-decoration: none;
}
</style>
```

Markdown:  
```markdown
[Required Reading Quiz due Jun 4th](https://canvas.sfu.ca/courses/44038/quizzes/168353 ':class=mybutton')
```

#### HTML Snippets

As supported by standard Markdown, HTML snippets can also be included (and mixed) within Markdown , for example:  

```html
<div class="row">
<div class="column">

Lorem ipsum dolor sit amet, consectetur adipiscing elit.

</div>
<div class="column">

Lorem ipsum dolor sit amet, consectetur adipiscing elit.

</div>
</div>
```

### Docsify-This Page Markdown Templates

The following example Markdown templates are available which can be cloned/forked on GitHub or imported into Codeberg. Templates can also be downloaded and hosted just about anywhere online. 

To use these templates you would generally do the following (specific instructions are included with each template):

1. Tap **Use this template** in the chosen template repository (upper-right green button) and then choose **Create a new repository**

2. Choose the name for your new repository to contain the files and then tap **Create repository** to copy the template files to your own GitHub account

3. View the **home.md** Markdown file in your newly created repository and copy it's URL

4. Go to https://docsify-this.net and paste the copied URL into the **Markdown File URL** field

5. Select the page options you want (e.g. Docsify Sidebar) and tap the **View as Standalone Page** button to view your Markdown file as a web page for sharing or embedding  

Now that the template files are located on your own GitHub account, modify their content to fit your needs.  

<h4><a href="https://github.com/hibbitts-design/docsify-this-one-page-article">Docsify-This One Page Article Templates</a></h4>

<img src="images/docsify-this-one-page-article.jpg" width="910" height="682" class="image-border" alt="Docsify-This One Page Article Template"><br>
<figcaption><em>Figure 3. Docsify-This One Page Article Template, for example the Markdown file <a href="https://github.com/hibbitts-design/docsify-this-one-page-article/blob/main/home.md">home.md</a> and displayed by Docsify-This as <a href="https://docsify-this.net/?basePath=https://raw.githubusercontent.com/hibbitts-design/docsify-this-one-page-article/main&homepage=home.md&sidebar=true&maxLevel=3">https://docsify-this.net/?basePath=https://raw.githubusercontent.com/hibbitts-design/docsify-this-one-page-article/main&homepage=home.md&sidebar=true&maxLevel=3</a></em></figcaption>

<h4><a href="https://github.com/hibbitts-design/docsify-this-one-page-course">Docsify-This One Page Course Template</a></h4>

<img src="images/docsify-this-one-page-course.jpg" width="910" height="682" class="image-border" alt="Docsify-This One Page Course Template"><br>
<figcaption><em>Figure 4. Docsify-This One Page Course Template, for example the Markdown file <a href="https://github.com/hibbitts-design/docsify-this-one-page-course/blob/main/home.md">home.md</a> and displayed by Docsify-This as <a href="https://docsify-this.net/?basePath=https://raw.githubusercontent.com/hibbitts-design/docsify-this-one-page-course/main&homepage=home.md&toc=true">https://docsify-this.net/?basePath=https://raw.githubusercontent.com/hibbitts-design/docsify-this-one-page-course/main&homepage=home.md&toc=true</a></em></figcaption>

<h4><a href="https://github.com/hibbitts-design/docsify-this-multiple-page-site">Docsify-This Multiple Page Site Template</a></h4>

<img src="images/docsify-this-multiple-page-site.jpg" width="910" height="682" class="image-border" alt="Docsify-This Multiple Page Site"><br>
<figcaption><em>Figure 5. Docsify-This Multiple Page Site, for example the Markdown file <a href="https://github.com/hibbitts-design/docsify-this-multiple-page-site/blob/main/home.md">home.md</a> and displayed by Docsify-This as <a href="https://docsify-this.net/?basePath=https://raw.githubusercontent.com/hibbitts-design/docsify-this-multiple-page-site/main&homepage=home.md">https://docsify-this.net/?basePath=https://raw.githubusercontent.com/hibbitts-design/docsify-this-multiple-page-site/main&homepage=home.md</a></em></figcaption>

<h4><a href="https://github.com/hibbitts-design/docsify-this-multiple-page-course-site">Docsify-This Multiple Page Course Site Template</a></h4>

<img src="images/docsify-this-multiple-page-course-site.jpg" width="910" height="682" class="image-border" alt="Docsify-This Multiple Page Course Site Template"><br>
<figcaption><em>Figure 6. Docsify-This Multiple Page Site, for example the Markdown file <a href="https://github.com/hibbitts-design/docsify-this-multiple-page-site/blob/main/home.md">home.md</a>, including the use of a custom Docsify a href="https://github.com/hibbitts-design/docsify-this-multiple-page-course-site/blob/main/_sidebar.md">Sidebar</a> file, and displayed by Docsify-This as <a href="https://docsify-this.net/?basePath=https://raw.githubusercontent.com/hibbitts-design/docsify-this-multiple-page-course-site/main&homepage=home.md&sidebar=true&loadSidebar=_sidebar.md&loadNavbar=_navbar.md&hide-credits=true&browser-tab-title=CPT-363">https://docsify-this.net/?basePath=https://raw.githubusercontent.com/hibbitts-design/docsify-this-multiple-page-course-site/main&homepage=home.md&sidebar=true&loadSidebar=_sidebar.md&loadNavbar=_navbar.md&hide-credits=true&browser-tab-title=CPT-363</a></em></figcaption>

<h4><a href="https://github.com/hibbitts-design/docsify-this-lms-content-pages">Docsify-This LMS Content Pages Template</a></h4>

<img src="images/docsify-this-lms-content-pages.jpg" width="910" height="682" class="image-border" alt="Docsify-This LMS Content Pages Template"><br>
<figcaption><em>Figure 7. Docsify-This LMS Content Pages Template, including such embeddable pages as a <a href="https://docsify-this.net/?basePath=https://raw.githubusercontent.com/hibbitts-design/docsify-this-lms-content-pages/main&homepage=home.md&edit-link=https://github.com/hibbitts-design/docsify-this-lms-content-pages/blob/main/home.md">home page</a>, <a href="https://docsify-this.net/?basePath=https://raw.githubusercontent.com/hibbitts-design/docsify-this-lms-content-pages/main&homepage=module-01.md&edit-link=https://github.com/hibbitts-design/docsify-this-lms-content-pages/blob/main/module-01.md">weekly module</a>, <a href="https://docsify-this.net/?basePath=https://raw.githubusercontent.com/hibbitts-design/docsify-this-lms-content-pages/main&homepage=topics.md&edit-link=https://github.com/hibbitts-design/docsify-this-lms-content-pages/blob/main/topics.md">topics</a> and <a href="https://docsify-this.net/?basePath=https://raw.githubusercontent.com/hibbitts-design/docsify-this-lms-content-pages/main&homepage=index.md">more</a></em></figcaption>

### Embedding Docsify-This Pages

#### iFrames

You can embed Docsify-This web pages using iFrames in almost any platform. URL parameters can also be used to match each destination platform better visually.

<img src="images/docsify-this-iframe.jpg" width="910" height="682" class="image-border" alt="Docsify-This iFrame"><br>
<figcaption><em>Figure 8. Docsify-This iFrame (within the Canvas LMS Homepage), for example <a href="https://canvas.sfu.ca/courses/76289">https://canvas.sfu.ca/courses/76289</a></em></figcaption>

```html
<p><iframe style="overflow: hidden; border: 0px #ffffff none; margin-top: -26px; background: #ffffff;" src="https://docsify-this.net/?basePath=https://raw.githubusercontent.com/paulhibbitts/cmpt-363-222-pages/main&homepage=home.md&font-family=Lato%20Extended,Lato,Helvetica%20Neue,Helvetica,Arial,sans-serif&font-size=1&hide-credits=true" width="800px" height="950px" allowfullscreen="allowfullscreen"></iframe></p>
```

As shown above, with the Canvas LMS a Canvas Page can be set as the course Homepage, and then an iFrame can be used for the content of that page. For more details, view [How do I set a Front Page in a course?](https://community.canvaslms.com/t5/Instructor-Guide/How-do-I-set-a-Front-Page-in-a-course/ta-p/797) and [Embed content in Canvas](https://www.howtocanvas.com/create-amazing-pages-in-canvas/embedding-content).

If a scroll bar is present, you may want to re-edit your iFrame code and adjust the "height" value.  

#### External URL

The URL of a Markdown file rendered by Docsify-This can also be included inside of other systems as an external URL.  

Many LMSs, including Canvas and Moodle, have the ability to include external URLs in their course navigation menus. For example, with the Canvas LMS you would use the [Redirect Tool](https://help.canvas.yale.edu/m/55452/l/914676-creating-a-custom-link-in-your-course-navigation-using-the-redirect-tool) to display Docsify-This web pages.

<img src="images/docsify-this-page.jpg" width="910" height="682" class="image-border" alt="Docsify-This Module"><br>
<figcaption><em>Figure 9. Docsify-This External URL within Canvas LMS (used with the Redirect Tool), for example <a href="https://canvas.sfu.ca/courses/76289/external_tools/36154">https://canvas.sfu.ca/courses/76289/external_tools/36154</a></em></figcaption>

```html
url=https://docsify-this.net/?basePath=https://raw.githubusercontent.com/paulhibbitts/cmpt-363-222-pages/main&homepage=resources.md&edit-link=https://github.com/paulhibbitts/cmpt-363-222-pages/blob/main/resources.md&font-family=Lato%20Extended,Lato,Helvetica%20Neue,Helvetica,Arial,sans-serif&font-size=1&hide-credits=true
```

With the Canvas LMS it is also possible to use an [external web page as content within a course Module](https://community.canvaslms.com/t5/Instructor-Guide/How-do-I-add-an-external-URL-as-a-module-item/ta-p/967).

<img src="images/docsify-this-module.jpg" width="910" height="682" class="image-border" alt="Docsify-This Canvas LMS Module"><br>
<figcaption><em>Figure 10. Docsify-This External URL with Page Table of Contents (used as a Canvas LMS Module), for example <a href="https://canvas.sfu.ca/courses/76289/modules/items/2816273">https://canvas.sfu.ca/courses/76289/modules/items/2816273</a></em></figcaption>

```html
https://docsify-this.net?basePath=https://raw.githubusercontent.com/paulhibbitts/cmpt-363-222-pages/main&homepage=week-01.md&toc-narrow=true&font-family=Lato%20Extended,Lato,Helvetica%20Neue,Helvetica,Arial,sans-serif&font-size=1&hide-credits=true
```

## Hosting Markdown Files
There are multiple ways to get a raw Markdown file available online, here are three options to help you get started:

### GitHub or Codeberg 
1. Signup for a [GitHub](https://github.com) or [Codeberg](https://codeberg.org) account
2. Create a new repository and upload your Markdown file
3. View the uploaded file, and copy/paste that URL into the Docsify-This **Markdown File URL** field

### Gist (GitHub Gists)
1. Signup for a [GitHub](https://github.com) account
1. Create a gist with your Markdown file at https://gist.github.com
2. Enter a filename ending with `.md` (e.g. `myfile.md`)
3. Choose **Create public gist** and tap on that button
4. Tap on **Raw** button in the upper right of your Gist field and copy/paste that URL into the Docsify-This **Markdown File URL** field

### Personal or Organizational Website
1. Obtain login information for your server
2. Upload the Markdown file to your server
3. Navigate to the location of that file, view the contents in your Browser, and copy/paste that URL into the Docsify-This **Markdown File URL** field

## Leveraging Git and GitHub

### Git

Git is a free and open source distributed version control system,  originally created by Linus Torvalds in 2005 for development of the Linux kernel. 

#### Version Control

Version control supports the management of changes, called revisions, to files... especially useful for pure text files such as those used by Docsify-This.

<img src="images/local.png" alt="Local Version Control" class="image-75">
<figcaption><em>Figure 11. Local Version Control (source: <a href="https://git-scm.com">https://git-scm.com</a>)</em></figcaption>

#### Collaboration

As a distributed version control system, Git also support collaboration with multiple contributors.

<img src="images/distributed.png" alt="Local Version Control" class="image-75">
<figcaption><em>Figure 12. Distributed Version Control (source: <a href="https://git-scm.com">https://git-scm.com</a>)</em></figcaption>

### GitHub

GitHub and Codeberg are examples of online Git services, providing point-and-click means to create and manage Git repositories.

In addition to supporting the hosting of Git repositories, online editing of repository content such as Markdown files (using the filename extension .md) is also provided.

<img src="images/github-markdown-file.jpg" alt="Local Version Control" class="image-75-border">
<figcaption><em>Figure 13. GitHub Markdown File</em></figcaption>

### GitHub Desktop
  
* Locally Store Git/GitHub Repositories  
* **Push** and **Pull** Repository Changes  

<img src="images/github-desktop-screenshot-mac.jpg" alt="GitHub Desktop" class="image-75-border">
<figcaption><em>Figure 14. GitHub Desktop Mac (source: <a href="https://git-scm.com">https://git-scm.com</a>)</em></figcaption>

### Docsify-This + GitHub or Codeberg Markdown Files 

To fully leverage the benefits of version control, and potentially collaboration using an optional "Edit this Page" link, store your Docsify-This Markdown pages within a GitHub or Codeberg repository and optionally use an app such as GitHub Desktop to push/pull changes to your desktop.

### Setting up GitHub Desktop

1. Install GitHub Desktop (https://desktop.github.com)
1. Enter your GitHub credentials as prompted
1. Go to a GitHub repository web page, tap **< > Code** and then choose **Open with GitHub Desktop** OR go to a Codeberg repository web page, copy the HTTPS address, then in GitHub Desktop choose **File > Clone Repository** and paste the copied URL
1. Choose the location for your cloned repository and tap the **Clone** button

### Desktop Text Editors

Once your Docsify-This Markdown files are synced (i.e. cloned) to your desktop via GitHub Desktop you can then use the text editor of your choice, such as VSCode, Pulsar Beta (was Atom.io), Typora etc.

Using GitHub Desktop you can preview any changes and then commit those changes back to the repository. VSCode can also be used alone to both sync and editing files.

<img src="images/docsify-this-github.jpg" alt="Docsify-This + GitHub Markdown Files" class="image-75-border">
<figcaption><em>Figure 15. Docsify-This + GitHub Markdown Files Workflow</em></figcaption>

<img src="images/docsify-this-webserver.jpg" alt="Docsify-This + Webserver Markdown Files" class="image-75-border">
<figcaption><em>Figure 16. Docsify-This + Webserver Markdown Files</em></figcaption>

## Additional Resources

* Markdown Format
  * [What Is Markdown, and How Do You Use It?](https://www.howtogeek.com/448323/what-is-markdown-and-how-do-you-use-it/)
  * [Markdown Guide](http://markdownguide.org)
  * [Markdown Cheatsheet](http://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
* Accessibility
  * [Improving The Accessibility Of Your Markdown](https://www.smashingmagazine.com/2021/09/improving-accessibility-of-markdown/)
* Creating and Editing Markdown on GitHub
  * [Quickstart for writing on GitHub](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/quickstart-for-writing-on-github)
  * [Authoring With Markdown](https://ucsbcarpentry.github.io/2022-01-31-ucsb-webpub-online/02-markdown/)
* GitHub and Open Education Resources (OER)
  * [Create and publish OER with GitHub](https://liascript.github.io/course/?https://raw.githubusercontent.com/TIBHannover/oer-github-tutorial/main/tutorial.md#1)
  * [OER on GitHub What, Why, & How](https://evanwill.github.io/make-oer)
* GitHub Desktop
  * [GitHub Desktop App](https://desktop.github.com/)
  * [An Introduction to Version Control Using GitHub Desktop](http://programminghistorian.org/en/lessons/retired/getting-started-with-github-desktop)
  * [Getting Started with Git and GitHub Desktop](https://www.codecademy.com/article/what-is-git-and-github-desktop)
* Markdown Desktop Editors
  * [VSCode](https://code.visualstudio.com/)
  * [Pulsar (was Atom.io)](https://pulsar-edit.dev/)
  * [Typora](https://typora.io/)
