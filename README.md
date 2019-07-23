![stability-wip](https://bitbucket.org/repo/ekyaeEE/images/3847436881-internal_use_stable.png)
![status-archived](https://bitbucket.org/repo/ekyaeEE/images/3278295154-status_archived.png)
![issues-closed](https://bitbucket.org/repo/ekyaeEE/images/1555006384-issues_closed.png)

# RATIONALE #

* An internal & must-do-mandatory-project since a lots of links collected and curated across times and devices generated a mountain of links with a plethora of tags. Since [Del.icio.us](https://del.icio.us/) was [sold twice!](https://dealbook.nytimes.com/2014/05/08/delicious-social-site-is-sold-by-youtube-founders/?mtrref=www.google.com&gwh=66EB03E0A8E0CDB06A837C01ABFF41CE&gwt=pay), we do not had another choice /B plan. This is the result of different tools applied with some collateral damages and some discoveries on the digital road.
* ~~This repo is a living document that will grow and adapt over time~~

### What is this repository for? ###

* Quick summary
    - Migration of bookmarks (and internal tags) to [Evernote](https://www.evernote.com/) (mainly from the _almost defunct_ [Del.icio.us](https://del.icio.us/)
* Version 1.01

### How do I get set up? ###

#### The easy way to export data ####
* Log in to your [Del.icio.us](https://del.icio.us/) account (_fingers crossed!_)
* Then go to `Profile` (upper right corner) > `Settings` > `Export` tab. Tick `Include My Tags` and `Include My Notes`. `Export` your bookmarks as `html` format
![exporting.png](https://bitbucket.org/repo/4pyror9/images/2603006681-delicious.png)
* The `export.html` can be clean out with:
	- clean up:
		- [Beautiful Soap](https://www.crummy.com/software/BeautifulSoup/)
		- [HTMLCleaner](http://htmlcleaner.sourceforge.net/index.php)
		- [html5lib](https://github.com/html5lib/html5lib-python)
		- [AdvancedHTMLParser](https://github.com/kata198/AdvancedHTMLParser)
	- exporting:
		- to a myriad of format via [Pandoc](https://pandoc.org/)
* Convert your `export.html` to an Evernote XML file. More data can be found [here](https://evernote.com/blog/how-evernotes-xml-export-format-works/) and [there](https://help.evernote.com/hc/en-us/articles/208314308-How-to-import-from-other-note-apps-into-Evernote)

#### Another way to export and import data ####
* Log in to your [Del.icio.us](https://del.icio.us/) account (_fingers crossed!_)
* Then go to `Profile` (upper right corner) > `Settings` > `Export` tab. Tick `Include My Tags` and `Include My Notes`. `Export` your bookmarks as `html` format. Save it.
* Open the `export.html` in your internet browser, ie.: Google Chrome
	- In Chrome (Mac) navigate to `View` and then click on `Developer` and then `View Source`. You also can right click and select `View Page Source`. The keyboard shortcut is `Option` + `Command` + `U`. 
	- In Chrome (PC) press `CTRL` + `U`. Or you can click on the weird-looking key with three horizontal lines in the upper right hand corner. Then click on `Tools` and select `View Source`.
* Select all the code. (ie.: Google Chrome > `Edit` > `Select all`)
* Go to http://jsfiddle.net/kT4nj/ 
* Go to section `Paste html here here`. Paste the code.
* Click on `Parse to Evernote XML`. Inside this box, again select all the code parsed (ie.: Google Chrome > `Edit` > `Select all`).
* Open TextEdit (mac) / WordPad (Windows). Create a brand new file. Paste the parsed data. Save as `exported.enex`
* Go to Evernote and [download](https://evernote.com/download) the app according to your operating system. Install it. Log in with your account. 
* Once opened go to `File` > `Import notes`. Select the previously exported file named & saved `exported.enex`

#### Evernote exporting ####
* Evernote recently made [controversial changes](https://techcrunch.com/2016/12/14/evernotes-new-privacy-policy-allows-employees-to-read-your-notes/) to their privacy policy that allows employees to read user notes. So we need a _B-plan_: Download [Standard Notes](https://standardnotes.org/) according your ~~operating system~~ device. Then follow this [guidelines](https://dashboard.standardnotes.org/tools)

### Source ###

* ~~Check them on [here](https://bitbucket.org/imhicihu/migration-bookmarks-to-evernote/src)~~

### Issues ###

* ~~Check them on [here](https://bitbucket.org/imhicihu/migration-bookmarks-to-evernote/issues)~~

### Changelog ###

* Please check the [Commits](https://bitbucket.org/imhicihu/migration-bookmarks-to-evernote/commits/) section for the current status

### Who do I talk to? ###

* Repo owner or admin
    - Contact `imhicihu` at `gmail` dot `com`
* Other community or team contact
    - Contact is _enable_ on the [board](https://bitbucket.org/imhicihu/migration-bookmarks-to-evernote/addon/trello/trello-board) of this repo. (You need a [Trello](https://trello.com/) account)


### Legal ###

* All trademarks are the property of their respective owners.

### License ###

* The content of this project itself is licensed under the ![MIT Licence](https://bitbucket.org/repo/ekyaeEE/images/2049852260-MIT-license-green.png)