---
section: For Instructors
nav_order: 4
title: Topic Modeling Data
---

This project can be applied to multiple disciplines, and implemented with or without the DH emphasis.
To this end, while the project template's topic modeling feature contains data intended for history students by default, this data can be supplemented or exchanged with whatever the instructor prefers.

**About the data used for this project:**

The State of the Union Addresses and Party Platforms used for the text analysis and topic modeling in this project template were obtained from the University of California Santa Barbara's [American Presidency Project](https://www.presidency.ucsb.edu/documents){:target="_blank" rel="noopener"}. 
This data can be found in multiple formats in the project template's GitHub repository in the [/assets/data/](https://github.com/learn-static/text-analysis/tree/main/assets/data){:target="_blank" rel="noopener"} folder.

Only Democratic and Republican parties were included in our 20th-century Party Platforms data.

Topic modeling was performed on our demo corpus using the [jsLDA](https://mimno.infosci.cornell.edu/jsLDA/){:target="_blank" rel="noopener"} tool by David Mimno. 
Information on the number of iterations performed on each corpus can be found in the project template's GitHub repository at [_data/topic-data.csv](https://github.com/learn-static/text-analysis/blob/main/_data/topic-data.csv){:target="_blank" rel="noopener"} spreadsheet.

The stopword list used for the State of the Union Address and Party Platform topic modeling is the Buckley-Salton stopword list, retrieved from Alan Liu's workshop at [http://dhworkshop.pbworks.com/w/file/105416844/Buckley-Salton-stopword-list.txt](http://dhworkshop.pbworks.com/w/file/105416844/Buckley-Salton-stopword-list.txt){:target="_blank" rel="noopener"}. 
The Buckley-Salton stopword list was also used for the Party Platforms, with the addition of three words: america, american, and americans.

---

## Prepare New Topic Data

**Formatting Topic Data**

When formatted topic data is added to the project template `/_data/topics/` and `/_data/documents/` folders, the Writing with Visualizations project template will automatically generate line graphs that show the percentage of each topic across all documents.

You will need to upload:

**A "Topic" CSV**

A CSV containing values for the fields topic, tokencount, words, and topicname:

The first row should contain field names, like so: `topic,tokencount,words,topicname`.
Following rows should contain the following information in each column:

- `topic`: a number assigned by the topic modeling software to a particular cluster of words
- `tokencount`: the number of times the words in this topic appear in the corpus
- `words`: a set of words that the topic modeling software clustered together into a topic
- `topicname`: a name assigned to the topic by you or your students.

Example:

```
topic,tokencount,words,topicname
0,45231,"law country made government service navy commerce officers proper duty",
1,25734,"men great man business power public good work labor conditions",labor in America
2,31823,"states united department year foreign court secretary trade canal commission",
```

Upload this topic CSV to your project template repository's `/_data/topics/` folder.

**A "Document" CSV**

Next, you will need to upload a CSV containing data on how often a topic appears in each document.

The field names of this spreadsheet should be `id,0,1,2,3,4,5,6,7,8,9`, where id is the document's id and the topic numbers 0-9 correspond to the values of the topic field in "Topics" CSV (the one you just created in the previous step).
You can use more than 10 topics if you'd like.
We've used 10 for demo purposes.

Below the field names, each row begins with a document id, followed by the percentage that each column's topic appears in the document.

Example:

```
id,0,1,2,3,4,5,6,7,8,9
1900-William-McKinley,0.12146954,0.024239801,0.14792771,0.0016773077,0.064062331,0.058327021,0.010280273,0.0019478411,0.002326588,0.023969267
1901-Theodore-Roosevelt,0.12079876,0.099325726,0.03003112,0.0046680498,0.042738589,0.067997925,0.017064315,0.0038381743,0,0.032105809
```

Upload this topic CSV to your project template repository's `/_data/documents/` folder.

**Topic Modeling**

You can use any topic-modeling software to do your analysis.
You'll just need to format your topic data output in the format specified above in order for the site to generate topic graphs.

---

## Topic Modeling with jsLDA

[jsLDA](https://mimno.infosci.cornell.edu/jsLDA/){:target="_blank" rel="noopener"} provides a light-weight option for topic modeling in-browser, without requiring any software installation. 

To prepare your corpus for topic modeling with jsLDA, create a TSV (tab-separated values) file that contains each document as a row, formatted like this:

`[doc ID] [tab] [label] [tab] [text...]`

In the example below, the document's filename is used for the "doc ID" value, and the date is used as the "label" value:

```
1900-William-McKinley	1900	"Fourth Annual Message: To the Senate and House of Representatives: At the outgoing of the old and the incoming of the new century you begin the last session of the Fifty-sixth Congress with evidences on every hand of individual and national prosperity and with proof of the growing strength and increasing power for good of republican institutions."
1901-Theodore-Roosevelt	1901	"First Annual Message: To the Senate and House of Representatives: The Congress assembles this year under the shadow of a great calamity. On the sixth of September, President McKinley was shot by an anarchist while attending the Pan-American Exposition at Buffalo, and died in that city on the fourteenth of that month."
```

Note that there is no row containing field names.

When your TSV is formatted, go to [jsLDA](https://mimno.infosci.cornell.edu/jsLDA/){:target="_blank" rel="noopener"} and follow these steps:

1. Click the "Run a model" button.

2. On the right side of the webpage, look for the "Use a different collection" box, in grey. 

3. Click the "Browse" button to the right of "Documents."

4. Upload your prepared TSV.

5. If using a stopword list,  Click the "Browse" button to the right of "Stoplist," and upload your stopword list.

6. Click the "Upload" button.

8. In the top right of the webpage, adjust the amount of topics you'd like to output (default is 25).

7. In the top left of the webpage, click the "Run 50 iterations" button. Topic numbers and words will display on the left side of the window, and previews of the documents with the highest topic weight will display in the middle of the window. Click on various topics to see their associated previews. 

8. Click the "Run 50 iterations" button as many times as needed to complete your desired number of iterations. Note: see the [_data/topic-data.csv](https://github.com/learn-static/text-analysis/blob/main/_data/topic-data.csv){:target="_blank" rel="noopener"} spreadsheet in the project template's GitHub repository for information on number of topics and iterations used for the demo data. 

9. When ready to download, click the "Downloads" button in the top right of the webpage, then select "Document topics" and "Topic summaries" to export both files. "Topic summaries" will become the file you add to your repository's `/_data/topics/` folder, while "Document topics" will become the file you add to your repository's `/_data/documents/` folder, but first you'll need to make the following edits.

10. Edit the first row of the "Topic summaries" file to be `topic,tokencount,words,topicname`.

11. Add a row to the top of the "Document topics" file, and add to this row the field names `id,0,1,2,3,4,5,6,7,8,9...`, where the numbers correspond to the topic numbers in the "Topic summaries" file.

12. Rename both files, then deposit the topics file in the project repository's `/_data/topics/` folder, and the documents file in the `/_data/documents/` folder.