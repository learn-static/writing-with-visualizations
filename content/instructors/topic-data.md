---
section: For Instructors
nav_order: 3
title: Topic Modeling Data
---

This project can be applied to multiple disciplines, and implemented with or without the DH emphasis.
To this end, while the project template's topic modeling feature contains data intended for history students by default, this data can be supplemented or exchanged with whatever the instructor prefers.

**About the data used for this project:**

The State of the Union Addresses and Party Platforms used for the text analysis and topic modeling in this project template were obtained from the University of California Santa Barbara's [American Presidency Project](https://www.presidency.ucsb.edu/documents){:target="_blank" rel="noopener"}. 
This data can be found in multiple formats in the project template's GitHub repository in the [/assets/data/folder](https://github.com/learn-static/text-analysis/tree/main/assets/data){:target="_blank" rel="noopener"}.

Only Democratic and Republican parties were included in our 20th-century Party Platforms data.

Topic modeling was performed on these texts using the [jsLDA](https://mimno.infosci.cornell.edu/jsLDA/){:target="_blank" rel="noopener"} tool by David Mimno. Information on the number of iterations performed on each corpus can be found in the project template's GitHub repository at [_data/topic-data.csv](https://github.com/learn-static/text-analysis/blob/main/_data/topic-data.csv){:target="_blank" rel="noopener"} spreadsheet.

The stopword list used for the State of the Union Address topic modeling and analysis is the Buckley-Salton stopword list, retrieved from Alan Liu workshop at [http://dhworkshop.pbworks.com/w/file/105416844/Buckley-Salton-stopword-list.txt](http://dhworkshop.pbworks.com/w/file/105416844/Buckley-Salton-stopword-list.txt){:target="_blank" rel="noopener"}. The Buckley-Salton stopword list was also used for the Party Platforms, with the addition of three words: america, american, and americans.