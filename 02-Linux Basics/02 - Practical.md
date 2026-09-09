High-level architecture:

User
  ↓
Applications
  ↓
Shell
  ↓
Kernel
  ↓
Hardware
Example

When you type:

ls

the flow is approximately:

You
 ↓
Shell
 ↓
Kernel
 ↓
File System / Storage
 ↓
Kernel
 ↓
Shell
 ↓
You see the files
3. WSL + UBUNTU SETUP — COMPLETED ✅

Because you're using Windows, we created a Linux environment using:

WSL 2 + Ubuntu

Your WSL setup:

Windows
   │
   ▼
WSL 2
   │
   ├── Ubuntu
   │
   └── docker-desktop

We specifically decided not to use C: for Ubuntu.

Ubuntu was moved successfully to:

E:\WSL\Ubuntu

Your Linux username:

aslam
4. LINUX HOME DIRECTORY — COMPLETED ✅

Inside Ubuntu, we learned:

pwd

Output:

/home/aslam

This is your Linux home directory.

Important paths
~              → /home/aslam
/home/aslam    → Your Linux home
/mnt/c         → Windows C: drive
/mnt/d         → Windows D: drive
/mnt/e         → Windows E: drive
5. pwd — COMPLETED ✅
Meaning
pwd

= Print Working Directory

It tells you:

Where am I currently?

Example:

/home/aslam/devops
DevOps use

Useful when working on:

Servers
Deployment folders
Logs
Docker
Jenkins
Configuration files
6. mkdir — COMPLETED ✅
Meaning
mkdir

= Make Directory

It creates a folder.

Example:

mkdir devops

Created:

/home/aslam/devops
7. ls — COMPLETED ✅
Meaning
ls

= List

Shows files and directories.

Example:

ls

Output:

notes.txt
project
ls -l
ls -l

shows detailed information.

Example:

-rw-r--r-- 1 aslam aslam    0 notes.txt
drwxr-xr-x 2 aslam aslam 4096 project

We noticed:

- → File
d → Directory

We'll learn the rwx permissions properly later.

8. cd — COMPLETED ✅
Meaning
cd

= Change Directory

Used to move between directories.

Enter a directory
cd devops
Go one level back
cd ..
Go to home
cd ~
Go to a specific location
cd /home/aslam/devops
Important lesson

The same command can work or fail depending on your current location.

For example:

/home/aslam

project ❌

because project is actually:

/home/aslam/devops/project
9. touch — COMPLETED ✅
Meaning
touch

Creates an empty file.

Example:

touch notes.txt

Created:

notes.txt
10. echo — COMPLETED ✅

echo prints text.

Example:

echo "Hello"

Output:

Hello

We also learned that it can be combined with redirection.

11. > — COMPLETED ✅

> redirects output into a file.

Example:

echo "Linux for DevOps" > notes.txt

This creates or overwrites the file.

Remember:

> = overwrite

12. >> — COMPLETED ✅

>> adds content to the end of a file.

Example:

echo "Docker" >> notes.txt

Your file eventually contained:

Hey there!
add docker

Remember:

>> = append

13. cat — COMPLETED ✅

cat displays the contents of a file.

Example:

cat notes.txt

Output:

Hey there!
add docker
🧠 Commands We Know So Far

You can now remember this group:

Command	Meaning
pwd	Show current directory
ls	List files/directories
ls -l	Detailed listing
cd	Change directory
cd ..	Go to parent directory
cd ~	Go home
mkdir	Create directory
touch	Create file
echo	Print text
cat	Read/display file
>	Overwrite file
>>	Append to file


That's a solid first practical block. ✅

📊 Current Progress
LINUX FUNDAMENTALS
────────────────────────────

What is Linux?              ✅
Why Linux was created?     ✅
Why Linux for DevOps?      ✅
Shell vs Kernel             ✅
Linux Architecture          ✅
WSL 2 setup                 ✅
Ubuntu setup                ✅
Linux home directory        ✅

BASIC COMMANDS
────────────────────────────

pwd                         ✅
ls                          ✅
ls -l                       ✅
cd                          ✅
cd ..                       ✅
cd ~                        ✅
mkdir                       ✅
touch                       ✅
echo                        ✅
cat                         ✅
>                           ✅
>>                          ✅



🚧 WHAT WE STILL NEED TO LEARN

This is where the real Linux-for-DevOps journey continues.

Part 1 — File Management
Next
cp
mv
rm
rmdir

Then:

find
locate
file
stat

We'll practice copying, moving, renaming, deleting, and searching files.

Part 2 — Linux File System

We'll properly understand:

/
├── /home
├── /etc
├── /var
├── /usr
├── /bin
├── /sbin
├── /tmp
├── /opt
├── /root
└── /mnt

This is very important for DevOps.

Part 3 — File Permissions 🔥

One of the most important Linux topics.

We'll learn:

r
w
x

and:

755
644
700
777

Commands:

chmod
chown
chgrp
umask
Part 4 — Users & Groups

We'll learn:

whoami
id
groups
who
w

Then:

sudo
su

And understand:

User
 ↓
Group
 ↓
Permissions
Part 5 — Process Management

Very important for DevOps troubleshooting.

Commands:

ps
top
htop
kill
killall
jobs
bg
fg

We'll learn how to answer:

"Why is my application consuming too much CPU?"

Part 6 — Disk & Memory

Commands:

df
du
free

We'll learn:

How do I check whether the server is running out of disk space?

Very useful in production.

Part 7 — Networking 🔥

Very important for DevOps.

Commands:

ping
curl
wget
ip
ss
ssh
scp
hostname

We'll understand:

Client
 ↓
Network
 ↓
Server
 ↓
Port
 ↓
Application

This will prepare you for Docker, Azure and Kubernetes.

Part 8 — Logs 🔥

You'll learn:

tail
tail -f
head
less
grep
journalctl

Example:

tail -f application.log

This is something you'll actually use while troubleshooting applications.

Part 9 — Text Processing

Very important for DevOps and shell scripting.

grep
awk
sed
sort
uniq
cut
wc
xargs

We'll practice with real log files.

Part 10 — Package Management

Ubuntu:

apt
apt-get

We'll learn how to install and update software.

Part 11 — Compression
tar
gzip
zip
unzip

Very useful when moving deployment packages and logs.

Part 12 — Environment Variables

We'll learn:

echo
export
env
printenv

And understand:

PATH
HOME
USER

Environment variables are extremely important in CI/CD.

Part 13 — SSH 🔥

One of the most important DevOps skills.

We'll learn:

ssh
scp

You'll understand how a DevOps engineer connects to a remote Linux server.

Example:

Your Computer
     │
     │ SSH
     ▼
Azure Linux VM
     │
     ▼
Application
Part 14 — Shell / Bash

After the Linux commands, we'll start Shell Scripting.

We'll learn:

#!/bin/bash
variables
if
else
for
while
functions
arguments
exit codes

This will become your Module 03 – Shell Scripting.

Part 15 — Real DevOps Practice

After learning the commands, we'll combine everything.

We'll simulate:

Linux Server
     ↓
Create application directory
     ↓
Copy application files
     ↓
Set permissions
     ↓
Check processes
     ↓
Check disk
     ↓
Check network
     ↓
Read logs
     ↓
Troubleshoot application

This is where the commands start becoming DevOps skills, rather than just Linux commands.

📌 What we should NOT do

Don't try to memorize 100 Linux commands.

Instead:

Learn command
      ↓
Understand problem
      ↓
Practice
      ↓
Use in DevOps scenario
      ↓
Repeat

That's the approach we'll continue.

🎯 Where we stopped

We stopped exactly here:

/home/aslam/devops

├── notes.txt
└── project

And notes.txt contains:

Hey there!
add docker
Next command:
cp

mv - move

mv for moving

Now let's move a file into the project directory.

Currently:

/home/aslam/devops
│
├── notes.txt
├── notes_old.txt
└── project/

Run:

mv notes_old.txt project/

Now check:

ls

You should see:

notes.txt
project

The file disappeared from the current directory because it was moved.

Now check inside project:

ls project

You should see:

notes_old.txt
🧠 So remember
mv file newname

➡️ Rename

mv file directory/

➡️ Move

⭐ Real DevOps Example

Imagine your application produces:

application.log

You want to move old logs into a backup directory:

mv application.log /backup/

Or rename a configuration:

mv application.conf application.conf.backup

This is useful when managing:

Application files
Configuration files
Logs
Deployment files
Backups
⚠️ Important difference: cp vs mv
cp
cp notes.txt backup.txt

Result:

notes.txt       ← Still exists
backup.txt      ← Copy
mv
mv notes.txt backup.txt

Result:

backup.txt      ← Exists
notes.txt       ← No longer exists

Easy way:

cp = Copy
mv = Move/Rename



rm is used to delete a file.

Syntax
rm filename
Practice

First create a safe test file:

touch test.txt

Check that it exists:

ls

You should see:

test.txt

Now delete it:

rm test.txt

Check again:

ls

test.txt should be gone.

🧠 Remember
cp  → Copy
mv  → Move / Rename
rm  → Delete

⚠️ Important: rm normally deletes the file directly; there is no normal Recycle Bin recovery.



rmdir means Remove Directory.

Unlike rm, which we used for files, rmdir is used to delete an empty directory.

Example
rmdir project

⚠️ This works only if project is empty.



Next: file

file tells us what type of file something really is.

For example:

file ~/devops/notes.txt

You might get:

notes.txt: ASCII text

Try it:

file ~/devops/notes.txt

Send me the output. Then we'll quickly finish file + stat and move to Linux File System. 🚀


