# YRLS Scoring

Script to extract the information of the viting for YRLS

```
usage: YRLS_scoring.py [-h] [-url <URL>] [-csv <FILEE>] -t <FILE>
                       [-o <OUTPUT>] [-min <INT>]

     *            *               *                   *
*           *               *   *   *  *    **                *   *
  **     *    *   *  *     *                    *               *
|| __     _______  _       _____    _____                    
|| \ \   / /  __ \| |     / ____|  / ____|                   
||  \ \_/ /| |__) | |    | (___   | (___   ___ ___  _ __ ___ 
||   \   / |  _  /| |     \___ \   \___ \ / __/ _ \| '__/ _ \
||    | |  | | \ \| |____ ____) |  ____) | (_| (_) | | |  __/
||    |_|  |_|  \_\______|_____/  |_____/ \___\___/|_|  \___|                                                                                                                      
 *      *   * *     *   **         *   *  *           *
  *      *         *        *    *              *
             *                           *  *           *     *

optional arguments:
  -h, --help            show this help message and exit

General input dataset options:
  -url <URL>, --url_info_csv <URL>
                        Shared URL to the google spreandsheet with all the
                        registration and google form [if you don't provide the
                        csv file]
  -csv <FILEE>, --file_info_csv <FILEE>
                        CSV with all the registration and google form [if you
                        don't provide the url]
  -t <FILE>, --template <FILE>
                        Png file with the tamplate to use for the slide and
                        the page that will contain the winners
  -o <OUTPUT>, --output <OUTPUT>
                        Using <OUTPUT> for output files (default: template
                        folder)
  -min <INT>, --minimum_votes <INT>
                        Minimal number of vote to stay in the competition
```

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

