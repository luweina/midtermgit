# midterm

##Section1

git clone is how you get a local copy of an existing repository to work on. say there is a repo on github and i want to copy it to my own computer

git pull (or git fetch + git merge) is how you update that local copy with new commits from the remote repository

git pull means you are fetching the last modified repository.

when i do git pull, i tried to see the changes from others and get myself the latest copy.

| Trello      | Asana           |  |
| ------------- |:-------------:| -----:|
|if you have lots of columns on a board, it can be harder to filter out what’s not relevant to you.    | One difference is the way sections are grouped makes it easier to keep track of where you arein large projects.  | |
|Trello’s version of dependency management comes via the “Hello Epics” card relationships power up. It lets you add parent-child relationships to tasks and view how many of the child tasks have been completed when looking at the paren     | That means you can specify which tasks need to be done before others can begin. Doing so enables you to spot potential bottlenecks and avoid situations where people are waiting for others to finish before they can do anything.     |    |
| The free version of Trello lets you have as many people as you want on your team. | sana limits you to 15 team members in its free version, though paying customers have no such restrictions.     |

##Section 3

Question 1: What is the .git folder? Where is the object database in this folder?

The .git folder contains all the information that is necessary for your project in version control and all the information about commits, remote repository address, etc. All of them are present in this folder. It also contains a log that stores your commit history so that you can roll back to history.

the database is in .git/object

Question 2: Explain in detail how the git hash-object function works.

Hash functions are one way functions. We can create a hash based on a given input, however we cannot take a Hash and convert it back into its original input. Another important characteristic is that when you take your input and run it through a hash function, the resulting Hash will be fixed length, regardless of what the length of the input was.

                            variable length input

                                           |

                                  Hash Function

C210FD2A1A62F9719955823CB31B7A7DA2E8D715

**Hash functions will always generate the same hash from the same input.**

TLDR;

- Hash functions are 1-way. Knowing a hash does not mean you can go back and figure out what the original input was.
- The same input will always produce the same resulting hash
- A fixed length hash will be generated from a variable length input


Question 3: Where does git internally store the file names to our files? How are tree objects related to this?

it does not store the file name
ree Objects in git represent directories. Each tree may contain BLOBs and other Trees. 