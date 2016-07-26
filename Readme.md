# Dropbox Downloader

Small Python script which downloads a shared folder (shard url) from Dropbox. 
The download script is necessary if the folder contains too much content to download a zip file and if you 
do not have enought space in your own dropbox left to add the content to your personal dropbox. 
 
The script uses asyncio and aiohttp to make parallel downloads. The maximum number of concurrent downloads is 
limited by a semaphore. The default limit is 5.
 
 ## How to use the Script
1. Clone the repository via `git clone `
2. Install the requirements specified in `requirements.txt` via `pip install -r requirements.txt`
3. Adjust the constants `DROPBOX_URL` and `DESTINATION_FOLDER` in the script to match your requirements
4. Run the script `python dropbox_download.py`. You'll see a progress bar telling you the total number of files in that folder and how much already has been downloaded.  
