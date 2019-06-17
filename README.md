# Veditor
HTML Based simple video editing

This is primarily intended as a simple tool to allow parents to produce more child friendly versions of a video, or simply to skip the boring bits.

## Installation
Download the zip file from Github, and unzip into the folder of your choice, and open *veditor.html* in a browser.

## Use ##
Locate a video file (strongly recommend from your local files) and paste into the Video Url box, then hit "Load Video".

*A fully qualified video URL will look like file:///C:/td/veditor/Media/The%20Incredibles.mp4*

A video should then load and start playing.

Use **In Mark** and **Out Mark** to select a section of the video. Use **Skip** or **Mute** to the script box.

Check the **Enable Skip Play** box to enable replay with skips and mutes.

Due to security limitations of Javascript, there is no easy way to offer file selection. However, if you copy the videos you want to edit
into the *Media* subfolder, you can view a list with the *Media* button, and use *Copy link Address* to copy and paste the URL.


## Saving/Loading scripts ##
Again due to limitations with Javascript, there is not reliable way to save to reload your script automatically. However, you can use copy and paste
to save your script to a text file. To reload the script, paste the script back into the script box and hit **Load Script**.

You can also manually edit the script: Remember to hit **Load Script** to pick up changes.

Sample Script:
```
Url: file:///C:/td/veditor/Media/The%20Incredibles.mp4
Skip: 00:00:00.00 - 00:03:33.00
Mute: 00:03:44.37 - 00:03:44.58
Skip: 00:03:57.72 - 00:05:09.44
```

## Times ##
Times are displayed as hours:minutes:seconds.100th . The **<** and **>** will advance or go back 1/25th of a second, approximate one frame. There is no standard way of retrieve framerate from a video in Javascript.

## Full Screen ##
Hitting the full screen control on the video player with play the video in full screen, and if **Enable Skip Play** is on, the edited video will play.


