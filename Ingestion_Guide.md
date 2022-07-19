# Ingesting Files into HathiTrust
## Setup (on Mac)
**1. Connect to server where files are stored:** Go to Finder -> Connect to Server (⌘K), then browse or type name of server and click “Connect.” Click the + to save as favorite server. 

**2. Download ingestion script from Github:** Go to https://github.com/TempleDSS/SciFiCorpusOCR and download ZIP folder. You will need the hathi_ingest.py and tesseract.sh files for this process (the others are sample data/output). Save the needed files on your local machine (ex. on the Desktop). 

**3. Open a new terminal window (Command + Space Bar):** You will be running the ingestion script through the terminal. If you do not have Python 3 installed on your machine, make sure to do this before running the script. [Install Python here] (https://www.python.org/downloads/). 

## Setup (on Windows) 

`python [YOUR PATH HERE]/hathi_ingest.py [PATH TO 
**How the Code Works:** 
* python → calls python to run the selected script; you may need to use python3 depending on what version(s) of python are on your machine
* [YOUR PATH HERE]/hathi_ingest.py → points to location of the script to be run (replace [YOUR PATH HERE] with wherever you saved the ingestion script; ex. Desktop/hathi_ingest.py)
* afp://LIB-DSS-NAS._afpovertcp._tcp.local/Novel Database/Digitized Books/Sci-Fi Round 3 → Path to the files to be ingested
  * To get file path: Navigate to folder in Finder, hold down Control, click on the folder name/icon and while menu is open hold down the option key. An option will appear to “Copy [Folder Name] as File Path].” Select this and paste into terminal after script path
