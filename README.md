# video2pdfslides
# Description
This project converts a video presentation into a deck of pdf slides by capturing screenshots of unique frames

# Setup
pip install -r requirements.txt

# Steps to run the code
python video2pdfslides.py <video_path> -ask

it will capture screenshots of unique frames and save it output folder...once screenshots are captured the program is paused and the user is asked to manually verify the screenshots and delete any duplicate images (if -ask flag is used). Once this is done the program continues and creates a pdf out of the screenshots.

# More
The default parameters works for a typical video presentation. But if the video presentation has lots of animations, the default parametrs won't give a good results, you may notice duplicate/missing slides. Don't worry, you can make it work for any video presentation, even the ones with animations, you just need to fine tune and figure out the right set of parametrs, The 3 most important parameters that I would recommend to get play around is "MIN_PERCENT", "MAX_PERCENT", "FGBG_HISTORY". The description of these variables can be found in code comments.

# Original Developer contact info
kaushik jeyaraman: kaushikjjj@gmail.com
