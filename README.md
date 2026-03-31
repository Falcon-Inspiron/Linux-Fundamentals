# Linux Fundamental
---

## How i learnt my linux (kubuntu 24.04LTS)
This repository tracks my learning of Linux basics: CLI, permissions, processes, users, tar, cron. I learnt<br>
the basics of linux from **Linuxjourney.com**,then i began from the history of linux and that gave me an<br>
understanding of the unique rules and function of the different types of unix linux system, the different<br>
distro we have and the unique features .
  
## Day 1: Command-Line
### a. NAVIGATION
---

1. Command: 'pwd' - **Print Working Directory** 
> It shows the current directory path you are working on

```bash 
pwd 
```
> Output: /home/username (where username is yourname).

2. Command: 'ls' - **List files** (list files in the directory).

```bash
ls
```
> Output: Desktop  Documents  Downloads Pictures Musics ....

   > `ls -a` List all the hidden files that start with '.' (e.g; .icons, .themes) 

   > `ls -l` List the files in long format (e.g; drwxr-xr-x  2 harry harry 4096 F-Ɛ 22 16:46).

   > `ls -la` With the combination of (-la) or (-al) doesn't matter it list both hidden and unhidden files in long format.

3. Command: 'cd' - **Change directory** (change from one directory to another).

```bash
cd Downloads
```
> Output: ~/Downloads   (This shows you that you are in the Downloads directory)

   > ` cd ~ ` or ` cd ` Go to home directory

   > ` cd .. ` Bring back to previous directory

### b. FILE
---
1. Command: 'touch' - Helps to create a new file in a directory or folder and its file-type, & can also edit or copy timestamp

```bash
touch ~/Downloads/file.dotx
```

> This command checks file timestamp
```bash
stat ~/Downloads/first.dotx
```
>Output:<br>
   Access: 2025-10-02 14:41:34.782807037 +0000<br>
   Modify: 2025-10-02 14:41:34.782807037 +0000<br>
   Change: 2025-10-02 14:41:34.782807037 +0000<br>

Get a new timestamp in this order YYYYMMDDhhmm.ss (Y: year,M: month,D: day,h: hour,m: minutes,s: seconds)
```bash
touch -t 202705231453.45 ~/Downloads/first.dotx
```

Create a new file with the timestamp
```bash
touch ~/Downloads/second.dotx
```

Copies first timestamp to second.
```bash
touch -r ~/Downloads/first.dotx second.dotx
```

Always use this check all changes done to a file timestamp 
```bash
stat ~/Downloads/second.dotx
```

2. Command: 'file' - Used to identify the exact filetype of a file
```bash
file ~/Downloads/first.dotx
```
> Output: /home/name/Downloads/first.dotx: PDF document, version 1.7.

3. Command: 'cat' - used to to read a text file in terminal
```bash
cat ~/Downloads/first.dotx
```

4. Command: 'less' - used to read and display file in page form
```bash
less ~/Downloads/first.dotx
```
5. command: 'history' - it shows last 15 command that you typed in the shell or terminal
 ```bash
history
```
> Output:<br>
   662  touch -r ~/Downloads/first.dotx<br>
   664  stat ~/Downloads/first.dotx<br>
   669  stat ~/Downloads/second.dotx<br>
   670  touch ~/Downloads/first.dotx<br>
   676  touch -t ~/Downloads/first.dotx<br>
   ..................
   .................. etc
 
> `!!` To print recent or previous command.

>Use "CTRL+R" to search for your previous similar command base on input letters
> Output:
        bash
           bck-i-search: _

> `clear` To clean all above and recent commands on the terminal.

## Day 2: Permissions
...

## Day 3: Processes
...

## Day 4: Users & Groups
...

## Day 5: tar Backups
...

## Day 6: Cron Jobs
...

## Day 7: Review
