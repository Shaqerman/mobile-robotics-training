
<!SLIDE>
# Using Git

<!SLIDE small incremental bullets>
# Installing
* Mac - http://git-scm.com/download/mac
* Mac - install XCode
* Ubuntu - apt-get install git-core
* Windows - http://git-scm.com/download/win

<!SLIDE incremental bullets>
# Initializing a Repository
* _git init_
* creates a .git folder


<!SLIDE incremental bullets>
# Cloning from existing
* Pulling down initial code from remote
* _git clone [url]_

<!SLIDE  incremental bullets>
# Let's Practice
* "Hey I just met you, and this is crazy, but here's my library so clone me maybe"
* git clone git://github.com/schreiaj/MiniQ.git

<!SLIDE>
# Make Changes
"True change comes from within... your text editor."

<!SLIDE incremental bullets>
[This slide intentionally left blank while I go make changes]

<!SLIDE incremental bullets>
# Adding files
* Files must be added before they are tracked
* _git add [file]_
* Uses globbing

<!SLIDE incremental bullets>
# Committing
* Commiting creates a point you can roll back to
* _git commit -m "[message]"_

<!SLIDE incremental bullets>
"If ya like then you shoulda put a ring on it... er what?"

<!SLIDE incremental bullets>
# History
* "Those who do not understand history are doomed to repeat it"
* _git log_

<!SLIDE smaller>
# What's This!
	@@@bash
		commit cde0b480e0f3995a539f8d822ba0f0a9435d3d8f
		Author: Andrew Schreiber 
		Date:   Wed Dec 5 23:24:08 2012 -0500

		    Moved git intro into own slide deck so it can 
		    be easily replaced.

<!SLIDE smaller center>
# Commit
	@@@bash
		commit cde0b480e0f3995a539f8d822ba0f0a9435d3d8f
## Unique hash to refer to this commit


<!SLIDE smaller center>
# Author
	@@@bash
		Author: Andrew Schreiber 
## Who made this commit

<!SLIDE smaller center>
# Date
	@@@bash
		Date:   Wed Dec 5 23:24:08 2012 -0500
## When it was made

<!SLIDE smaller center>
# Message
	@@@bash
		Moved git intro into own slide deck so it can 
	    be easily replaced.
## What was done

<!SLIDE bullets incremental smaller>
# About Commit Messages
* They are like comments
* Clear
* Concise
* Descriptive
* Tells why as well

<!SLIDE bullets incremental smaller>
# When do I commit?
* When you're ready
* Small commits are better
* Descriptive 
* Functional/NonFunctional?
* At __LEAST__ daily

<!SLIDE bullets incremental smaller>
# Branching
* Branches of a tree
* Typically per feature
* Multiple branches are ok
* Named
* Remote or Local

<!SLIDE bullets incremental smaller center>
# Creating a Branch
	@@@bash
		git branch feature
		git checkout feature
* Creates a new branch
* Switches to that branch


<!SLIDE bullets incremental center>
# Working on branches
* Keep Calm and Develop On
* Make some commits

<!SLIDE bullets incremental smaller center>
# Warning, Merge Ahead
	@@@bash
		git checkout master
		git merge feature
* Switches back to _master_
* Merges changes from feature branch

<!SLIDE bullets incremental center small>
# Git Hosting
* Github
* Gitorious
* BitBucket

<!SLIDE bullets incremental center>
# Github
* [github.com](http://github.com/)
* [It's free](https://github.com/edu)

