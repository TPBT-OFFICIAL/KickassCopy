KickassCopy - A project for Liberty
===================================

KickassCopy is a collection of short programs (often written in C++) that helps to mirror torrent files and magnet links from Websites.
I made this project primary to save all that amazing torrents because never knows how long there will be in the internet and secondly for the openbay project because I don't like their official Database because it's too small for me.
Important to know is that I start with this project 2 days after the December 2014 Raid against PirateBay and not after I heard of the openbay project. I don't write all this code to support illegal torrent downloads. I do it for a freedom Internet.

Please creating issues if you find a bug or a misspelling, have any questions, this to discuss, needing help by using my program, don't understand some code, have some technical questions, want to talk with me over skype, have a god Idea, don't be sure if you should do a thing for this protect, needs my help by anything else that have to do with computers (I make free Support),...

Pull requests are welcome but the code is in a very high churn state and may not be accepted, so ask before taking on anything big. Contributions are awesome but the focus of the developers is on writing new code, not teaching programming. If you understand over 60% of the code you are probably good enough to send Pull requests.

## Fautures
* Getting live Database updates by using RSS feeds from famous Torrent sites. Be using this cool PHP tool
* Creating Download lists for HTTrack
* Brut force search downloading (uses much CPU on the Sphinx Server if you are not careful with this the other site can go down, banned you or installing an anti DDOS tool)
* Reading the maximal amount of Search results Sites from the first opage of every bruteforce result and make a list with every existing site for HTTrack. This requires a copy of one site of every brute.
* Convert the downloaded HTML files into a importable, with MySQL compatible, CSV file or in a magnet/torcache link list
* Dublicate filter ro remove equal torrent search result (ca. 50% if you make the brute force thing)
* Converter from dalydumps (Torrent api) into importable CSV files.
* A lot of useful tools to convert, split and edit raw data, csv files and HTTrack download list. I recommend not downloading more than 999999 in one step because if you do you have to remove the HTTrack max links limit in the settings and also the ban change is higher if you download that much in one step. Try always to get the best download speed by using more connections and a high download rate but try not to slowdown the server and think that only if you are quiet they couldn’t see what you are doing an so they don’t ip-ban you.
* Some notes with useful MySQL commands. Thay not have any order. I wrote it nearly randomly into different files but you will maybe find what you want.

## Building
What do you use?
- A windows PC or if you want to use Linux/Mac and time for debugging
- A C++ Compiler like MinGW
- An IDE I'm using Code::Blocks

I made this step very easy. You don't have to do anything then to open the main cpp file of the subproject in your favourite IDE. I don't use any header or make files and very seldom non-standard libraries to make this step as easy as I can. If you want you can also use Code::Blocks you only have to open the CodeBlocks project and it will work.

## Contributors Wanted!
Have some spare time, know medium C++, and want to help me?
Contribute! There's a ton of work that needs to be done. And a lot of it makes fun and is very interesting.


## Code design
I don't care a lot about the code design but here some things you should know:
- Try to normally use if blocks except you only have a one short command that isn't in a else if or else block and you can be sure that it doesn't make sense  to add a second line to that if conditional in the future like if(i==5) break;
- Try to use the same indent and indentation rules as I used.
- Comments difficult or technical important lines. Over or after the command on the same line. For longer text use multiline commends characters.
- Make some empty line if it needs, to make the code more clear.
- Try to use only standard cross-platform libraries and wrote the header file after the #include commands to make the building process as easy as you can.
- I prefer static libraries because dynamic always often problems but the best thing is still to use the standard ones.
- Don't upload big useless text, csv or log files to GitHub because then they spam the changed files site. If you have such date delete it before sending me a pull request or make a 7zip (use LAZMA2) if the files are important or useful for others. But look that the files don't are too big.


## FAQ
### Can I get an exe?
**Yes**. I am always releasing binaries for Windows.
If you get some dll error you will find the missing file in 1min by using google. Maybe I posted it already on GitHub.
For Linux you have to compile it by our own but I think if you use Linux you should know the make command. Look below for more information about other operating systems.

### Have you removed any illegal/copyrighted file before the final release and what I I find something?
No and I didn't removed anything yet. I don't feel responsible which info hashes I downloaded from the websites. The DB contains no Torrent, Magnet Links or any copyrighted file. It contains only names and hashes and other information that aren’t copyrighted. If there see some very illegal files like child porn then you should report this by opening an issue and I'll probably remove this in the next release because I don’t want to support such things. Probably I’ll make a list with the removed data. I can’t change anything of released torrent files because that’s technical not possible. The best thing is to report the material on the sites that using the released Databases or the site from witch I downloaded the hashes because also if I would remove your material a lot of sites wouldn't download my updates. I need the same information like http://bitsnoop.com/info/dmca.html to remove something.

### What about Linux/OSX?
The project is designed to be cross-platform but probably it uses some windows specific command that you have to change that into the Linux one or cross-platform ones because I never tested it on other operating systems. If you find please make it per #if when it is operating system specific and sent me a pull request.

### Hey I'm going to go modify every file in the project, ok?
I welcome contributions, but please try to understand that I cannot accept
changes that radically alter the structure or content of the code, especially
if they are aesthetic and even more so if they are from someone who has not
contributed before. This may seem like common sense, but apparently it isn't.
If a pull request of this nature is denied that doesn't necessarily mean your
help is not wanted, just that it may need to be more carefully applied.


## Known Issues
### The Duplicate checker don't remove every duplicate
There are some fief duplicates in the finally file of the kickass2MySQL program but is doesn't matter because if you set the hash column to unique then MySQL will remove this automatically but if I or somebody else have time it's maybe something to do.

This readme partially based on based https://github.com/benvanik/xenia/edit/master/README.md because I like this one.
