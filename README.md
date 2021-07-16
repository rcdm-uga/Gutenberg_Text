# Gutenburg_Text
Downloads from Project Gutenberg

This collection of text was pulled from Project Gutenberg's [Top 100 Authors Yesterday](https://www.gutenberg.org/browse/scores/top#authors-last1). Only the text in English were pulled if other languages were present. Indexes were deleted. This list changes frequently on project gutenberg's website, so this list will not be the same as what it is currently. 

These were pulled using this [python package](https://github.com/c-w/Gutenberg) since they made it very easy to pull the ebooks from them. Since pulling from Project Gutenberg required some specfic installs, virtual enviornments are best if using this library. 


### Issues
There are some current issues with this specific dataset, listed [here](https://github.com/DigiUGA/Gutenberg_Text/issues/1). Take a look and see for yourself, and feel free to add if there are any more spotted. 

### Dataset (1.7Gigabytes)

There are 98 authors in this dataset, two were just directories of indexes. Each containing a different amount of txt files. **Each txt file has a header and footer added by Project Gutenberg.** Thus will needed to be removed when doing any type of analysis. 
  * authors.xls: a spreadsheet of meta data about each author. Some authors have a accent marks in their names and some programs overide the encoding of a csv. The encoding holds in .xls (Excel Format). Python and R can read excel files just as they can csv files. 
    * `Name`: `str` The author's name
    * `Nationality`: `str` The authors nationality
    * `Gender`: `str` The author's gender
    * `genre`: `str` the genre the author belongs in
      * These are broad categories about the authors
    * `original language`: `str` the language the authors original language
      * If not Engligh, then the text was translated from that orginal language

*******
If you are looking for some types of ideas on analyzing text, check out our web [tutorials](https://digi.uga.edu/text-analysis/). 

