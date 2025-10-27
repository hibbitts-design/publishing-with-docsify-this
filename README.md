# Markdown Publishing with Docsify-This

A detailed guide to Markdown publishing using the open source [Docsify-This.net](https://docsify-this.net/) project.

## Markdown

Before diving into publishing with Docsify-This, let's cover the basics of Markdown - the simple formatting (markup) language that makes all of this possible. Understanding these fundamentals will help you create better content and take full advantage of Docsify-This.

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

## Hosting Markdown Files

To use Docsify-This, your Markdown files need to be available online with a web link. While this might sound a bit technical, there are several straightforward ways that require no server management or technical expertise. Here are three popular approaches:

### GitHub or Codeberg 

#### Step 1: Create a New Repository

1. **Log in** or **Sign up** to GitHub or Codeberg
2. **Create a new repository**:
   - Tap the **+** icon and select **New Repository**
   - Fill in the repository details:
     - Choose a **Repository Name** for your repository (e.g., `docsify-this-demo`)
     - Confirm that the **Visibility** is **Public**
   - Tap **Create Repository**

#### Step 2: Add Your Markdown Content

**Option A: Create a New Markdown File**

1. **Go to your new repository**, tap **Add File** and then choose **New File**
2. **Name your file** and use the `.md` extension (e.g., `demo.md`)
3. Enter your **Markdown content**. For example:
   ```markdown
   # Welcome!
   
   This is my sample Markdown file.
   ```

**Option B: Upload an Existing File**

1. **Go to your new repository**, tap **Add File** and then choose **Upload File**
2. **Choose your file** and make sure it uses the `.md` extension (e.g., `demo.md`)

#### Step 3: Commit the Changes

1. **Commit your file**:
   - Provide a **Commit Message** (e.g., "Create demo.md")
   - Tap the **Commit Changes** button

#### Step 4: Verify the File and View it with Docsify-This

1. In your repository, **view the file** to see the rendered Markdown
2. **Copy the file URL** from your Browser's address bar
3. **Go to [Docsify-This.net](https://docsify-this.net)** and paste the copied URL into the **Markdown File URL** field
4. Tap the **Publish as a Web Page** button to view your Markdown file rendered as a web page using Docsify-This

### Gist (GitHub Gists)
1. Signup for a [GitHub](https://github.com) account
2. Create a gist with your Markdown file at https://gist.github.com
3. Enter a filename ending with `.md` (e.g. `mygist.md`)
4. Choose **Create public gist** and tap on that button
5. Tap on **Raw** button in the upper right of your Gist field and copy/paste that URL into the Docsify-This **Markdown File URL** field

### Personal or Organizational Website
1. Obtain login information for your Webserver
2. Upload the Markdown file to your Webserver with a filename ending with `.md` (e.g. `myfile.md`)
3. Navigate to the location of that file, view the contents in your Browser, and copy/paste that URL into the Docsify-This **Markdown File URL** field

## Publishing with Docsify-This

Now that you have Markdown files hosted online, you're ready to transform them into visually styled web pages. Docsify-This makes this process remarkably simple while offering a range of customization options to match your needs.

_As an open source project, you even have the option to host your own Docsify-This instance with your own custom domain, giving you full control over your publishing platform with minimal configuration required._

### Getting Started

To use the Docsify-This **[Web Page Builder](https://docsify-this.net/)** enter the URL for an online Markdown file and tap the 'Publish as a Web Page' button. You can use either a regular GitHub or Codeberg file URL (e.g. https://github.com/username/repo/blob/main/README.md) or a raw URL (e.g. https://raw.githubusercontent.com/username/repo/main/README.md) - both are fully supported. The Markdown file will then be rendered as a web page with its own URL that can be copied and shared.

<img src="https://raw.githubusercontent.com/paulhibbitts/github-repo-images/refs/heads/master/docsify-this-v1-10-6-web-page-builder.png" width="910" height="682" class="responsive" alt="Docsify-This Web Page Builder"><br>

<em>Figure 1. Docsify-This Web Page Builder</em>

**Important:** If you're manually constructing a Docsify-This URL (bypassing the Web Page Builder), you must use the raw source URL for GitHub files. You can obtain the raw URL by clicking the "Raw" button when viewing the file on GitHub, or by changing the URL format from:
- `https://github.com/username/repo/blob/main/README.md` 
to:
- `https://raw.githubusercontent.com/username/repo/main/README.md`

However, when using the Web Page Builder, you can paste either the regular GitHub URL or the raw URL - both formats are supported.

### Example Docsify-This URL Created by Web Page Builder

```html
https://docsify-this.net/?basePath=https://raw.githubusercontent.com/hibbitts-design/docsify-this-one-page-article/main&homepage=home.md
```

<img src="https://raw.githubusercontent.com/hibbitts-design/publishing-with-docsify-this/main/images/docsify-this-rendered-markdown-file.jpg" width="910" height="682" class="responsive image-border" alt="Docsify-This Rendered Markdown File"><br>
<em>Figure 2. Docsify-This Rendered Markdown File</em>

Docsify-This rendered Web pages are also perfect for embedding, with the ability to visually style Docsify-This pages to the destination platform.

### Basic Customization

The visual appearance of any Markdown file displayed by Docsify-This can be altered with the Web Page Builder or using the provided set of [URL Parameters](https://docsify-this.net/#/?id=page-appearance-url-parameters-basic).

For example, you can change font family with the Web Page Builder or by using the **font-family** URL parameter:

```
https://docsify-this.net/?basePath=https://raw.githubusercontent.com/hibbitts-design/docsify-this-one-page-article/main&homepage=home.md&font-family=Open%20Sans,sans-serif
```

You can also add a collapsible sidebar with the Web Page Builder or by using the **sidebar** URL parameter:
```
https://docsify-this.net/?basePath=https://raw.githubusercontent.com/hibbitts-design/docsify-this-one-page-article/main&homepage=home.md&sidebar=true
```

Please note that when you use the Docsify-This Web Page Builder the Docsify-This URL generated includes these same URL parameters. For example, selecting a custom font family like "Open Sans" will add the parameter `font-family=Open%20Sans,sans-serif` to your generated URL. Similarly, options like adding a sidebar for navigation or adding an "Edit this Page" link are all translated into URL parameters that can be bookmarked and shared.

For a complete list of available URL parameters and advanced customization options, see the [Docsify-This URL parameter documentation](https://docsify-this.net/#/?id=page-appearance-url-parameters-basic).

### Editing a Docsify-This URL

You can also render other Markdown files in the same repository by manualy editing the Docsify-This URL parameter **homepage**, for example:

```html
https://docsify-this.net/?basePath=https://raw.githubusercontent.com/hibbitts-design/docsify-this-one-page-article/main&homepage=anotherfile.md
```

### Example Usage Scenarios

* Publish your Markdown files as web pages, with no website setup or build process required
* Visually style your web pages using a point-and-click Web Page Builder
* Share existing GitHub-hosted Markdown files as web pages, with an optional 'Edit this Page' link
* Seamlessly embed constraint-free Markdown/HTML into other platforms (e.g. LMS or CMS)
* Use the available options when embedding content to match each destination platform better visually

### Markdown CSS Classes

If you can edit the Markdown file that is displayed by Docsify-This the visual appearance can be further altered by using a set of provided [Markdown CSS Classes](https://docsify-this.net/#/?id=supported-markdown-css-classes). For example:  

**button**  

[Required Reading Quiz due Jun 4th](https://canvas.sfu.ca/courses/44038/quizzes/166553 ':class=button')

```markdown
[Required Reading Quiz due Jun 4th](https://canvas.sfu.ca/courses/44038/quizzes/166553 ':class=button')
```

**banner-image**  

<img src="https://raw.githubusercontent.com/hibbitts-design/publishing-with-docsify-this/main/images/12650723674_d5c85af332_k.jpg" width="910" height="250" class="banner-image" alt="UX - User Experience">

```markdown
![UX - User Experience](https://raw.githubusercontent.com/hibbitts-design/publishing-with-docsify-this/main/images/12650723674_d5c85af332_k.jpg ':class=banner-image')
```

For a complete reference of all available CSS classes and advanced styling options, see the [Docsify-This CSS Markdown classes documentation](https://docsify-this.net/#/?id=supported-markdown-css-classes).

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

### Ready-to-Use Templates

Starting from scratch isn't always necessary. These pre-designed templates provide a solid foundation for common publishing scenarios, from simple articles to complete course websites. You can use them as-is or change them to fit what you need.

The following Markdown templates can be cloned/forked on GitHub, imported into Codeberg, or downloaded and hosted on your own webserver.

To use these templates you would generally do the following (specific instructions are included with each template):

1. Tap **Use this template** in the chosen template repository (upper-right green button) and then choose **Create a new repository**
2. Choose the name for your new repository to contain the files and then tap **Create repository** to copy the template files to your own GitHub account
3. View the **home.md** Markdown file in your newly created repository and copy it's URL
4. Go to https://docsify-this.net and paste the copied URL into the **Markdown File URL** field
5. Select the page options you want (e.g. Docsify Sidebar) and tap the **View as a Web Page** button to view your Markdown file as a web page for sharing or embedding  

Now that the template files are located on your own GitHub account, modify their content to fit your needs.  

<h4><a href="https://github.com/hibbitts-design/docsify-this-one-page-article">Docsify-This One Page Article Template</a></h4> 

<img src="https://raw.githubusercontent.com/hibbitts-design/publishing-with-docsify-this/main/images/docsify-this-one-page-article.jpg" width="910" height="682" class="responsive image-border" alt="Docsify-This One Page Article Template"><br>
<em>Figure 3. Docsify-This One Page Article Template, for example the Markdown file <a href="https://github.com/hibbitts-design/docsify-this-one-page-article/blob/main/home.md">home.md</a> and displayed by Docsify-This as <a href="https://docsify-this.net/?basePath=https://raw.githubusercontent.com/hibbitts-design/docsify-this-one-page-article/main&homepage=home.md&sidebar=true&maxLevel=3">https://docsify-this.net/?basePath=https://raw.githubusercontent.com/hibbitts-design/docsify-this-one-page-article/main&homepage=home.md&sidebar=true&maxLevel=3</a></em>

<h4><a href="https://github.com/hibbitts-design/docsify-this-one-page-course">Docsify-This One Page Course Template</a></h4>

<img src="https://raw.githubusercontent.com/hibbitts-design/publishing-with-docsify-this/main/images/docsify-this-one-page-course.jpg" width="910" height="682" class="responsive image-border" alt="Docsify-This One Page Course Template"><br>
<em>Figure 4. Docsify-This One Page Course Template, for example the Markdown file <a href="https://github.com/hibbitts-design/docsify-this-one-page-course/blob/main/home.md">home.md</a> and displayed by Docsify-This as <a href="https://docsify-this.net/?basePath=https://raw.githubusercontent.com/hibbitts-design/docsify-this-one-page-course/main&homepage=home.md&toc=true">https://docsify-this.net/?basePath=https://raw.githubusercontent.com/hibbitts-design/docsify-this-one-page-course/main&homepage=home.md&toc=true</a></em>

<h4><a href="https://github.com/hibbitts-design/docsify-this-multiple-page-site">Docsify-This Multiple Page Basic Site Template</a></h4>

<img src="https://raw.githubusercontent.com/hibbitts-design/publishing-with-docsify-this/main/images/docsify-this-multiple-page-basic-site.jpg" width="910" height="682" class="responsive image-border" alt="Docsify-This Multiple Page Basic Site"><br>
<em>Figure 5. Docsify-This Multiple Page Basic Site, for example the Markdown file <a href="https://github.com/hibbitts-design/docsify-this-multiple-page-site/blob/main/home.md">home.md</a> and displayed by Docsify-This as <a href="https://docsify-this.net/?basePath=https://raw.githubusercontent.com/hibbitts-design/docsify-this-multiple-page-site/main&homepage=home.md">https://docsify-this.net/?basePath=https://raw.githubusercontent.com/hibbitts-design/docsify-this-multiple-page-site/main&homepage=home.md</a></em>

<h4><a href="https://github.com/hibbitts-design/docsify-this-multiple-page-blog-style-site">Multiple Page Blog Style Site Template</a></h4>

<img src="https://raw.githubusercontent.com/hibbitts-design/publishing-with-docsify-this/main/images/docsify-this-multiple-page-blog-style-site.jpg" width="910" height="682" class="responsive image-border" alt="Docsify-This Multiple Page Blog Style Template"><br>
<em>Figure 6. Docsify-This Multiple Page Blog Style Site Template, for example the Markdown file <a href="https://github.com/hibbitts-design/docsify-this-multiple-page-blog-style-site/blob/main/home.md">home.md</a> and displayed by Docsify-This as <a href="https://docsify-this.net?basePath=https://raw.githubusercontent.com/hibbitts-design/docsify-this-multiple-page-blog-style-site/main&homepage=home.md">https://docsify-this.net?basePath=https://raw.githubusercontent.com/hibbitts-design/docsify-this-multiple-page-blog-style-site/main&homepage=home.md</a></em>

<h4><a href="https://github.com/hibbitts-design/docsify-this-multiple-page-open-publishing-site">Multiple Page Open Publishing Site Template</a></h4>

<img src="https://raw.githubusercontent.com/hibbitts-design/publishing-with-docsify-this/main/images/docsify-this-multiple-page-open-publishing-site.jpg" width="910" height="682" class="responsive image-border" alt="Docsify-This Multiple Page Open Publishing Site Template"><br>
<em>Figure 7. Multiple Page Open Publishing Site <a href="https://github.com/hibbitts-design/docsify-this-multiple-page-open-publishing-site/blob/main/home.md">home.md</a> file, including the use of a Docsify custom <a href="https://github.com/hibbitts-design/docsify-this-multiple-page-open-publishing-site/blob/main/_sidebar.md">Sidebar</a> file, displayed by Docsify-This as <a href="https://docsify-this.net?basePath=https://raw.githubusercontent.com/hibbitts-design/docsify-this-multiple-page-open-publishing-site/main&homepage=home.md&sidebar=true&loadSidebar=_sidebar.md&hide-credits=true">https://docsify-this.net?basePath=https://raw.githubusercontent.com/hibbitts-design/docsify-this-multiple-page-open-publishing-site/main&homepage=home.md&sidebar=true&loadSidebar=_sidebar.md&hide-credits=true</a></em>

<h4><a href="https://github.com/hibbitts-design/docsify-this-multiple-page-course-site">Docsify-This Multiple Page Course Site Template</a></h4>

<img src="https://raw.githubusercontent.com/hibbitts-design/publishing-with-docsify-this/main/images/docsify-this-multiple-page-course-site.jpg" width="910" height="682" class="responsive image-border" alt="Docsify-This Multiple Page Course Site Template"><br>
<em>Figure 8. Docsify-This Multiple Page Site, for example the Markdown file <a href="https://github.com/hibbitts-design/docsify-this-multiple-page-site/blob/main/home.md">home.md</a>, including the use of a custom Docsify <a href="https://github.com/hibbitts-design/docsify-this-multiple-page-course-site/blob/main/_sidebar.md">Sidebar</a> file, and displayed by Docsify-This as <a href="https://docsify-this.net/?basePath=https://raw.githubusercontent.com/hibbitts-design/docsify-this-multiple-page-course-site/main&homepage=home.md&sidebar=true&loadSidebar=_sidebar.md&loadNavbar=_navbar.md&hide-credits=true&browser-tab-title=CPT-363">https://docsify-this.net/?basePath=https://raw.githubusercontent.com/hibbitts-design/docsify-this-multiple-page-course-site/main&homepage=home.md&sidebar=true&loadSidebar=_sidebar.md&loadNavbar=_navbar.md&hide-credits=true&browser-tab-title=CPT-363</a></em>

<h4><a href="https://github.com/hibbitts-design/docsify-this-lms-content-pages">Docsify-This LMS Content Pages Template</a></h4>

<img src="https://raw.githubusercontent.com/hibbitts-design/publishing-with-docsify-this/main/images/docsify-this-lms-content-pages.jpg" width="910" height="682" class="responsive image-border" alt="Docsify-This LMS Content Pages Template"><br>
<em>Figure 9. Docsify-This LMS Content Pages Template, including such embeddable pages as a <a href="https://docsify-this.net/?basePath=https://raw.githubusercontent.com/hibbitts-design/docsify-this-lms-content-pages/main&homepage=home.md&edit-link=https://github.com/hibbitts-design/docsify-this-lms-content-pages/blob/main/home.md">home page</a>, <a href="https://docsify-this.net/?basePath=https://raw.githubusercontent.com/hibbitts-design/docsify-this-lms-content-pages/main&homepage=module-01.md&edit-link=https://github.com/hibbitts-design/docsify-this-lms-content-pages/blob/main/module-01.md">weekly module</a>, <a href="https://docsify-this.net/?basePath=https://raw.githubusercontent.com/hibbitts-design/docsify-this-lms-content-pages/main&homepage=topics.md&edit-link=https://github.com/hibbitts-design/docsify-this-lms-content-pages/blob/main/topics.md">topics</a> and <a href="https://docsify-this.net/?basePath=https://raw.githubusercontent.com/hibbitts-design/docsify-this-lms-content-pages/main&homepage=index.md">more</a></em>

For additional template examples, see the [Docsify-This Markdown templates](https://docsify-this.net/#/?id=ready-to-use-docsify-this-markdown-templates)

### Embedding Docsify-This Pages

#### iFrames

In additition to generating web pages and sites, you can embed Docsify-This web pages using iFrames in almost any platform. URL parameters can also be used to match each destination platform better visually.

_In general, paste the below HTML into your HTML editor and then replace the default `basepath` and `homepage` value with your own. For WordPress users: Add the code below to a Custom HTML block._

For basic embedding with a fixed height to blend in smoothly with your other page content:

```html
<div style="width: 100%; margin: 0; padding: 0; overflow: hidden;">
  <iframe src="https://docsify-this.net/?basePath=https://raw.githubusercontent.com/paulhibbitts/github-demo-markdown-file/main&homepage=README.md&max-width=100&hide-credits=true" 
    style="width: 100%; height: 2700px; border: none; display: block;"
    scrolling="no"
    frameborder="0">
  </iframe>
</div>
```

_Adjust the `height` value (2700px) to match your content length. Test on different devices to ensure all content is visible._

<img src="https://raw.githubusercontent.com/hibbitts-design/publishing-with-docsify-this/main/images/docsify-this-iframe.jpg" width="910" height="682" class="responsive image-border" alt="Docsify-This iFrame"><br>
<em>Figure 10. Docsify-This iFrame (within the Canvas LMS Homepage), for example <a href="https://canvas.sfu.ca/courses/76289">https://canvas.sfu.ca/courses/76289</a></em>

```html
<p>
  <iframe style="overflow: hidden; border: 0px #ffffff none; background: #ffffff;"
    src="https://docsify-this.net?basePath=https://raw.githubusercontent.com/paulhibbitts/cmpt-363-222-pages/main&homepage=home.md&font-family=Lato%20Extended,Lato,Helvetica%20Neue,Helvetica,Arial,sans-serif&font-size=16px&hide-credits=true"
      width="800px"
      height="1400px"
      allowfullscreen="allowfullscreen">
  </iframe>
</p>
```

As shown above, with the Canvas LMS a Canvas Page can be set as the course Homepage, and then an iFrame can be used for the content of that page. For more details, view [How do I set a Front Page in a course?](https://community.canvaslms.com/t5/Instructor-Guide/How-do-I-set-a-Front-Page-in-a-course/ta-p/797) and [Embed content in Canvas](https://www.howtocanvas.com/create-amazing-pages-in-canvas/embedding-content).

If a scroll bar is present, you may want to re-edit your iFrame code and adjust the "height" value.  

#### External URL

The URL of a Markdown file rendered by Docsify-This can also be included inside of other systems as an external URL.  

Many LMSs, including Canvas and Moodle, have the ability to include external URLs in their course navigation menus. For example, with the Canvas LMS you would use the [Redirect Tool](https://help.canvas.yale.edu/m/55452/l/914676-creating-a-custom-link-in-your-course-navigation-using-the-redirect-tool) to display Docsify-This web pages.

<img src="https://raw.githubusercontent.com/hibbitts-design/publishing-with-docsify-this/main/images/docsify-this-page.jpg" width="910" height="682" class="responsive image-border" alt="Docsify-This Module"><br>
<em>Figure 11. Docsify-This External URL within Canvas LMS (used with the Redirect Tool), for example <a href="https://canvas.sfu.ca/courses/76289/external_tools/36154">https://canvas.sfu.ca/courses/76289/external_tools/36154</a></em>

```html
url=https://docsify-this.net/?basePath=https://raw.githubusercontent.com/hibbitts-design/cmpt-363-222-pages/main&homepage=resources.md&edit-link=https://github.com/hibbitts-design/cmpt-363-222-pages/blob/main/resources.md&font-family=Lato%20Extended,Lato,Helvetica%20Neue,Helvetica,Arial,sans-serif&font-size=1&hide-credits=true
```

With the Canvas LMS it is also possible to use an [external web page as content within a course Module](https://community.canvaslms.com/t5/Instructor-Guide/How-do-I-add-an-external-URL-as-a-module-item/ta-p/967).

<img src="https://raw.githubusercontent.com/hibbitts-design/publishing-with-docsify-this/main/images/docsify-this-module.jpg" width="910" height="682" class="responsive image-border" alt="Docsify-This Canvas LMS Module"><br>
<em>Figure 12. Docsify-This External URL with Page Table of Contents (used as a Canvas LMS Module), for example <a href="https://canvas.sfu.ca/courses/76289/modules/items/2816273">https://canvas.sfu.ca/courses/76289/modules/items/2816273</a></em>

```html
https://docsify-this.net?basePath=https://raw.githubusercontent.com/hibbitts-design/cmpt-363-222-pages/main&homepage=week-01.md&toc-narrow=true&font-family=Lato%20Extended,Lato,Helvetica%20Neue,Helvetica,Arial,sans-serif&font-size=1&hide-credits=true
```

## Leveraging Git with GitHub or Codeberg

To get the most out of Docsify-This, consider using GitHub or Codeberg repositories to store your Markdown files. This approach provides version control, enables collaboration through "Edit this Page" links, and allows you to edit content locally on your desktop using your choice of text editor.

### Git

Git is a free and open source distributed version control system,  originally created by Linus Torvalds in 2005 for development of the Linux kernel. 

#### Version Control

Version control supports the management of changes, called revisions, to files... especially useful for pure text files such as those used by Docsify-This.

<img src="https://raw.githubusercontent.com/hibbitts-design/publishing-with-docsify-this/main/images/local.png" alt="Local Version Control" class="responsive-border"><br>
<em>Figure 13. Local Version Control (source: <a href="https://git-scm.com">https://git-scm.com</a>)</em>

#### Collaboration

As a distributed version control system, Git also support collaboration with multiple contributors.

<img src="https://raw.githubusercontent.com/hibbitts-design/publishing-with-docsify-this/main/images/distributed.png" alt="Distributed Version Control" class="responsive-border"><br>
<em>Figure 14. Distributed Version Control (source: <a href="https://git-scm.com">https://git-scm.com</a>)</em>

### GitHub and Codeberg

GitHub and Codeberg are examples of online Git services, letting you more easily create and manage Git repositories.

Besides hosting your files, online editing of repository content such as Markdown files (using the filename extension .md) is also provided.

<img src="https://raw.githubusercontent.com/hibbitts-design/publishing-with-docsify-this/main/images/github-markdown-file.jpg" alt="GitHub Markdown File" class="responsive-border">
<em>Figure 15. GitHub Markdown File</em>

### Docsify-This + GitHub or Codeberg Markdown Files 

To get the most from version control, and potentially collaboration using an optional "Edit this Page" link, store your Docsify-This Markdown pages within a GitHub or Codeberg repository and optionally use an app such as GitHub Desktop to push/pull changes to your desktop.

### Setting up GitHub Desktop

1. Install GitHub Desktop (https://desktop.github.com)
1. Enter your GitHub credentials as prompted
1. Go to a GitHub repository web page, tap **< > Code** and then choose **Open with GitHub Desktop** OR go to a Codeberg repository web page, copy the HTTPS address, then in GitHub Desktop choose **File > Clone Repository** and paste the copied URL
1. Choose the location for your cloned repository and tap the **Clone** button

### GitHub Desktop
  
* Locally Store Git/GitHub/Codeberg Repositories  
* **Push** and **Pull** Repository Changes  

<img src="https://raw.githubusercontent.com/hibbitts-design/publishing-with-docsify-this/main/images/github-desktop-screenshot-mac.jpg" alt="GitHub Desktop" class="responsive-border"><br>
<em>Figure 16. GitHub Desktop Mac (source: <a href="https://git-scm.com">https://git-scm.com</a>)</em>

### Desktop Text Editors

Once your Docsify-This Markdown files are synced (i.e. cloned) to your desktop via GitHub Desktop you can then use the text editor of your choice, such as VSCode, Pulsar Beta (was Atom.io), Typora etc.

Using GitHub Desktop you can preview any changes and then commit those changes back to the repository. VSCode can also be used alone to both sync and editing files.

<img src="https://raw.githubusercontent.com/hibbitts-design/publishing-with-docsify-this/main/images/docsify-this-github.jpg" alt="Docsify-This + GitHub Markdown Files" class="responsive-border">
<em>Figure 17. Docsify-This + GitHub Markdown Files Workflow</em>

<img src="https://raw.githubusercontent.com/hibbitts-design/publishing-with-docsify-this/main/images/docsify-this-webserver.jpg" alt="Docsify-This + Webserver Markdown Files" class="responsive-border"><br>
<em>Figure 18. Docsify-This + Webserver Markdown Files</em>

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