# Part 1 - Section A

## Q1. Define the following Git terms with examples:

- Repository: A directory that Git tracks when git init is run. It contains all the project files.
- Commit: A snapshot that saves your current changes permanently so you can come back to it anytime.
- Branch: Allows you to work on something or add a feature without changing the main code.
- Merge: Adds the changes or features from one branch into another.
- Clone: Copies a remote repository with all its history from GitHub into your local machine.

## Q2. Explain the difference between:

- git fetch vs git pull:
git fetch downloads the changes from the remote but does not apply them.
git pull fetches the changes and applies them.

- git merge vs git rebase:
git merge creates a new commit joining two branch histories together, keeping the original history preserved.
git rebase puts the current branch commits on top of another branch so it looks like you branched off a later point.

- Local repository vs Remote repository:
Local repo is the project on your local machine.
Remote repo is the project on GitHub.

## Q3. What is the purpose of a .gitignore file?

A .gitignore file tells Git which files not to track. For example:
- node_modules/
- .env
- *.log


## Part 1 - Section B

git log shows commit history. --oneline compresses each commit to a single line 

git log --graph --all --decorate
--graph draws a text-based graph of branch/merge history. --all shows all branches.
--decorate labels commits with names and tags.

git status
Shows the current state of your working directory, what is staged, modified, and untracked.

git branch -a
git branch lists branches. -a shows both local and remote branches

git remote -v
git remote manages remote connections. -v shows the URLs for fetch and push.



# Part 2 - Q1

IP Address: A unique numerical label assigned to every device on a network so they can identify and communicate with each other.

Subnet Mask: A 32-bit number that is used to identify which part of the IP Address is the network portion and which is the host portion.

Default Gateway: The IP address of the router on your local network. It is used when a device wants to communicate with something outside it's subnet.

CIDR Notation: A clean method of writing an IP address and its subnet mask together.

Broadcast Address: The last address in a subnet, used to send a message to all devices on that subnet simultaneously.

# Part 2 - Q2

| IP Address  | Class | Public/Private |
|-------------|-------|----------------|
| 10.0.0.1    | A     | Private        |
| 172.16.5.10 | B     | Private        |
| 192.168.1.1 | C     | Private        |
| 8.8.8.8     | A     | Public         |
| 224.0.0.1   | D     | Public         |

# Part 2 - Q3

---IPv4 vs IPv6---
-IPv4 is 32 bits and is represented in decimal.
-IPv6 is 128 bits and is represented in hexadecimal.

---TCP vs UDP---
-TCP is connection based, reliable, and guarantees delivery.
-UDP is connectionless, faster, but does not guarantee delivery.

---Static IP vs Dynamic IP (DHCP)---
-Static IP is assigned manually and never changes.
-Dynamic IP is automatically assigned by the DHCP server any time a device connects.

