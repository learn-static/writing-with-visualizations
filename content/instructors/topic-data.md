---
section: For Instructors
nav_order: 3
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

The stopword list used for the State of the Union Address topic modeling and analysis is the Buckley-Salton stopword list, retrieved from Alan Liu workshop at [http://dhworkshop.pbworks.com/w/file/105416844/Buckley-Salton-stopword-list.txt](http://dhworkshop.pbworks.com/w/file/105416844/Buckley-Salton-stopword-list.txt){:target="_blank" rel="noopener"}. 
The Buckley-Salton stopword list was also used for the Party Platforms, with the addition of three words: america, american, and americans.

Note that you can use any topic-modeling software in place of jsLDA to do your analysis.
Ultimately, your topic data just needs to be in the format specified below in order to generate topic graphs.

To prepare the demo corpus for topic modeling with [jsLDA](https://mimno.infosci.cornell.edu/jsLDA/){:target="_blank" rel="noopener"}, first format

```
id,date,text
1900-William-McKinley,1900,"Fourth Annual Message: To the Senate and House of Representatives: At the outgoing of the old and the incoming of the new century you begin the last session of the Fifty-sixth Congress with evidences on every hand of individual and national prosperity and with proof of the growing strength and increasing power for good of republican institutions. [See APP Note.] Your countrymen will join with you in felicitation that American liberty is more firmly established than ever before, and that love for it and the determination to preserve it are more universal than at any former period of our history. The Republic was never so strong, because never so strongly entrenched in the hearts of the people as now. The Constitution, with few amendments, exists as it left the hands of its authors. The additions which have been made to it proclaim larger freedom and more extended citizenship. Popular government has demonstrated in its one hundred and twenty-four years of trial here its stability and security, and its efficiency as the best instrument of national development and the best safeguard to human rights. When the Sixth Congress assembled in November, 1800, the population of the United States was 5,308,483.It is now 76,304,799. Then we had sixteen States. Now we have forty-five. Then our territory consisted Of 909,050 square miles. It is now 3,846,595 square miles. Education, religion, and morality have kept pace with our advancement in other directions, and while extending its power the Government has adhered to its foundation principles and abated none of them in dealing with our new peoples and possessions."
1901-Theodore-Roosevelt,1901,"First Annual Message: To the Senate and House of Representatives: The Congress assembles this year under the shadow of a great calamity. On the sixth of September, President McKinley was shot by an anarchist while attending the Pan-American Exposition at Buffalo, and died in that city on the fourteenth of that month. Of the last seven elected Presidents, he is the third who has been murdered, and the bare recital of this fact is sufficient to justify grave alarm among all loyal American citizens. Moreover, the circumstances of this, the third assassination of an American President, have a peculiarly sinister significance. Both President Lincoln and President Garfield were killed by assassins of types unfortunately not uncommon in history; President Lincoln falling a victim to the terrible passions aroused by four years of civil war, and President Garfield to the revengeful vanity of a disappointed office-seeker."
```

, we split each State of the Union Address and Party Platform into its own text file, then uploaded all of the State of the Union text files into one instance of Voyant, and all of the Party Platform text files into another instance of Voyant.
To view these text files, see the [/assets/data/state-of-the-union/txt/](https://github.com/learn-static/text-analysis/tree/main/assets/data/state-of-the-union/txt/) folder and [/assets/data/party-platforms/txt/](https://github.com/learn-static/text-analysis/tree/main/assets/data/party-platforms/txt/) folder in the project template's GitHub repository.

We then added links to these Voyant instances (one with State of the Union files and one with Party Platform files) to the documentation's [Voyant](/content/digital-humanities/voyant.html) page as buttons, so that students can link out to them easily.

As an alternative to pre-loading the text into Voyant, if time allows you could choose instead to teach students how to upload the requisite text files to the Voyant home page themselves.

## Prepare New Topic Data

1. Obtain and clean a body of text that you'd like your students to analyze.

2. Break the text into "documents" according to how you'd like to analyze it (documents are "segments of text" -- they can be paragraphs, chapters, books, speeches, etc.). Each document should be separated into its own text file.

3. **Either** teach students how to load the documents into the [Voyant Tools Home Page](https://voyant-tools.org/), **Or** upload the documents into the [Voyant Tools Home Page](https://voyant-tools.org/) yourself, then copy and distribute the URL of the visualization page that Voyant generates to your students. (Note that if you've already copied [this documentation repository](https://github.com/learn-static/writing-with-visualizations) to create a customized version of this learning sequence, you can replace the current button links in the [Voyant page](/content/digital-humanities/voyant.html) of this documentation site with your new links. Simply locate the three "button includes" on the page--which look like this: 
```
{% raw %}{% include button.html text="20th-Century State of the Union Addresses" link="https://voyant-tools.org/?corpus=3331b9ec3186b714ca53835d5b3ed722" color="success" %}{% endraw %}
```
--and replace the "text" and "link" values with your own).

4. Once they're viewing the requisite text in Voyant, students can proceed through this documentation's [Text Analysis with Voyant](/content/digital-humanities/voyant.html) and [Export an Image from Voyant](/content/digital-humanities/voyant-export.html) pages.