---
section: For Instructors
nav_order: 3
title: Voyant Data
---

This project can be applied to multiple disciplines, and implemented with or without the DH emphasis.
To this end, while the project template's topic modeling feature contains data intended for history students by default, this data can be supplemented or exchanged with whatever the instructor prefers.

**About the demo data used for this project:**

The State of the Union Addresses and Party Platforms used for the text analysis and topic modeling in this project template were obtained from the University of California Santa Barbara's [American Presidency Project](https://www.presidency.ucsb.edu/documents){:target="_blank" rel="noopener"}. 
This data can be found in multiple formats in the project template's GitHub repository in the [/assets/data/](https://github.com/learn-static/text-analysis/tree/main/assets/data){:target="_blank" rel="noopener"} folder.

Only Democratic and Republican parties were included in our 20th-century Party Platforms data.

The stopword list used for the State of the Union Address and Party Platform text analysis is the Buckley-Salton stopword list, retrieved from Alan Liu's workshop at [http://dhworkshop.pbworks.com/w/file/105416844/Buckley-Salton-stopword-list.txt](http://dhworkshop.pbworks.com/w/file/105416844/Buckley-Salton-stopword-list.txt){:target="_blank" rel="noopener"}. The Buckley-Salton stopword list was also used for the Party Platforms, with the addition of three words: america, american, and americans.

To prepare the demo corpus for text analysis with [Voyant Tools](https://voyant-tools.org/){:target="_blank" rel="noopener"}, we split each State of the Union Address and Party Platform into its own text file, then uploaded all of the State of the Union text files into one instance of Voyant, and all of the Party Platform text files into another instance of Voyant.
To view these text files, see the [/assets/data/state-of-the-union/txt/](https://github.com/learn-static/text-analysis/tree/main/assets/data/state-of-the-union/txt/) folder and [/assets/data/party-platforms/txt/](https://github.com/learn-static/text-analysis/tree/main/assets/data/party-platforms/txt/) folder in the project template's GitHub repository.

We then added links to these Voyant instances (one with State of the Union files and one with Party Platform files) to the documentation's [Voyant](/content/digital-humanities/voyant.html) page as buttons, so that students can link out to them easily.

As an alternative to pre-loading the text into Voyant, if time allows you could choose instead to teach students how to upload the requisite text files to the Voyant home page themselves.

## Prepare New Voyant Data

1. Obtain and clean a body of text that you'd like your students to analyze.

2. Break the text into "documents" according to how you'd like to analyze it (documents are "segments of text" -- they can be paragraphs, chapters, books, speeches, etc.). Each document should be separated into its own text file.

3. **Either** teach students how to load the documents into the [Voyant Tools Home Page](https://voyant-tools.org/), **Or** upload the documents into the [Voyant Tools Home Page](https://voyant-tools.org/) yourself, then copy and distribute the URL of the visualization page that Voyant generates to your students. (Note that if you've already copied [this documentation repository](https://github.com/learn-static/writing-with-visualizations) to create a customized version of this learning sequence, you can replace the current button links in the [Voyant page](/content/digital-humanities/voyant.html) of this documentation site with your new links. Simply locate the three "button includes" on the page--which look like this: 
```
{% raw %}{% include button.html text="20th-Century State of the Union Addresses" link="https://voyant-tools.org/?corpus=3331b9ec3186b714ca53835d5b3ed722" color="success" %}{% endraw %}
```
--and replace the "text" and "link" values with your own).

4. If necessary, prepare a stopword list for students to upload to Voyant (or pre-load it to your Voyant instance). We recommend appending your stopwords to the [Buckley-Salton Stopword List](http://dhworkshop.pbworks.com/w/file/105416844/Buckley-Salton-stopword-list.txt){:target="_blank" rel="noopener"}.

5. Once students are viewing the requisite text in Voyant, they can proceed through this documentation's [Text Analysis with Voyant](/content/digital-humanities/voyant.html) and [Export an Image from Voyant](/content/digital-humanities/voyant-export.html) pages.