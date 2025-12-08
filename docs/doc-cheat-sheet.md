
# Documentation Cheat Sheet
This is your [MkDocs Reference (with the Material theme)](https://squidfunk.github.io/mkdocs-material){target="_blank"} MkDocs (Material theme) cheatsheet covering headers, lists, links, images, code blocks, tables, and more – all in one printable page for quick reference when writing docs, READMEs, or tutorials.
{: .indent-h1 .intro }

This markdown cheat sheet is not an exhaustive list of markdown tags available to you, only the bare minimum to help you create and edit beautiful documentation and tutorials.  For a full list of available markdown tags, visit the [Material for MkDocs Reference](https://squidfunk.github.io/mkdocs-material/reference){target="_blank"} documentation.
{: .indent-h1 .intro }

Remember, unreadable documentation is useless. Beautiful documentation is readable and useful. Make it beautiful in order to make it useful.
{: .indent-h1 .intro }


## CONTENT AND LAYOUT

All document pages are to be organized hierarchically using H1 to H6 headings with appropriate indentation.
{: .indent-h2 }

### Indent H1 Paragraph

:warning: **WARNING!** - H1 headings and paragraphs are special. We do not indent the text but we do use a slightly larger font to draw attention to the introduction of each page. The following attribute must be used for these paragraphs:
{: .indent-h3 }

<div class="indent-h3">
```markdown title="Markdown Example"
# This is a Heading (H1)
Condimentum olestie leo pellentesque bibendum olestie.
{: .indent-h1 .intro }

```
</div>

### Indent Headings and Text
All pages are to be organized into hiearchies with headers (H1 through H6) and indented appropriately for readability as follows: 
{: .indent-h3 }

<div class="indent-h3">
```markdown title="Markdown Example"
## This is a Heading (H2)
Dolor nisl facilisis tincidunt vel.
{: .indent-h2 }

### This is a Heading (H3)
Rutrum condimentum nec placerat gravida leo et quisque phasellus .
{: .indent-h3 }

#### This is a Heading (H4)
Erat morbi felis proin quis sit mi cursus tincidunt.
{: .indent-h4 }

##### This is a Heading (H5)
Magna lorem mi sit rutrum tempus eu quis orci.
{: .indent-h5 }

###### This is a Heading (H6)
Enim magna ac morbi rtaest maximus ut id felis.
{: .indent-h6 }

```
</div>

### Indent an ordered/unordered list

Lists cannot be indented even if wrapped with <div\></div\> tags. We need to drop to inline html code and manually create lists as follows (note the class="indent-h3" used for indentation):
{: .indent-h3 }

#### Indented Unordered List

<div class="indent-h4">
```html title="Unordered List Example"
<ul class="indent-h4">
<li>
    List item.
</li>
<li>
    List item.
</li>
</ul>

```
</div>

#### Indented Ordered List

<div class="indent-h4">

```html title="Ordered List Example"
<ol class="indent-h4">
<li>
    List item.
</li>
<li>
    List item.
</li>
</ol>

```
</div>

### Indent a Code Block

If we need to indent code blocks under headings, we wrap the code block with the following inline html code:
{: .indent-h3 }

<div class="indent-h3">
````markdown title="This is a Markdown Example"
<div class="indent-h4">

```markdown title="Markdown Example"

Text can be {--deleted--} and replacement text {++added++}. This can also be combined into {~~one~>a single~~} operation. {==Highlighting==} is also possible {>>and comments can be added inline<<}.

```
</div>
````
</div>

### Indent an Admonition

Regular admonition syntax cannot be used even if wrapped in <div\></div\> tags. Instead, we drop down to plain html and create Admonitions that can be indented like this (note the class="margin-h4" style for indentation):
{: .indent-h3 }

<div class="indent-h3">
```markdown title="Markdown Example"
<div class="admonition note margin-h4">
<p class="admonition-title">Note</p>
<p>
This is an admonition note.
</p>
</div>
```
</div>

The example Admonition renders like this:
{: .indent-h3 }

<div class="admonition note margin-h4">
<p class="admonition-title">Note</p>
<p>
This is an admonition note.
</p>
</div>



You can find the available Admonition notes on the [Material for MkDocs - Admonitions](https://squidfunk.github.io/mkdocs-material/reference){target="_blank"} page.
{: .indent-h3 }

### Documentation Custom CSS

We created custom css classes to help us indent page components. The css file is well documented and you can find it here: 
{: .indent-h3 }

<div class="indent-h3">
```yaml title="Location of custom CLOG css for the documentation"
.
├─ docs/
│  └─ src/
│     └─ styles/
│        └─ clog-styles.css
└─ mkdocs.yml[B

```
</div>


## TEXT STYLING

<div class="admonition warning margin-h2">
<p class="admonition-title">Warning</p>
To be completed.
</p>
</div>

## MEDIA

Image:

<div class="admonition warning margin-h2">
<p class="admonition-title">Warning</p>
To be completed.
</p>
</div>

Local Video:

<div class="admonition warning margin-h2">
<p class="admonition-title">Warning</p>
To be completed.
</p>
</div>

Hosted Video (Youtube):

<div class="admonition warning margin-h2">
<p class="admonition-title">Warning</p>
To be completed.
</p>
</div>

## ADMONITIONS

:warning: **WARNING!** - We cannot use the standard MkDocs Admonitions markup because indenting them properly is not possible even if we wrap them in <div\><\div\> tags.
{: .indent-h2 }

Instead, we drop down to inline html and manually create the Admonitions like this (note the class="margin-h2" style used for indentation in this example): 
{: .indent-h2 }

<div class="margin-h2">

```
<div class="admonition note margin-h2">
<p class="admonition-title">Note</p>
<p>
This is a note.
</p>
</div>
```
</div>

The Admonitions look like this:

<div class="admonition note margin-h2">
<p class="admonition-title">Note</p>
<p>
This is a note.
</p>
</div>

<div class="admonition warning margin-h2">
<p class="admonition-title">Warning</p>
<p>
This is a warning.
</p>
</div>

<div class="admonition example margin-h2">
<p class="admonition-title">example</p>
<p>
This is an example.
</p>
</div>

You can find the available Admonition notes on the [Material for MkDocs - Admonitions](https://squidfunk.github.io/mkdocs-material/reference){target="_blank"} page. Use the code above and adjust for the Admonitions you want to use.
{: .indent-h3 }

## ANNOTATIONS

:warning: **WARNING!** - Do not use Annotations in documenation and tutorials. Annotations hide information from the user and are better suited for other use cases.
{: .indent-h3 }

## DIAGRAMS

The Diagrams feature of MkDocs uses the [Mermaid.js]((https://squidfunk.github.io/mkdocs-material/reference){target="_blank"}){target="_blank"}.
{: .indent-h3 }

For example, this documentation project is currently being built on top of the [Material for MkDocs](https://squidfunk.github.io/mkdocs-material){target="_blank"} software stack. Unfortunately, as of the first week of November 2025, Material for MkDocs is [deprecated and in maintenance mode](https://github.com/squidfunk/mkdocs-material/issues/8523){target="_blank"}. The authors are building a drop-in replacement called [Zensical](https://zensical.org){target="_blank"}.
{: .indent-h3 }

Because we have already invested some time into building our documentation system, we now need to consider the following options:
{: .indent-h3 }


<ul class="indent-h3">
<li>
Keep documentation on MkDocs and see what happens, migrate to a CLOG native wiki when ready?
</li>
<li>
Keep documentation on MkDocs and migrate to Zensical and THEN to a CLOG native wiki?
</li>
<li>
If MkDocs is unable to handle our needs, do we migrate to Zensical right away?
</li>
<li>
What if the CLOG native wiki is ready for testing, do we migrate to that right away?
</li>
</ul>


We can create a visualization of the above decision tree with Mermaid as follows:
{: .indent-h3 }

``` mermaid
graph LR
  A[Start with MkDocs] --> B{Evaluate MkDocs};
  B -->|Yes| C[Stick with MkDocs];
  B -->|No| D[Evaluate Zensical];
  C -->|Migrate| F[CLOG Native Wiki];
  C -->|Migrate| E[Zensical];
  E -->|Migrate| F[CLOG Native Wiki];
  D -->|Migrate| F[CLOG Native Wiki];
  B ---->|If CLOG Native Wiki is ready before Zensical is ready -> Migrate| F[CLOG Native Wiki];
  
```


## TOOLTIPS

<div class="admonition warning margin-h2">
<p class="admonition-title">Warning</p>
To be completed.
</p>
</div>

## CONCLUSION

As of November 07, 2025, Material for MkDocs seems to do everything that we need. The key requirement that we were looking for are:
{: .indent-h2 }

<ul class="task-list indent-h2">

<li class="task-list-item">
<label class="task-list-control">
<input type="checkbox" checked="">
<span class="task-list-indicator"></span>
</label>
Looking for a solution that supports the absolute minimum of markup syntax elements required for proper page layouts.
<br>
<b>MATERIAL for MkDocs VERDICT:</b> Pass
</li>

<li class="task-list-item">
<label class="task-list-control">
<input type="checkbox" checked="">
<span class="task-list-indicator"></span>
</label>
Suport for Github markup and Github integration.
<br>
<b>MATERIAL for MkDocs VERDICT:</b> Pass
</li>

<li class="task-list-item">
<label class="task-list-control">
<input type="checkbox" checked="">
<span class="task-list-indicator"></span>
</label>
The site generator software has to be easy to install,  configure and learn to use.
<br>
<b>MATERIAL for MkDocs VERDICT:</b> Pass. Easy for developers not easy for regular users at all.
</li>

<li class="task-list-item">
<label class="task-list-control">
<input type="checkbox" checked="">
<span class="task-list-indicator"></span>
</label>
The documentation solution needs to support modern and up to date themes and templating, as well as make it relatively easy to get a documentation site up and running with mostly copy/paste of code examples and turning on features.
<br>
<b>MATERIAL for MkDocs VERDICT:</b> Pass. Material looks fantastic, tons of features.
</li>

<li class="task-list-item">
<label class="task-list-control">
<input type="checkbox" >
<span class="task-list-indicator"></span>
</label>
The documentation solution needs to be under active development and support.
<br>
<b>MATERIAL for MkDocs VERDICT:</b> FAIL. Solution is deprecated, devs are building a stand in replacement called Zensical. Solution does have 12 months of support going forward and our work transfers so we have time to migrate.
</li>

<li class="task-list-item">
<label class="task-list-control">
<input type="checkbox" checked="">
<span class="task-list-indicator"></span>
</label>
The site generator needs must use a free software license.
<br>
<b>MATERIAL for MkDocs VERDICT:</b> Pass.
</li>

</ul>

First, there is no way to test all of the static site generators available on the marketplace. A reasonable Google search was done to find the most popular options that met our needs and get us to start testing right away.
{: .indent-h2 }

Some of the other solutions considered:
{: .indent-h2 }


<ul class="indent-h2">
<li>
    DocuSaurus
</li>
<li>
    Jekyll
</li>
<li>
    Sphinx
</li>
<li>
    GitBook
</li>
<li>
    Hugo
</li>
<li>
    Gatsby
</li>
</ul>


Competing documentation solutions are either too complex and too powerful, difficult to setup and run, don't have enough features that support beautiful layouts or are proprietary.
{: .indent-h2 }

MkDocs has two majour flaws: It is deprecated in favor of Zensical and we cannot indent many of the markdown components without dropping down to raw inline html and applying the appropriate css classes. Compared to the pain points of the competing systems, these are relatively minor and we can work around them for now.
{: .indent-h2 }




