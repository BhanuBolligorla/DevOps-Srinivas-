## `Why do we need Version Control?`
  * For collaboration
  * Storing Versions
  * Figuring out what happend
  * Backup

  ## `Issues without version control `
  * Once saved, all the changes made in the files are permanent and cannot be reverted back
  * No record of what was done and by whom
  * Downtime that can occur because of a faulty update could cost millions in losses 

  ## `Version Control :`
Version control systems (VCS) are tools that help track changes to files and manage versions over time. They are essential in software development and other fields where collaboration and revision history are crucial.
 *  Here are the types of version control systems:

    * Local Version Control Systems

    * Centralized Version Control Systems (CVCS)

    * Distributed Version Control Systems (DVCS)

## `Local Version Control Systems:`
 ### Description: 
Tracks file changes on a single computer. These systems are simple and store revisions locally.
## `How It Works: `
Changes are saved in a database or directory structure on the same machine.
## `Examples:`
Revision Control System (RCS)
Local backup scripts
 ## `Advantages:`
Simple and easy to set up.
Suitable for individuals.
 ## `Disadvantages:`
No collaboration features.
No remote backups (loss of data if the machine fails).

## `Centralized Version Control Systems (CVCS):`
`Description:` A single central server stores all the versioned files, and clients check out files from this server.

`How It Works:` Developers sync with a central server for commits, updates, and history.

`Examples:`
* Subversion (SVN)
 * Concurrent Versions System (CVS)
 * Perforce

`Advantages:`
* Easy to manage with a central repository.
* Simpler to enforce security and permissions.

`Disadvantages:`
 * Single point of failure (if the server crashes, all work stops).
* Limited offline capabilities.

 ## `Distributed Version Control Systems (DVCS):`
`Description:` Every developer has a full copy of the repository, including its history.

`How It Works:` Changes are committed locally and then pushed/pulled to/from other repositories when needed.

`Examples:`
 * Git
 * Mercurial
 * Bazaar
 * Fossil

`Advantages:`
 * Full repository backups are available on every developer's machine.
 * Enables offline work.
 * Faster operations since most actions are local.
 * Decentralized collaboration reduces risks.

`Disadvantages:`
 * Initial learning curve for new users.
 * Larger storage requirements (complete history on every machine).
  
