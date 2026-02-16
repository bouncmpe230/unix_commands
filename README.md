# UNIX COMMANDS WITH USAGES



## APT-GET Command

```bash
sudo apt-get update
```

→ Update package lists.

```bash
sudo apt-get upgrade
```

→ Upgrade all upgradable packages.

```bash
sudo apt-get install [package]
```

→ Install a specified package.

```bash
sudo apt-get remove [package]
```

→ Remove a specified package.

```bash
sudo apt-get autoremove
```

→ Remove packages no longer needed.



## AR Command

```bash
ar rcs lib.a file1.o file2.o
```

→ Create or replace a static library archive.

```bash
ar t lib.a
```

→ List contents of a static library archive.

```bash
ar x lib.a
```

→ Extract files from a static library archive.

```bash
ar d lib.a file.o
```

→ Delete a file from the archive.

```bash
ar q lib.a file.o
```

→ Quickly append file to archive.

```bash
ar s lib.a
```

→ Write an index to the archive.



## CAT Command

```bash
cat file.txt
```

→ Display contents of a file.

```bash
cat file1.txt file2.txt
```

→ Concatenate and display multiple files.

```bash
cat > newfile.txt
```

→ Create a file by typing (end with `Ctrl+D`).



## CD Command

```bash
cd /path/to/dir
```

→ Change to a specific directory.

```bash
cd ..
```

→ Go up one directory.

```bash
cd ~
```

→ Go to home directory.



## CHMOD Command

```bash
chmod +x file.sh
```

→ Add execute permission.

```bash
chmod 755 file.sh
```

→ Set read/write/execute for owner, read/execute for others.

```bash
chmod -R 777 dir
```

→ Recursively set full permissions.



## CHOWN Command

```bash
sudo chown user file
```

→ Change file owner.

```bash
sudo chown user:group file
```

→ Change file owner and group.

```bash
sudo chown -R user:group dir
```

→ Recursively change ownership.



## CLEAR Command

```bash
clear
```

→ Clear the terminal screen.



## CP Command

```bash
cp file1.txt file2.txt
```

→ Copy file1.txt to file2.txt.

```bash
cp -r dir1 dir2
```

→ Recursively copy directories.

```bash
cp -i file.txt backup/
```

→ Prompt before overwriting.



## CRON Command

The cron table (`crontab`) defines time-based jobs that the system executes periodically (e.g., daily backups, weekly reports).

```bash
crontab -e
```

→ Edit current user's cron table.

```bash
crontab -l
```

→ List cron jobs.

```bash
crontab -r
```

→ Remove all cron jobs.



## DF Command

```bash
df
```

→ Show disk space usage.

```bash
df -h
```

→ Show human-readable disk usage.

```bash
df -T
```

→ Show filesystem type.



## DIFF Command

```bash
diff file1.txt file2.txt
```

→ Compare two files line by line.

```bash
diff -u old.c new.c
```

→ Unified format for patches.



## DU Command

```bash
du
```

→ Show disk usage per file.

```bash
du -sh .
```

→ Summarize disk usage for current directory.

```bash
du -a
```

→ Show all files and folders with sizes.



## EMACS Command

```bash
emacs file.txt
```

→ Open a file in Emacs.

```bash
emacs -nw file.txt
```

→ Open Emacs in terminal mode.



## EXPORT Command

```bash
export VAR=value
```

→ Set environment variable.

```bash
export PATH=$PATH:/new/path
```

→ Add to PATH.



## FINGER Command

```bash
finger
```

→ Show info on all users.

```bash
finger username
```

→ Show info on specific user.



## G++ Command

```bash
g++ file.cpp
```

→ Compile C++ file.

```bash
g++ -o prog file.cpp
```

→ Compile to a specific output file.

```bash
g++ -Wall file.cpp
```

→ Enable all warnings.



## GCC Command

```bash
gcc file.c
```

→ Compile C file.

```bash
gcc -o prog file.c
```

→ Compile to output file.

```bash
gcc -Wall file.c
```

→ Enable all warnings.

```bash
gcc -fPIC -c file.c
```

→ Generate position-independent code.



## GREP Command

```bash
grep 'main' file.c
```

→ Search for 'main' in file.

```bash
grep -i 'main' file.c
```

→ Case-insensitive search.

```bash
grep -r 'TODO' .
```

→ Recursively search all files.



## GUNZIP Command

```bash
gunzip file.gz
```

→ Decompress `.gz` file.



## GZIP Command

```bash
gzip file
```

→ Compress file.

```bash
gzip -k file
```

→ Compress and keep original.



## HISTORY Command

```bash
history
```

→ Show command history.

```bash
history | grep ssh
```

→ Search history for 'ssh'.



## KILL Command

```bash
kill PID
```

→ Send SIGTERM to a process.

```bash
kill -9 PID
```

→ Force kill a process.

```bash
kill -l
```

→ List signal names.



## LAST Command

```bash
last
```

→ Show last logins.

```bash
last -x
```

→ Include shutdown/reboot entries.



## LS Command

```bash
ls
```

→ List directory contents.

```bash
ls -l
```

→ Long listing format.

```bash
ls -a
```

→ Include hidden files.

```bash
ls -lh
```

→ Human-readable sizes.



## LSCPU Command

```bash
lscpu
```

→ Display CPU architecture info.



## MAKE Command

```bash
make
```

→ Run the default Makefile target.

```bash
make clean
```

→ Delete built files.

```bash
make target
```

→ Run a specific Makefile target.



## MAN Command

```bash
man ls
```

→ Show manual for the `ls` command.

```bash
man 5 passwd
```

→ Show section 5 manual entry for `passwd`.



## MKDIR Command

```bash
mkdir newdir
```

→ Create a new directory.

```bash
mkdir -p a/b/c
```

→ Create nested directories.



## MORE Command

```bash
more file.txt
```

→ Display file page by page.



## MOUNT Command

```bash
sudo mount /dev/sdb1 /mnt
```

→ Mount a device to `/mnt`.

```bash
mount -t iso9660 -o ro /dev/cdrom /mnt/cdrom
```

→ Mount CD-ROM as read-only.



## MV Command

```bash
mv old.txt new.txt
```

→ Rename a file.

```bash
mv file.txt /backup/
```

→ Move a file to another directory.



## NSLOOKUP Command

```bash
nslookup example.com
```

→ Find the IP address of a domain.



## PASSWD Command

```bash
passwd
```

→ Change your own password.

```bash
passwd username
```

→ Change another user's password (requires sudo).



## PING Command

```bash
ping google.com
```

→ Ping a host continuously.

```bash
ping -c 4 example.com
```

→ Ping a host 4 times.



## POPD Command

```bash
popd
```

→ Return to previous directory from stack.



## PS Command

```bash
ps
```

→ Show current shell's processes.

```bash
ps aux
```

→ Show all running processes.

```bash
ps -ef
```

→ Show full-format process list.



## PUSHD Command

```bash
pushd /tmp
```

→ Push current directory to stack and change to `/tmp`.



## PWD Command

```bash
pwd
```

→ Print current working directory.



## RM Command

```bash
rm file.txt
```

→ Remove a file.

```bash
rm -r folder
```

→ Recursively remove a directory.

```bash
rm -f file.txt
```

→ Force delete without prompting.



## RPM Command

```bash
rpm -i package.rpm
```

→ Install RPM package.

```bash
rpm -q package
```

→ Query installed package.



## SFTP Command

```bash
sftp user@host
```

→ Start secure FTP session.

```bash
put file.txt
```

→ Upload file.

```bash
get file.txt
```

→ Download file.

```bash
mkdir folder
```

→ Create remote folder.

```bash
cd /path
```

→ Change remote directory.

```bash
lcd /local/path
```

→ Change local directory.

```bash
ls
```

→ List remote directory contents.

```bash
pwd
```

→ Show remote working directory.

```bash
exit
```

→ Exit SFTP session.



## SOURCE Command

```bash
source ~/.bashrc
```

→ Apply shell configuration changes.

```bash
. env.sh
```

→ Alternative syntax for `source`.



## SSH Command

```bash
ssh user@host
```

→ Open remote shell.

```bash
ssh -i key.pem user@host
```

→ Connect with SSH key.

```bash
ssh -p 2222 user@host
```

→ Connect on specific port.

```bash
ssh user@host 'ls -la'
```

→ Run command remotely.

```bash
ssh -X user@host
```

→ Enable X11 forwarding.



## SU Command (Switch User)

```bash
su john
```

→ Switch to user john.

```bash
su -
```

→ Login as root with full environment.

```bash
su - username
```

→ Switch to specific user with full environment.



## TAR Command

```bash
tar -cvf archive.tar files
```

→ Create tar archive.

```bash
tar -xvf archive.tar
```

→ Extract tar archive.

```bash
tar -xvzf archive.tar.gz
```

→ Extract gzipped archive.

```bash
tar -tvf archive.tar
```

→ List archive contents.

```bash
tar -czf archive.tar.gz dir
```

→ Create gzipped archive.

```bash
tar -xvjf archive.tar.bz2
```

→ Extract bzip2 archive.

```bash
tar -cvJf archive.tar.xz dir
```

→ Create xz compressed archive.



## TEE Command

```bash
echo 'hello' | tee file.txt
```

→ Write output to file and display.

```bash
ls | tee list.txt
```

→ Save and display `ls` output.

```bash
command | tee -a file.txt
```

→ Append output.



## SCRIPT Command

```bash
script
```

→ Start recording terminal session.

```bash
exit
```

→ Stop recording.



## VI Command

```bash
vi file.txt
```

→ Edit file.

```bash
vi +42 file.txt
```

→ Open at line 42.



## W Command

```bash
w
```

→ Show logged-in users and activity.



## WC Command

```bash
wc file.txt
```

→ Show line, word, byte counts.

```bash
wc -l file.txt
```

→ Show line count only.



## WGET Command

```bash
wget http://example.com/file.txt
```

→ Download file from URL.

```bash
wget -O output.txt URL
```

→ Save with specific filename.



## WHO Command

```bash
who
```

→ Show who is logged in.



## WHOAMI Command

```bash
whoami
```

→ Show current username.



## YUM Command

```bash
yum install package
```

→ Install package.

```bash
yum update
```

→ Update all packages.
