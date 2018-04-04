# YRLS Scoring

Script to extract the information of the viting for YRLS

Dependencies :
--------------

- Python 3.6
   - Imageio 2.3.0
   - Seaborn 0.8.1
   - Matplotlib 2.2.2
   - Pandas 0.22.0
   - Request 2.18.4

Format input file
-----------------
The file is a comma separated file with the following columns :  

Spreadsheet_name,Speadsheet_url,Number_people,Number_talk,Names_talk,Number_poster,Names_poster

And at the first row the link to the registration spreadsheet and the following are the information about the spreadsheet for the votes

The comments begin with **#**  

Format URL
----------

The URL need to be shared google spreadsheet URL that look like that :

`https://docs.google.com/spreadsheets/d/[GOOGLE SPREADSHEET ID]`

