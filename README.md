These are scripts that can parse pubmed/medline  xml files into the format required by mallet.
There are two scripts: 

parse_medline_priya.py:
   usage: parse_medline_priya.py: 'mallet' 'pubmed_2013.xml' >> fileout ; where pubmed_2013.xml is the xml file. This prints out in utf-8 and then you can pipe it to a file 
# This script prints out title, abstract (if >100 ch) and keywords and only iff all three are present.

 
 
parse_pubmed_journal .py
usage: python parse_pubmed_journal.py 'mallet' 'pubmed.xml' >> fileout ; where pubmed.xml is the xml file. This prints out in utf-8 and then you can pipe it to a file 
This script print out pmids and journal names, but only iff abstract(>100 ch), title, and keywords are present. 

pubmed_2013.xml..: a rather large typical xml file from pubmed. These files can be obtained from pubmed using the 'save as' button on the main page.