	  __  __
	 |  \/  | __ _ _ __   __ _  __ _
	 | |\/| |/ _` | '_ \ / _` |/ _` |
	 | |  | | (_| | | | | (_| | (_| |
	 |_|  |_|\__,_|_| |_|\__, |\__,_|
	  ____               |___/
	 / ___|  ___ _ __ __ _ _ __  _ __   ___ _ __
	 \___ \ / __| '__/ _` | '_ \| '_ \ / _ \ '__|
	  ___) | (__| | | (_| | |_) | |_) |  __/ |
	 |____/ \___|_|  \__,_| .__/| .__/ \___|_|
						  |_|   |_|
	
						  By : Psycho_Coder
			  rC Developers @ rawCoders.com

# MangaScrapper 
===============
It is simple, easy, and fast CLI tool to download manga's and save them in a directory and as well as save them as an ebook in pdf format. 

*Requires __Python 2.7__ to run.* Manga's are scraped from [MangaPanda](http://www.mangapanda.com/). Whole or complete Manga can be downloaded, or a single chapter or can be downloaded in a range. All these customizations are provided by this tool.

**MangaScrapper** makes use of 3rd party libraries for HTTP Requests and HTML processing. You need to fulfill these requirements before using this tool.

Fulfill the requirements by executing the following in bash
	
	pip install -r requirements.txt

The *requirements.txt* file is present in the repo. 

# Help & Usage
==============

	usage: mangascrapper.py [-h] [-b BEGIN] [-e END] [-c CHAPTER] [-l LOCATION]
                        [-lc]
                        manga_name

    MangaScrapper is simple, easy, and fast CLI tool to download manga's and also
    create an ebook in pdf format.

    positional arguments:
      manga_name            Enter the name of the manga.

    optional arguments:
      -h, --help            show this help message and exit
      -b BEGIN, --begin BEGIN
                            Enter the starting chapter. By default its first
                            chapter
      -e END, --end END     Enter the ending chapter. Defaults to the last chapter
                            possible.
      -c CHAPTER, --chapter CHAPTER
                            Give the chapter number if you want to download only
                            one chapter.
      -l LOCATION, --location LOCATION
                            The location where manga has to be downloaded. By
                            default stored in the current directory.
      -lc, --latest         Download the latest Manga chapter
							

# Example Usage
===============

#### To download complete Manga

	python mangascrapper.py <manga-name>
	
*Example:-* 	

	python mangascrapper.py "One Piece"

#### To download a particular chapter of Manga

	python mangascrapper.py -c <chapter-number> <manga-name>
						or
	python mangascrapper.py --chapter <chapter-number> <manga-name>
	
*Example:-*

	python mangascrapper.py --chapter 1 "Detective Conan"

#### To download chapters of Manga in a range

	python mangascrapper.py -b <beginning-chapter-number> -e <ending-chapter-number> <manga-name>
						or
	python mangascrapper.py --begin <beginning-chapter-number> --end <ending-chapter-number> <manga-name>
	
*Example:-* 	

	python mangascrapper.py --begin 1 --end 5 "Fairy Tail"

#### To download the latest Manga chapter.

	python mangascrapper.py <manga-name> -lc
	                or
	python mangascrapper.py <manga-name> --latest

*Example:-*

	python mangascrapper.py "One Piece" --latest


## Screenshots

![Downloading complete manga "Once Again"](https://i.imgur.com/5dxlDWi.png)
---

![Help Options](https://i.imgur.com/S5QKkuw.png)
---

![Usage Demo and Directory Structure made](https://i.imgur.com/W7D4YAL.png)
---

![A look at the PDF generated](https://i.imgur.com/QiX9wTj.png)
---

![A close look at the PDF generated](https://i.imgur.com/yhN8Rup.png)
---
