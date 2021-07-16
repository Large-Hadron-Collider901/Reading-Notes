# Git Tutorial- A Comprehensive Guide Notes #

## Version Control ##

**Version control** is a system that keeps track of all changes that are made to your files and allows you to revert back to different versions and modify them as needed.
* Local Version Control consists of one database on your hard disk that stores all changes to files
* Centralized Version Control consists of a *single server* where all changes and file versions are stored. This optimizes the developer's experience by streamlining the collaboration process.
* Distributed Version Control is a system which allows for multiple mirrored repositories. This not only allows programmers to collaborate in various ways, but it addresses the issue of the server as a single point of failure. This way, if the server goes down and anything is lost, the data backups from the DVCS can replace lost information

## What is Git? ##

**Snapshots**
Git is a DVCS where all data in the filesystem is made up of snapshots. Each time you commit a change to your project, Git creates a snapshot of the file and stores a reference to it

**Local Operations**
Git eliminates the need to fetch information from the server and allows you to work offline because it relies (mostly) on local operations

**Tracking Changes**
Git tracks all changes applied to any file or directory and will also detect file corruption or loss of information in transit

**Loss of Data**
Through the use of snapshots, Git greatly reduces the possibility of irreversible damage to files including lost data.