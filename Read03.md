# Reading Notes For: Revisions and the Cloud

Version control is a numerical system to keep track of newer or older versions of a document or set of code. It's like a history of previous versions of 
the same application. Locally it can be a database on the hard drive, but as collaboration is a common thing nowadays, github allows for cloud storage of
all the versions of files from start to finish.
Files can be cloned from the cloud to the local machine and edited and then the new changes can be committed back to the cloud version, and it keeps a 
history of every major revision along with notes identifying what was changed or added.
Git was first utilized on Linux systems, so whatever the operating system you use on your machine, you will need to set up a Linux terminal to run on
your machine. For my windows pc I installed the powershell terminal and within that I added Ubuntu and then a number of untilities to run from that
command line interface.
When a repository is created on GitHub, the command line interface for Git allows for cloning that repository on the local machine to be worked on, using
the syntax git clone (URL) from github repository. The terminal will keep track of any files added or edited. It can be checked with git status
which will show new or edited files in red. To update the repository online with the new or edited files, first git add (file name) or git add * for all files
to be included, then git commit -m "message about what and why you have changed in the repository" to stage the new repository.
Finally git push origin master will upload the local version of the edited repository to become the 'head' or newest version on the cloud.

[Back to Main Page](https://draquix.github.io/reading-notes-javascript-102/)
