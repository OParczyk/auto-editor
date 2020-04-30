# auto-editor
Easily remove the boring parts of the video.

auto-editor is a tool that can find the silent (boring) parts of the video and cut or speed them up. 
It works by using ffmpeg to split the video up into the audio and the frames. Calculates the new audio and adds and drops frames where needed, and stiches that back into a video.

This project is a fork of Carykh's inactive [jumpcutter](https://github.com/carykh/jumpcutter). This project seeks to fix the issues (and design flaws) of the original while still following the same general idea.

# Usage
Using auto-editor with its default parameters.

``` python3 auto-editor.py example.mp4```

Download a video in a URL and remove the boring parts.

``` python3 auto-editor.py "https://www.youtube.com/watch?v=kcs82HnguGc"```

speed up a lecture with Carykh's procrastinator settings.

``` python3 auto-editor.py "https://www.youtube.com/watch?v=_PwhiWxHK8o" --video_speed=1.8 --silent_speed=8```

get help on any of the other parameters

``` pythnon3 auto-editor.py --help```

# Download the Libraries and Dependencies
This program is written in Python. Check if you have Python 3 by running.

``` python3 --version```

if the terminal says ```command not found: python3``` you need to get Python 3 https://www.python.org/downloads/ and install Python 3.

> Note: if you installed Python 3 but the terminal still won't recognize python3, try python --version and see if that has the right version. If it does, then you need to remove the 3 for all of the commands

Check if you have Homebrew.

``` brew --version```

If not then go to https://brew.sh and install Homebrew.

To install all of the needed dependencies, paste this to your terminal.
``` 
brew update
brew install ffmpeg
brew install youtube-dl
python3 -m pip install --upgrade pip
python3 -m pip install scipy audiotsm opencv-python
```
> Note: Be warned that ffmpeg can take up to 15 minutes to install if you do not already have it.
# Installation

Click 'Clone or Download' then 'Download ZIP'. You should see the file being downloaded. 

Go to your download location and move it to your Home directory (your username). 

Open the ZIP file, then go to your terminal and run ```cd auto-editor-master```. This will take you where auto-editor is.

Run  ``` python3 auto-editor.py --help``` to make sure terminal can find the file.

If it runs successfully, then congratulations, you have installed auto-editor. See usage to see more examples.

If it didn't run successfully or if you have any other suggestions or concerns, then feel free to create a new issue on this page.

Visit jumpcutter's [official discord.](https://discord.gg/2snkzhy)