---
section: Get Started
nav_order: 2
title: Website Setup
---

---

**Goals**: Copy a GitHub repository template; Edit the repository's configuration file; Turn on GitHub Pages

**Prerequisites**: [Learn Static GitHub Foundations Module](https://github.com/learn-static/foundations-0-github/blob/main/intro-github.md){:target="_blank" rel="noopener"}

**Estimated Time to Complete**: 30 minutes

---

Now that you've created a GitHub account, you'll be working on GitHub to set up your project website. 

## Step 1. Log in to GitHub

1. Go to <https://github.com>{:target='_blank' rel='noopener'} and sign in.

{:#template}
## Step 2. Copy the project template repository

Remember, a GitHub repository is a folder that stores a project's files and keeps track of changes to those files over time.
Let's copy our "Writing with Visualizations" project template repository to your GitHub account so you can start editing it.

1. Go to the [Writing with Visualizations](https://github.com/learn-static/text-analysis){:target="_blank" rel="noopener"} repository and locate and click on the green "Use This Template" button (appears on the top right side of the screen above the code area). Note that the "Use This Template" button only appears if you're logged into GitHub!
2. This brings you to a "Create a new repository" form. Follow these steps:
    1. **Repository name**: Use a lowercase name without spaces or odd characters (no `$`, `#`, `@`, `?`, `!`, etc.). Hyphens (`-`) and underscores (`_`) are okay to use. Keep in mind that this repository name will become part of your project site's URL, so think through how it will look as a link!
    2. In the **Description** text box, add a very brief description of your project, something like: `My multimedia essay project`.
    3. Select the option for "**Public**" repository.
    4. Leave the "Include all branches" option **Unchecked**!
    5. Click on the green button titled "**Create repository from template**". This will take you to your new repository (note that it may take a few seconds to generate).

**Need a visual? Follow along with the video below:**

{% include video-embed.html youtubeid="VJwcyeHUtw4" caption="Copy a GitHub Repository" %}

## Step 3. Edit the site settings

1. Take a look at the files in your repository and locate the one titled `_config.yml`. Click on this file to open it.
2. In the top right corner of the `_config.yml` file, locate and click on the pencil icon to enter GitHub's editing mode.

The `_config.yml` file is used to configure the core features of your project site (things like the site's title, author, and tagline).
The configuration options are made up of key-value pairs, separated by a colon (`:`), and written in a format called [YAML](https://collectionbuilder.github.io/cb-docs/docs/glossary/#yaml). 
For example, below is the **key**, "title", followed by its **value**, "Analyzing Political Text of The 20th Century":

```
# title of site appears in banner
title: Analyzing Political Text of The 20th Century
```

Above "title," the line of text that starts with a pound sign (`#`) is a **comment**.
The comment is a note to you, the website creator, to tell you what value you should add to the title. 
The computer ignores the comment but processes the title key and value.
Any line in this `_config.yml` file that starts with a `#` is a comment.

Right now, placeholders fill all the values in the `_config.yml` file.
You'll need to switch out these placeholders with the information you create about your individual site.

**There are four values you need to edit**.
Below, we'll walk through editing each one.

To get started, first look for the SITE SETTINGS comment.
It should look like this:

```
##########
# SITE SETTINGS
```

Directly *above* the SITE SETTINGS comment, locate the "source-code" key.  

### source-code: 

- `source-code` is the full URL for the GitHub repository containing your project code. It is used on your website to add a link back to your project repository. Copy your repository's URL and paste it over the example text to the right of `source-code:`

For example, the default placeholder value is this:
```
source-code: https://github.com/learn-static/text-analysis
```

And should be replaced with your own repository's URL:
```
source-code: https://github.com/my-github-name/my-repository-name
```

Now move on to the three values *below* `# SITE SETTINGS`, and fill them out: 

### title: 

- `title` is the title of your digital project. This will appear as the title on your website's home page, and on every other page's header and footer. Change the words `Writing with Visualizations` to a title of your choice.
```
title: Writing with Visualizations
```

### tagline: 

- `tagline` is an *optional* descriptive subtitle for the digital project. This will appear underneath the title on your site's home page and on every other page's header. Replace the words `Create a multimedia essay webpage and visualize historical text as data` with a tagline of your choice.
```
tagline: Create a multimedia essay webpage and visualize historical text as data
```

### author: 

- `author` is you! The creator of the digital project. Use your GitHub username or your name. This will only appear in the site's meta tags and won't be visible on the site itself. Change the name `owikle` to your own name or username.
```
author: owikle
```

**That's it!**
There's nothing else you need to edit in the `_config.yml` file.
Proceed to the next step to save your changes.

## Step 4. Commit changes to _config.yml
1. To commit the changes you just made to your `_config.yml` file, scroll to the bottom of the page where you made your edits. You'll see a box titled "Commit changes."
2. In the text box directly underneath "Commit changes," type a short message that describes your edits, such as "update site settings".
3. Skip the option to add an extended description to the commit, and keep the box checked next to "Commit directly to the main branch".
4. Click on the green "Commit changes" button. This will save your changes and take you out of the "edit" mode.
5. Go back to repository's homepage (if you ever are confused about how to get back to the homepage, click on the "<> Code" tab in the top left section of the screen).

**Need a visual? Follow along with the video below:**

{% include video-embed.html youtubeid="Gq4vS9q13mc" caption="Edit a Configuration File" %}

{:#gh-pages}
## Step 5. Activate GitHub Pages

Now you're going to actually "turn on" your website by telling GitHub to generate a website from your repository.

1. On your project repository's homepage, click the "Settings" button (appears on the right, towards the top of the page, just above the green "code" button).
2. On the "Settings" page, locate the "Code and automation" section of the menu on the left.
3. Under "Code and automation," click on "Pages." This will take you to a page titled "GitHub Pages."
4. Underneath the title "GitHub Pages," locate the section titled "Source." Change the dropdown button from "none" to "main."
5. Leave the other dropdown button just as it is (it should say "/(root)"), then click the "Save" button.
6. Once saved, the page will refresh with a green alert that provides the URL where your site will appear. 

**Note that it takes a few minutes for your site to go live, so if you click on the URL right away, you'll only see a 404 webpage.** 
***This is normal!***
Proceed to the next section while you're waiting for your site to build.

## Step 6. Add your new URL to the homepage of your GitHub repository

While you're waiting for your site to build, we will set up our new site URL to display on your GitHub repository homepage, to make it easier for you to access in the future:

1. Copy the URL that GitHub created for you.
2. Go to repository's homepage (if you ever are confused about how to get back to the homepage, click on the "<> Code" tab in the top left section of the screen).
3. On the right side of the code area, to the right of the green "Code" button, look for the word "About". Click the cog icon to the right of "About." A box titled "Edit repository details" will pop up.
4. In the "Edit repository details" popup, paste your URL into the "Website" section, then click the green "Save changes" button. This will post your URL underneath the "About" section on your GitHub repository's homepage, making it easy to access the site in the future!

Now click on your URL again to see if your site is live yet.
If you still get the 404 page, don't worry--sometimes it can take up to five minutes.
Refresh your browser every minute or so to check to see if it's live.

If after five minutes it's still not live, make sure you've followed the steps above, and if you're still having trouble reach out to Professor Wikle who can help you troubleshoot.

**Need a visual? Follow along with the video below:**

{% include video-embed.html youtubeid="d2I6Z3u8_Tc" caption="Turn on GitHub Pages" %}

## Step 7. Celebrate!

Congratulations! 
Today you created a website. 
Take some time to click around your new site and explore the pages.
In the next lesson we'll start adding content to the site and visualizing some topic modeling done with the Party Platforms and State of the Union Addresses.