<!SLIDE>
# Versioning Your Code

<!SLIDE incremental bullets>
# Why?
* Cuz I said so
* It's good practice
* Real world experience
* Cuz stuff breaks

<!SLIDE small incremental bullets>
# Why It's Good
* Track changes
* Revert to known good code
* Great for collaboration
* Isolate changes
* Track history
* Code backup

<!SLIDE small incremental bullets>
# Options
* CVS
* SVN
* Bitkeeper
* Git
* Mercurial

<!SLIDE small incremental bullets>
# CVS - 1990
* Client-Server
* Open Source
* Check-in model
* _Clunky_
* Suggested Client - Don't use

<!SLIDE smaller incremental bullets>
# SVN - 2000
* Client-Server
* Open Source
* Commit Model
* _Terrible error messages_
* _Little support for branching_
* _Tagging is clunky_
* Suggested Client - Tortoise SVN

<!SLIDE small incremental bullets>
# Bitkeeper - 2000
* Closed Source 
* Distributed 
* Commit Model
* Used for Linux Kernel Originally
* Spawned Git after licensing change
* Don't Use, mentioned for historical purposes only

<!SLIDE small incremental bullets>
# Git - 2005
* Open Source 
* Distributed
* Commit Model
* Created to meet needs of Linux Kernel
* _Cryptic error messages_
* _Lots of options, some of them are illogical_
* _Lots of __dense__ documentation_

<!SLIDE small incremental bullets>
# Mercurial - 2005
* Open Source
* Distributed
* Commit Model
* Created to meet same needs as Git
* _Better error messages_

<!SLIDE small incremental bullets>
# Why git?
* It's what I know
* Fast
* Distributed
* Open
* Popular
* Space efficient

<!SLIDE small incremental bullets>
# Installing
* Mac - already good
* Ubuntu - apt-get install git-core
* Windows - http://git-scm.com/download/win

<!SLIDE>
# Installing Windows
http://git-scm.com/download/win

<!SLIDE console incremental bullets>
# Initializing a Repository
* _git init_
* creates a .git folder


<!SLIDE console incremental bullets>
# Adding files
* Files must be added before they are tracked
* _git add [file]_
* Uses globbing

<!SLIDE console incremental bullets>
# Committing
* Commiting creates a point you can roll back to
* _git commit -m "[message]"_

<!SLIDE console incremental bullets>
# Cloning from existing
* Pulling down initial code from remote
* _git clone [url]_





