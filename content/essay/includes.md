---
section: Write Your Essay
nav_order: 5
title: Including Primary Sources
---

---

**Goals**: Include images and documents in essay

**Estimated Time to Complete**: 30 minutes

---

## Step 1. Locating and Downloading Digital Objects

Please locate and download an image you'd like to include in your essay.

For guidance on where to look for digitized primary sources that you can incorporate into your essay, please see the Multimedia Essay [Assignment](/content/essay/assignment.html){:target="_blank" rel="noopener"} page.

Here are a few suggestions:

- [National Archives](https://www.archives.gov/research){:target="_blank" rel="noopener"}
- [Internet Archive](https://archive.org/index.php){:target="_blank" rel="noopener"} (not all sources here are primary, so you’ll need to be careful)
- [Chronicling America](https://chroniclingamerica.loc.gov/){:target="_blank" rel="noopener"}
- [Digital Public Library of America](https://dp.la/){:target="_blank" rel="noopener"}

Remember to keep copyright in mind as you think about incorporating images and documents into your essay. 

### Downloading your digital object

Once you've found an item you can use in your essay, you'll need to download it to your computer.

Take a close look at webpage from which you'd like to download an item to use in your essay.
More often than not, there will be a "download" button somewhere on the page, allowing you to download the image or PDF.
If you've looked and are *absolutely sure* that there is no "download" option, you can resort to taking a screenshot of the item.

When you download an item or take a screenshot, keep track of where that file is saved on your computer (most likely your "Downloads" folder if it's a download, or "Desktop" if it's a screenshot).
You'll need to remember this location when you go to upload it to your GitHub repository in the next step.

Also keep track of the URL of the webpage from which you downloaded your item.
You'll need to embed this so that your readers will be able to see the sources of your primary sources.

Follow the steps below to incorporate your chosen image or PDF into your essay.

---

## Step 2. Navigate to Your Project Repository

1. Log in to GitHub (<https://github.com>{:target="_blank" rel="noopener"}).
2. Once you're logged in, select the dropdown arrow in the very top-right corner of your browser window. Once you select this, a dropdown list should appear that starts with the words "Signed in as [your username]." On the dropdown, locate the link titled "Your repositories" and click on it. This will take you to your GitHub account and a list of all the repositories you've ever created.
3. Locate the name of the repository you created for this project, and click on it. This will bring you to your project repository and website, where you can continue editing files following the steps below.

---

## Step 3. Open Your Website in a New Browser Tab or Window

1. In the "About" section of your repository homepage (the section to the right of the green "Code" button), locate the URL for your project site. Right click this URL and select either "Open link in new tab" or "Open link in new window."
2. Now you should have two tabs/windows open: **one with your GitHub repository** (the "*back end*" of your site) and **one with your website** (the "*front end*" of your site). You'll need both of these tabs/windows open for the duration of this Lab, and you'll work with both of them open in future Labs.

---

## Step 4. Upload an image to the GitHub repository

1. Switch to the browser tab that holds your GitHub repository, and navigate to the homepage of your GitHub repository by clicking on the <> Code tab above your repository files.
2. In your repository, locate and click on the "**objects**" folder (directly above the "pages" folder). There are already some demo files in this folder, and we're going to add your new file to them.
3. Towards the top right of the page (where the pencil button would normally be) locate the "Add file" button and click on it. This is a dropdown button that gives you two options: "Create new file" and "Upload files." Select "**Upload files**."
4. This brings you to a page that says "Drag files here to add them to your repository or choose your files." Click on the "choose your files" link. This will open up your File Explorer application (on a Windows machine) or your Finder application (on a Mac).
5. In File Explorer/Finder, locate the file you'd like to upload to your essay. 
6. Once you've selected the correct file, click the "Open" button in the bottom right of your File Explorer/Finder window. This will automatically trigger GitHub to upload the file.
7. In order to finalize the upload, you'll need to commit the change, so add a commit message to the "Commit changes" box at the bottom of the page, then click the green "Commit changes" button.
8. After you commit the file, GitHub will automatically redirect you to the repository's homepage. If you want to you can look inside your "objects" folder again to see the file you just uploaded, but this isn't necessary.

---

**Need a visual? Follow along with the video below:**

{% include video-embed.html youtubeid="_huFCz1LDyQ" caption="Upload an Image to Your GitHub Repository" %}

---

## Step 4. Locate the "Include Generator" Form

1. Switch to the browser tab that holds the "front end" of your project website.
2. In the navigation bar, locate and click on "Include Generator." We are going to use this form to generate an "include," a snippet of text that will allow us to display images on our essays, just as we displayed topic graphs last week.

---

## Step 5. Input Information About Your Object

1. In the middle of the "Include Generator" page, click on the dropdown that says "Select include type," and select "image" or "document" from the dropdown options, then follow the appropriate instructions below.

#### Image Options

1. Click on the **Image filename** dropdown. Select the file you just uploaded to your GitHub repository.
2. Fill out the following fields:

- **Image alt text** (required): Allows screen readers to describe images to them as they navigate the web. Value should be should be brief but descriptive text that identifies the image you've uploaded. For instance, `image of a word cloud generated from Party Platform texts from the years 1900-1944` would be an appropriate value.

- **Image caption** (optional): Adds a brief caption underneath the image. Keep your caption length to a sentence or less. 

- **Image width** (optional): Controls how large your image is displayed on your essay. Choose from four values: 25%, 50%, 75%, and 100%. If left blank, will automatically display at 100%.

- **Image link** (optional but highly recommended): Links back to the website where you found your image.

<br>

#### PDF Options

1. Click on the **Image filename** dropdown. Select the file you just uploaded to your GitHub repository.
2. Fill out the following fields:

- **Document caption** (optional): Adds a brief caption underneath the document. Keep your caption length to a sentence or less. 

- **Document width** (optional): Controls how large your document is displayed on your essay. Choose from four values: 25%, 50%, 75%, and 100%. If left blank, will automatically display at 100%.

- **Document link** (optional but highly recommended): Links back to the website where you found your document.

---

## Step 6. Copy and Paste the Include Code Into the Essay

Once you've filled in the desired fields in your form, click the blue "Submit" button at the bottom of the form. 
This will generate a box that appears beneath the form, titled "Include code," and containing a line of pink "include" text that looks similar to this:

`{% raw %}{% include feature/image.html filename="sotu-word-cloud.png" alt="image of a word cloud generated from corpus of 20th century State of the Union Addresses" width="50" %}{% endraw %}`

Copy **all** of the pink include text (brackets and all), then follow these steps to paste it into your `essay.md` file:

1. Click over to the browser tab that holds your GitHub repository, and navigate to the homepage of your GitHub repository by clicking on the <> Code tab above your repository files.

2.  Locate and click on the "pages" folder in your repository.

3.  Inside the "pages" folder, locate and click on the `essay.md` file.

4. Click the pencil button at the top right of your `essay.md` file to open editing mode.

5. Choose a line in your essay in which you'd like to insert your item.

6. Scroll down to the bottom of the file and type a commit message into the "Commit changes" text box.

7. Click the green "Commit changes" button to save your changes.

8. Head over to where you opened your website in a different tab or window, and use the navigation menu to switch back to the "Essay" page.

9. Wait a minute or two, then refresh the "Essay In Progress" page. Once you refresh your site, you should see the new image appear below your essay title. The updates may take a few seconds to a few minutes to appear, so hold tight and keep refreshing if you don't see them right away.

---

**Need a visual? Follow along with the video below:**

{% include video-embed.html youtubeid="_zzZnXaAp0o" caption="Generate an Image Include and Add It to Your Essay" %}

---