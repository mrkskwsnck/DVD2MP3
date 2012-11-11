DVD2MP3

Description

Dumping the audio stream of DVD chapters into MP3 files.


Preamble

I own a lot DVDs of concerts and I like to listen to music very much. Also I’m proud doing it using my iPhone for which I need to use iTunes. But it seems there is no way to import just the audio stream from a DVD while considering the chapters into the iTunes library from the scratch. — The only solution seems to buying a software which can do this for me? But no, I for sure can do this by myself!

Anyway I didn’t know how to start. Googling the web I found another project with a similar goal from “Jim Crumley” at SourceForge. His solution is written in the most awesome language Perl as command line program for the terminal. But I wanted something more interactive. So as proud Mac user I decided to develop my solution using the AppleScript automation capabilities.


Usage

Save the AppleScript using the AppleScript Editor in the application file format. The icon will become a droplet. Next mount your DVD so it will appear on your desktop. Now drag the DVD icon using your mouse onto the droplet and release the mouse button. It will begin to examine the DVD and you will be prompted to choose one DVD track you want to dump. Once you confirm the selection the process can take a while. — Remember there is no progress indicator.


Known issues

Some DVDs with copy protection won’t work using this droplet. A workaround is to use this droplet in combination with the “Fairmount” and “VideoLAN Client media player” software. Where VLC provides the libdvdcss library Fairmount can use it to mount the copy protected DVD removing the protection temporarily.


Dependencies

In order to use this droplet you need to install some additional software: First of all an AppleScript scripting addition from “Late Night Software” which extends AppleScripts capabilities for parsing XML data must be installed. Using MacPorts package manager there are two further packages which need to be installed. The first one is lsdvd which helps retrieving any information from a given DVD. The second package is MPlayer which brings two further tools: mencoder for encoding the DVD stream and mplayer for dumping the audio stream. Anyway both MacPorts packages depend on another packages wich will be installed, too.


Related internet resources

• http://sourceforge.net/projects/dvd2mp3/
• http://www.latenightsw.com/freeware/XMLTools2/index.html
• http://www.macports.org/
• http://www.metakine.com/products/fairmount/
• http://download.videolan.org/pub/videolan/vlc/1.1.9/


-- Markus Kwaśnicki