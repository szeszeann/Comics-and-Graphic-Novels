---
section: Write Your Essay
nav_order: 6
title: Customizing Your Website
---
---

**Goals**: Customize the website's home page

**Estimated Time to Complete**: 20 minutes

---

## Step 1. Navigate to your project repository

1. Log in to GitHub (<https://github.com>{:target="_blank" rel="noopener"}).
2. Once you're logged in, select the dropdown arrow in the very top-right corner of your browser window. Once you select this, a dropdown list should appear that starts with the words "Signed in as [your username]." On the dropdown, locate the link titled "Your repositories" and click on it. This will take you to your GitHub account and a list of all the repositories you've ever created.
3. Locate the name of the repository you created for your class project, and click on it. This will bring you to your project repository and website, where you can continue editing files following the steps below.

---

## Step 2. Open your website in a new browser tab or window

1. In the "About" section of your repository homepage (the section to the right of the green "Code" button), locate the URL for your project site. Right-click this URL and select either "Open link in new tab" or "Open link in new window."
2. Now you should have two tabs/windows open: **one with your GitHub repository** (the "*back end*" of your site) and **one with your website** (the "*front end*" of your site). You'll need both of these tabs/windows open for the duration of this Lab, and you'll work with both of them open in future Labs.

---

## Step 3. Add an introduction to your website's homepage

1. From your repository's homepage, locate and click on the "pages" folder.

2. Inside the "pages" folder, click on the file titled "index.md." Then select the pencil button in the top right corner of the `index.md` file to open editing mode.

3. `index.md` contains the text content written on the homepage of your project website! It's written in markdown, just like your essay (notice that the title is a heading 1?). This is an opportunity for you to add your own introduction to your site. It doesn't need to be long, think of it as a brief welcome to the imagined future users of your site, and a short description of what your research is about.

4. When you're ready to write, delete the four paragraphs of stock content (starting with `Instructions for how to use this site to write your multimedia essay...` and ending with `images into your essays`). Delete these four paragraphs, and add your own introduction in their place.

5. Replace the heading `# Writing with Visualizations` with your own title for your homepage.

6. Remember **DO NOT** alter the front matter that exists at the very top of the page (lines 1-6). Leave the front matter exactly as it is, otherwise your site will not work correctly.

7. When you're happy with your title and introduction, commit your changes: add a commit message to the "Commit changes" box at the bottom of the page, then click the green "Commit changes" button.

8. Go back to repository's homepage (if you ever are confused about how to get back to the homepage, click on the "<> Code" tab in the top left section of the screen).

9. Head over to where you opened your website in a different tab or window, and make sure you've navigated to your website's home page.

10. Wait a minute or two, then refresh your website's homepage. Once you refresh your site, you should see your new introduction. The updates may take a few seconds to a few minutes to appear, so hold tight and keep refreshing if you don't see them right away.

---

## Step 4. Add a custom image to your website's homepage

You're welcome to change the image that is featured on the homepage of your website.

### Find an image

You can use an image of your choice, as long as you have the rights to it, or it is in the public domain (images created before 1927 are now in the public domain).
This means that it should be an image that you've created, or an image that is not under copyright.

Some options to find public domain include:

- Unsplash: <https://unsplash.com/>{:target="_blank" rel="noopener"}
- Wikimedia Commons: <https://commons.wikimedia.org/wiki/Main_Page>{:target="_blank" rel="noopener"}

### Upload your image

When you've found the image you want to use, upload it to your repository's "objects" folder following these steps:

1. In your repository, locate and click on the "**objects**" folder (directly above the "pages" folder). There are already some files in this folder, and we're going to add your new file to them.

2. Towards the top right of the page (where the pencil button would normally be) locate the "Add file" button and click on it. This is a dropdown button that gives you two options: "Create new file" and "Upload files." Select "**Upload files**."

3. This brings you to a page that says "Drag files here to add them to your repository or choose your files." Click on the "choose your files" link. This will open up your File Explorer application (on a Windows machine) or your Finder application (on a Mac).

4. In File Explorer/Finder, locate and select the image that you've decided to use.

5. Once you've selected the correct file, click the "Open" button in the bottom right of your File Explorer/Finder window. This will automatically trigger GitHub to upload the file.

6. In order to finalize the upload, you'll need to commit the change, so add a commit message to the "Commit changes" box at the bottom of the page, then click the green "Commit changes" button.

7. After you commit the file, GitHub will automatically redirect you to the repository's homepage. If you want to you can look inside your "**objects**" folder again to see the file you just uploaded, but this isn't necessary.

### Set up your image to display on the homepage

1. In your repository, locate and click on the "**_data**" folder (the folder at the very top of your repository!). Inside the _data folder, locate the `theme.yml` file and click on it. Then select the pencil button in the top right corner of the `theme.yml` file to open editing mode.

2. This file is written in [YAML](https://collectionbuilder.github.io/cb-docs/docs/glossary/#yaml), just like your `_config.yml` is! Remember, YAML is a data type made up of key-value pairs, separated by a colon (`:`). You will also see comments in this file (indicated by a pound sign (`#`) at the beginning of a line). Locate the comment that reads `# HOME PAGE`.

#### featured-image:

- In the `# HOME PAGE` section, locate the `featured-image: feature-image.jpg` key-value pair. To add your own image, replace the value `featured-image.jpg` with your image's filename (including file extension). For instance, if you just uploaded an image with filename `digital-project-homepage.jpg` to your objects folder, this is the exact value you'd use for `featured-image`. Note that any typos will cause your image not to appear, so be sure to double check that your spelling matches the actual filename. You can use either PNG or JPG files for your featured image.

#### home-title-y-padding:

- Underneath `featured-image`, there is the key-value pair `home-title-y-padding: 9em`. This key lets you adjust how tall your image appears on your homepage. You can reduce the size of the image by replacing the number 9 with a number less than 9 (example: `6em`). You can increase the size of the image by replacing the number 9 with a number greater than 9 (example: `12em`). Remember to include the letters `em` after the number you choose! The em unit is used in web development to measure padding around elements on the webpage.

#### home-banner-image-position:

- Finally, if desired, you can change the position of your featured image. By default, your image will display so that the center of the image is aligned with your site title. You can add a value to the key `home-banner-image-position` to make your image positioned from its top or bottom instead of center. To do this, add the value `top` or the value `bottom` to the right of the colon (`:`) after the `home-banner-image-position` key, but before the pound sign (`#`) (remember, everything after the pound sign is a comment, so if you add the value after the sign, the computer won't register it!). To keep the position at center, just leave the value for `home-banner-image-position` blank.

### Commit your changes:
- Add a commit message to the "Commit changes" box at the bottom of the page, then click the green "Commit changes" button.
- Head over to where you opened your website in a different tab or window, and make sure you've navigated to your website's Home page.
- Wait a minute or two, then refresh your website's homepage.
- Once you refresh your site, you should see the changes to the image on your homepage.
- The updates may take a few seconds to a few minutes to appear, so hold tight and keep refreshing if you don't see them right away.

{:.alert .alert-success}
**NOTE**: It's entirely possible that you won't like the edits you made to the padding or the image position! That's okay! Just go back into the theme.yml file and edit them again. If you find that you do not like the image that you added, feel free to use the default image that came with the site. Simply use the value `feature-image.jpg` for the `featured-image` key.

---