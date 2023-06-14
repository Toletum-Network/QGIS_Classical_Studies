This is a short hack to convert the data from EDCS into a CSV. 
Select the search result and paste into word. 

1.	Copy paste the selection from EDCS with formatting
2.	Replace “^l” with | 
3.	Replace “Publikation: “ with nothing, to delete
4.	Replace “Datierung: “ with nothing, to delete
5.	Replace “ bis ” with |
6.	Replace “         EDCS-ID: “ with |
7.	Replace “Provinz: “ with nothing to delete
8.	Replace “         Ort: ” with |
9.	Replace “Inschriftengattung / Personenstatus: “ with nothing to delete
10.	Replace “Material: ” with noting to delete
11.	Clean the EDCS conventions. Replace all:
“[6]” to “[- - - - -]”
“[3]” to “[- - -]”
“[3” to “[- - - “
“3]” to “ - - -]”
12.	Ctrl A  Ctrl X  Ctrl V without formatting. (This deletes the links and images)
13.	Enter the headers line: 
Reference|Date start|Date end|EDCS-ID|Provincia|Place|Text|Attributes|Material|Commentary
14.	Ctrl A  Ctrl C 
15.	open new excel sheet
16.	Ctrl V into field A1
17.	Open tab Data 
18.	Select Text to Columns
19.	Select Delimited and Next
20.	Check the box “Other” and enter |
21.	Next and finish to get the data into columns

**``Note!``**<br>As some inscriptions have more information than others there are columns with different types of data. When converting the rows and columns into a table we can order and curate the data.
