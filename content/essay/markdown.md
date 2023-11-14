---
section: Write Your Essay
nav_order: 3
title: Writing in Markdown
---

---

**Goals**: Add text to essay

**Prerequisites**: [Learn Static Markdown Foundations Module](https://github.com/learn-static/foundations-2-markdown/blob/main/intro-markdown.md){:target="_blank" rel="noopener"}

**Estimated Time to Complete**: 30 minutes

---

## Step 1. Navigate to Your Project Repository

1. Log in to GitHub (<https://github.com>{:target="_blank" rel="noopener"}).
2. Once you're logged in, select the dropdown arrow in the very top-right corner of your browser window. Once you select this, a dropdown list should appear that starts with the words "Signed in as [your username]." On the dropdown, locate the link titled "Your repositories" and click on it. This will take you to your GitHub account and a list of all the repositories you've ever created.
3. Locate the name of the repository you created for this project, and click on it. This will bring you to your project repository and website, where you can continue editing files following the steps below.

---

## Step 2. Open Your Website in a New Browser Tab or Window

1. In the "About" section of your repository homepage (the section to the right of the green "Code" button), locate the URL for your project site. Right click this URL and select either "Open link in new tab" or "Open link in new window."
2. Now you should have two tabs/windows open: **one with your GitHub repository** (the "*back end*" of your site) and **one with your website** (the "*front end*" of your site). You'll need both of these tabs/windows open for the duration of this Lab, and you'll work with both of them open in future Labs.

---

## Step 3. Locate your essay.md file

1. Navigate to the browser tab/window that contains your GitHub repository.
3. In your GitHub repository, locate and click on the "pages" folder.
4. Inside the "pages" folder, click on the file titled "essay.md." Then select the pencil button in the top right corner of the `essay.md` file to open editing mode. 

The content of the `essay.md` file should look like this:

```
---
title: Essay
layout: about
permalink: /essay.html
---

{% raw %}{% include feature/nav-menu.html sections="Introduction;Conclusion;Notes" %}{% endraw %}]

# My Essay Title

## Introduction

## Conclusion

## Notes

```

Below, we will discuss how to add your text content to this document.

---

## Step 4. Front Matter

At the very top of the file (**lines 1-5**), you'll see the following:

```
---
title: Essay
layout: about
permalink: /essay.html
---
```
This little grouping of text is called "front matter."
It must be left exactly as it is for your site to work correctly, so ***don't change it!***. 
Simply ignore it and move to the next section.

---

## Step 5. Markdown

The content in your `essay.md` file is written in a format called "Markdown."
Markdown was developed as a simple way to write content for the web without using HTML (hypertext markup language), a language commonly used to write content for websites.
We're using Markdown for your essays because it is much simpler than HTML, yet it will still allow you to create web essays that easily incorporate images, pdfs, and visualizations.

Markdown is very similar to the way you write and format content in Microsoft Word documents, but uses symbols and spacing to organize and emphasize text.

{% include alert.html text="**Note**: Before continuing through the next steps to edit your essay, please make sure you've completed the [Learn-Static Foundations Markdown Module](https://github.com/learn-static/foundations-2-markdown/blob/main/intro-markdown.md){:target='_blank' rel='noopener'}" color="danger" %}

Practice editing the following components of your Markdown file:

{:#headings}
### Headings

Headings are used to title a section in your essay, and are indicated with one or more pound signs (`#`) in front of them.

{:#paragraphs}
### Paragraphs

Keep an empty line between paragraphs, and do not indent the first sentence of a paragraph.

1. Click the pencil button at the top right of your `essay.md` file to open editing mode.

2. Underneath the new essay title that you just created, add two or three sentences of text (the subject can be anything, related or unrelated to your essay topic, this is just for practice).

### Font styles

{:#italic}
To make a word or phrase *italic*, add one asterisk before and after that word or phrase, like this: `*example phrase*`.
The asterisks won't be visible on your webpage, but your text will appear italicized.

{:#bold}
To make a word or phrase **bold**, add two asterisks before and after that word or phrase, like this: `**example phrase**`.
Again, the asterisks won't be visible on your webpage, but your text will appear bold.

{:#hyperlinks}
### Hyperlinks

To link to another page or site, insert the link title (what you want displayed to the site visitors) into square brackets, followed by a URL in parentheses: 
`[GitHub Help](https://help.github.com/)` in your `essay.md` file will look like [GitHub Help](https://help.github.com/) on your "Essay In Progress" webpage.

{:#lists}
### Lists

You can create lists in two different ways:

A bullet list is created using a hyphen (`-`) in front of each bullet point:

- dog
- cat
- muffin

A numbered list is created using a number followed by a period (`.`) in front of each list item:

1. one
2. two
6. three
2. four

### Now try it yourself

1. Click the pencil button at the top right of your `essay.md` file to open editing mode.

2. In your `essay.md` file, replace the words in the first heading `# My Essay Title` with a new title for your essay . Make sure you include one `#` in front of your essay title, like this: `# My New Essay Title`.

3. Create an empty line underneath the `## Introduction` heading. Under this empty line, add two or three sentences of text (the subject can be anything, related or unrelated to your essay topic, this is just for practice).

4. Add some italic and bold text and a hyperlink to the sentences you just created

5. Leaving a blank line underneath the `## Conclusion` heading, add either a bullet list or numbered list.

3. Scroll down to the bottom of the file and type a commit message into the "Commit changes" text box.

4. Click the green "Commit changes" button to save your changes.

5. Head over to where you opened your "Essay" page in a different tab or window.

6. Wait a minute or two, then refresh the "Essay" page.

7. Once you refresh your site, you should see your changes.

8. The updates may take a few seconds to a few minutes to appear, so hold tight and keep refreshing if you don't see them right away.

---

Continue to the next step to learn how to edit the Table of Contents at the top of your essay and create citations. 