Fork on the project gitstats
=========================================

These are some personal changes I've added the project [gitstats](http://gitstats.sourceforge.net/), which I hope will soon integrate.

###Changes:
	
 - Change the style sheet(`gitstats.css`).
 - Spanish localization (embed code into `gitstats`).

###Future work:

 - Location in multi-languages ​​(support files `.po`).
   - en\_UK
   - en\_US
   - es\_MX
 - Multilingual support templates
 - Graphing a timeline through the command: `git log --graph --oneline --all`

How to install:
----------------------------

After downloading the project how to install it using the file _MakeFile_ using the `make` with _install_ parameter as follows:

	sudo make install

Gnuplot `requires` and other agencies, should be installed from the package repository to resolve dependencies:

	apt-get install gitstats

Enter the project folder **gitstats** (previously downloaded) and copy the following files:

**updating the CSS**

	 sudo cp gitstats.css /usr/local/share/gitstats/gitstats.css
	 sudo chmod +r /usr/local/share/gitstats/gitstats.css
	 
**updating the script**

	 sudo cp gitstats /usr/bin/gitstats
	 sudo chmod +rx /usr/bin/gitstats
