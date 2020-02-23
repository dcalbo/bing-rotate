# Little script to set wallpaper dynamically

Set wallpaper on desktop Gnome 3 and Cinnamon using the 'Picture of the day' from Bing, a.k.a. Windows 10.

## $xmlURL is needed to get the xml data from which the relative URL for the Bing pic of the day is extracted.

The format parameter determines what language gets the information. 
Valid values are: xml (XML), RSS (rss) and JSON (js).

The idx parameter determines where to start from. 0 is the current day, 1 the previous day, etc.

The mkt parameter determines which Bing market you would like to obtain your images from.
Valid values are: en-US, es-ES, zh-CN, ja-JP, en-AU, en-UK, de-DE, en-NZ, en-CA.

xmlURL="http://www.bing.com/HPImageArchive.aspx?format=xml&idx=0&n=1&mkt=en-EN"

## The desired Bing picture resolution to download

Valid options: "_1024x768" "_1280x720" "_1366x768" "_1920x1080" "_1920x1200"
If you wont Bing's watermark don't use 1920x1200.

## Check for a new image every hour

If you want to check for a new image every hour, you can configure crontab.

0 * * * * ~/path-to/bing-rotate.sh

Enjoy!!!