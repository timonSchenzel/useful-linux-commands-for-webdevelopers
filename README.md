## Common-linux-commands-for-webdevelopers
As a webdeveloper you're not really that much busy with sysops stuff, so I made a list of (basic) commands for webdevelopers of common Linux commands.

### Filesystem

Print working directory
```
pwd
```

List directory content (list files within current working directory)
```
ls
```

List directory content including dot files and as a long list
```
ls -al
```

Making a directory
```
mkdir directoryname/
```

Moving a file/Renaming a file
```
mv oldfile newfile
```

Moving a directory and files within it
```
mv oldir/ newdir/
```

Copying a file
```
cp file copiedfile
```

Copying a directory and files within it
```
cp -R oldir/ copieddir/
```

Moving a file/directory from local to remote (file/directory will come in /some/directory remote)
```
scp file username@remotehost:/some/directory
```

Moving a file/directory from remote to local (file/directory will come in /some/directory)
```
scp username@remotehost:file /some/directory
```

Downloading a file from a url to current directory
```
wget http://www.remote.com/item.txt
```

Human readable directory size or filesize
```
du -sch file
```

### SSH

SSH into a remote machine
```
ssh username@remotehost
```

SSH into a remote machine on a certain port
```
ssh username@remotehost -p PORTNUMBER
```

Copying a public key to remote as authorized key (so you don't have to use a password in the future)
```
ssh-copy-id username@remotehost
```

## Searching
Find a file by name from current directory
```
find . -name 'FILENAME'
```

Find content within a file by string from the current directory (with filename and linenumber)
```
grep -Hinr 'STRING' .
```
