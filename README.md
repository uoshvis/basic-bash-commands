# bash commands
`bash --version`
`clear`
`uptime`
`history`
`history -c`
`cat .bash_history`
## reverse search in shell history
`Ctrl+R`

## system date and time
`date`

## system information
```
uname
uname -a
```

## DNS lookup
`host google.com`

## system's host name
`hostname`

## python version
'python -V'

## combine commands
`pwd; ls -l`

## output to file
`(pwd; ls -l) > <filename>`

## move
```
mv source destination
mv source/*.pdf destination
```

## copy
`cp`

## list directory
`ls`

## list parent dir
ls ..

## home directory

ls ~

## all (hidden included)
`ls -a`

## ls long
```
ls -l
ls -l Documents/*.pdf
```

## all long
`ls -al`

## print current working dir
`pwd`

## change dir
`cd <dirname>`

## current dir
`.`

##parent dir
`..`

## home dir
`~`

## create and remove dir
`mkdir`
`rmdir`

## informative remove
`rm -i <target>`

## remove not empty dir
`rm -r <dirname>`

## view whole file concatenate
`cat <filename>`

## view file fit in shell
`more <filename>`

## word count: lines, words, bytes
`wc <filename>`

## count lines
`wc -l <filename>`

## compare files
`diff <f1> <f2>`

## manual
`man <command name>`

## sort file
`sort <filename>`

## unique lines
`uniq <filename>`

## standart output
`sort <filane> > <sorted_filename>`

## standart input redirection
`cat < <filename>`

## show text file
`less <file>`
q quit
D or space -- scroll page
U -- scroll up
< > -- skip first/last line


## search <name> n or N next or previous

/<name>

## globbing
* - wildcard

```ls *html
ls*s
ls *pp*
ls b*png
```

## in brackets

`ls app.{css, html}`

## any one or several ?
```
ls bea?.png
ls bea??.png
```

## any one

`ls be[aeiou]r.png`

## case sensitive
`ls *{jpg,JPG}`

## login info
`who`

## output to file
`who > <filename>`

## configuration files
`/etc`

## variable files expect to grow f.e logs
`/var`

## executable binaries for all users necessary for boot
`/bin`

## super user bin system management applications
`/sbin`

## libraries that support binaries
`/lib`

##user programs
`/usr`

## directories to look for program shell variable $
`echo $PATH`

## lasts until you close shell
`PATH=$PATH:new/dir`

## update
```
man apt-get
sudo apt-get update
sudo apt-get upgrade
sudo apt-get autoremove
```

## users info
`/etc/passwd`

## sudo privilegies
`/etc/sudoers`

## includes to sodoers
https://help.ubuntu.com/community/Sudoers
`sudo ls /etc/sudoers.d`

## permissions
r=4; w=2; x=1
`chmod _+_+_`

## change owner & group
```
sudo chown <name> <target>
sudo chgrp <name> <target>
```

## see url

`curl -o google.html -L 'http://google.com'`
- L (see linked)

## filter commands
```
grep
more
less
sort
uniq
```

## filter examples
```
ls -la | more
cat <filename> | wc
man cat | grep file
ls -l | grep txt | wc
who | sort > <filename>
sort <filename> | uniq | wc -l
```

## grep and pipe
```
grep <obj> <file> | less
grep shell dict.txt | less
curl -L <url> | grep fish | wc -l
```

## PS1 shell variable
google bashrcgenerator

## short names for commands alias
`alias ll='la -la'`

## pupular aliases save to .bash_profile
```
alias .. ='cd ..'
alias ll ='ls -la'
```

## current processes status
```
ps
ps -aef
ps -aef | more
ps -aef | sort | more
ps -aef | sort > <outputfilename>
```

## explaratory data analysis in UNIX
```
cat, grep, wc, sort, uniq
head, tail, cut, sed, find
head -5 <filename>
tail -3
(head -2; tail -2) < <fromfilename>
## paste to file column by column
paste <filename*> > <newfilename>
```

## users running most processes
```
ps -aef | cut -c1-8 | sort | uniq -c | sort -nr | head -3
ps -aef | cut -c1-8 | sort | grep root| wc -l
```
