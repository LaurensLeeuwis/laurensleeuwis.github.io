# State of the apps 2019

I've been using a MacBook Air at home to browse and code a bit while chilling on the couch for about 4 years now. After switching jobs I'm now using on a MacBook Pro at work. I had to step up my game, having developed on a Windows machine for 7 years. 

This is a list of the applications I've installed on my Mac. Very useful as reference for myself once I need to reinstall all of it. Could be useful for you as well, just like the inspiration for this - [State of the apps 2018 by jqno](https://jqno.nl/post/2018/10/07/state-of-the-apps/) - was very very very useful for me ;)

## Development

- [Jetbrains Toolbox](https://www.jetbrains.com/toolbox/) is a nice tool to install IntelliJ IDEA. If new versions comes out it's very easy to update, and it gives me a nice menu in the toolbar which makes it convenient to open recent projects. Also useful when trying a new experimental IntelliJ version, because it can easily install multiple versions at the same machine.
	- [IntelliJ IDEA Ultimate](https://www.jetbrains.com/idea) is my IDE of choice. I've used it for many years and feel most productive using it.
	    - [Presentation Assistant Plugin](https://plugins.jetbrains.com/plugin/7345-presentation-assistant) I always have this plugin enabled. It shows me which shortcuts I could've used instead of using my mouse. It is also useful during presentations and extreme programming; the audience can follow what keys you've pressed. Also, it gives me quick feedback that I actually used the intended shortcut ;)
	    - [FiraCode](https://github.com/tonsky/FiraCode) my font of choice. I enabled the ligatures as well, which gives me amazing `=>` and `!=`'s.
	    - I disabled tabs. I use CMD+E [a lot](https://twitter.com/LaurensLeeuwis/status/701779865813524480).
	    - Solarized (light) theme (can't remember whether I used [this](https://github.com/jkaving/intellij-colors-solarized) or [this](https://github.com/4lex4/intellij-platform-solarized)). Because I was using the solarized theme for iTerm (see later on) I use the solarized (light) theme for IntelliJ as well. Of course I'm using the same shell (zsh) inside and outside of IntelliJ.
	    - [BashSupport plugin](https://plugins.jetbrains.com/plugin/4230-bashsupport) for Bash support
	    - [My Bricks background](./achtergrond%20witte%20bakstenen.jpg) as the editor background (repetitive). Yeah. Weird?
- [iTerm2](https://www.iterm2.com/). While the default _Terminal_ was fine for my hobby projects, it was time for something more serious.
	- I use _zsh_ as my shell, _Meslo_ as a font, _Powerlevel9k_ and _Oh My Zsh_ as well. I actually don't have too much experience with all of this, but I quite like it so far. I followed the installation guide [here](https://gist.github.com/kevin-smets/8568070). Because I'm using Docker, I enabled the autocomplete for that.
- [Brew](https://brew.sh/) to easily install some tools
	- `zsh` including `zsh-autosuggestions` and `zsh-syntax-highlighting`. Don't know if I'm actually using the last two, since I installed the whole Meslo/Powerlevel9k/OhMyZsh afterwards (see above).
	- `git` for obvious reasons. The latest version, so not the old version which is installed by default on MacOS
	- `git-lfs` because we have some repositories at work which make use of the large file storage capabilities.
	- `bat` which is like `cat`, but with syntax highlighting.
	- `node` nodeJS (which includes `npm` as well).
	- `jenv` to easily switch JDK's ([jenv](https://www.jenv.be/))
	- `wireshark` via `brew cask install wireshark`
- [Docker](https://hub.docker.com/editions/community/docker-ce-desktop-mac). ([Docker Docker Docker!](https://youtu.be/5JMK8vaGxyI?list=PLpQuPreMkT6ArrW7WOI5PhQhBMQNGfPXr&t=95)) I tried installing this via brew, but weirdly that didn't really work. Installed it via the `.dmg`.
- [Insomnia](https://insomnia.rest/) is a tool like Postman; making it easy to make API requests. I like Insomnia a bit better than Postman. Installed it via the brew cask.
- [VirtualBox](https://www.virtualbox.org/wiki/Downloads) to run VM's. I had to enable installing software from developer _Oracle America, Inc._ in the security and privacy settings of MacOS before I was able to install it.
	- [IE and Edge VM's](https://developer.microsoft.com/en-us/microsoft-edge/tools/vms/) are the things I mostly run on VirtualBox. Yeah, living the IE11 dream!
- [ChromeDriver](http://chromedriver.chromium.org/) to let Selenium speak Chrome
- Java
	- First I installed AdoptOpenJDK 8 (Hotspot) via [a brew cask](https://github.com/AdoptOpenJDK/homebrew-openjdk). This is my default java. Unfortunately some things (jars for work using some _@rpath/libfreetype.6.dylib_ (swing?) which it couldn't find) didn't work correctly. Furtunately an update fixed this.
	-  [Oracle JDK 8](https://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html) which I use to run that particular jar.
- [Vue CLI](https://cli.vuejs.org/) to help developing Vue apps. Currently this is the only npm package I've installed globally. Probably more will follow.

Is that it? Yeah. No Maven or Gradle yet. These will probably follow later when I actually need to have them installed globally. For now, `gradlew` and `mvnw` do their thing just fine.

## Tools

- [MacPass](https://macpassapp.org/) to save and generate all my passwords. My go-to 'KeePass compatible' app for the Mac. I use KeePass itself on my Windows machines and [KeePass Touch](https://itunes.apple.com/nl/app/keepass-touch/id966759076) on my iOS device. What I like about KeePass is that I feel that I'm in control over my secret stuff. No company (which can be hacked) keeping track of my passwords.
- [Dropbox](https://www.dropbox.com/downloading) to sync my KeePass database between machines. Integrates nicely with the _KeePass Touch_ app for iOS.
- [STACK](https://www.transip.nl/stack/) as my cloud storage. I like that it's hosted in the Netherlands, and I got 1TB of free storage.
- [VLC](https://www.videolan.org/) it was a week at my new job before I received my first `.wmv` video. VLC is a nice tool to play all media with.
- [Scroll reverser](https://pilotmoon.com/scrollreverser/). Usually I use my MacBook with an external (Windows) keyboard, external monitor and external mouse. I like to have my scroll wheel on my mouse work like I'm used to (the Windows default, what MacOS calls not natural) and my touchpad like I'm used to as well (what MacOS calls natural). Scroll reverser lets me actually set this up like I want to.
- [Aerial screensaver](https://github.com/JohnCoates/Aerial) as mentioned before I use my MacBook with an external monitor. If I lock my MacBook, the external screen will go into sleep. It doesn't wake up correctly without switching it on and off again. Bummer. Therefore I always lock it with a screensaver; that way the external monitor won't sleep. I really like the Aerial screensaver, which often shows Hong Kong where I have some fond memories of ;). I also set up a hot-corner to easily put my machine on screensaver mode.
- [Magnet](https://magnet.crowdcafe.com) which adds hotkeys for me to put the windows where I want them. 
- [Alfred](https://www.alfredapp.com/) which is a powerful replacement for Spotlight. I'm just getting started with this tool, there is a lot to learn I think :)
- [OBS Studio](https://obsproject.com/) which lets me record my screen. While CMD+SHIFT+5 can do something like that as well, this tool is more powerful.
- [Soundflower](https://github.com/mattingalls/Soundflower) is a tool which redirects a sound output ('speaker') to a sound input ('microphone'). Enabling me to record the screen sound in OBS.
- [The Unarchiver](https://theunarchiver.com/) to extract RAR files, etc.


## Office, web text


- [MacDown](https://macdown.uranusjr.com/) to write markdown. I wrote this post using it.
- [Sublime Text](https://www.sublimetext.com/) to write all kinds of files. Actually I would really like to have [Notepad++](https://notepad-plus-plus.org/) back, but that is Windows only.
- [Google Chrome](https://www.google.com/chrome/) is my browser of choice. It syncs my history, bookmarks and some passwords between devices as well. I also know my way around in the developer tools, more than those of the other browsers.
- [GIMP](https://www.gimp.org/). A long long time ago I've used Adobe Photoshop to edit images. GIMP is quite similar (for my usage), but free. I sometimes use it to give images some effects when using them in presentations and stuff. Cropping screenshots is a thing I don't do as much as I did before because of the magic CMD+SHIFT+5 tooling in MacOS.
- Microsoft Office. My company uses Office, which I've always used in school, university and at work before as well. I know my way around in Outlook, Word, Excel, Powerpoint and Skype. Because I'm productive in these tools I quite like them as well. I removed Pages, Keynote and Numbers from my machine because they feel obsolete. Actually I have a license for Office at home as well (thanks [HUP](https://www.microsofthup.com)).
- Of course I have installed some company stuff as well, like Cisco AnyConnect, Sophos Endpoint, etc. etc.


## Things I still miss from my Windows era

- [Notepad++](https://notepad-plus-plus.org/) was amazing. Especially that you didn't have to save files when closing the application. And they were still there once you reopened the app! I will try [Sublime Text](https://www.sublimetext.com/) for now.
- [Workrave](http://www.workrave.org/)/[Workpace](http://www.workpace.com/workpace/about/what-is-workpace/). This helps preventing RSI. While I generally don't like to be disturbed by microbreaks, I dislike it even more when my back or wrist hurts. I tried [Stretchly](https://hovancik.net/stretchly/) and [TimeOut](https://www.dejal.com/timeout/) but I didn't like those. Especially that they didn't reset their times when I took a break on my own.

