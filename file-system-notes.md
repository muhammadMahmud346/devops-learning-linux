# 5 useful commands 

# ls - Lists contents of the current directory however we can amend this by using ls -l for detailed listing, ls -a to show hidden files 

❯ ls
' '   500          'My Project 2'   command       greet.sh   input.txt   lesson1.txt   lesson5         multilinept2.txt    nearly          requests             yoooooooooooooo
 1   '<S-F1>'       bootcamp        done          helloooo   just        lesson2       mama            my_directory_copy   newfile.txt     set_permissions.sh   you
 2    Hello         bye             example.txt   hi         lesson      lesson3       man             myfile.txt          newfile2.txt    test
 3   'My Project'   combined.txt    file.txt      hi.txt     lesson1     lesson4       multiline.txt   myfile.txtx         newfilebs.txt   yo


# man - man command is the system manual pager, (info gotten from running man man:

NAME
       man - an interface to the system reference manuals

SYNOPSIS
       man [man options] [[section] page ...] ...
       man -k [apropos options] regexp ...
       man -K [man options] [section] term ...
       man -f [whatis options] page ...
       man -l [man options] file ...
       man -w|-W [man options] page ...

DESCRIPTION
       man  is the system's manual pager.  Each page argument given to man is normally the name of a program, utility or function.  The manual page associated with each of these argu‐
       ments is then found and displayed.  A section, if provided, will direct man to look only in that section of the manual.  The default action is to search in all of the available
       sections following a pre-defined order (see DEFAULTS), and to show only the first page found, even if page exists in several sections.

# Whoami - prints effective user name, helpful to know what user you are in to navigate around

❯ whoami
abstract


# chmod - change permissions for a file/direcotry, really helpful when trying to split what the user, group and others can do with the file/directory

❯ man chmod
❯ chmod 644 myfile.txt
❯ ls -la
-rw-r--r--  1 abstract    abstract    302 Aug 15 13:35  myfile.txt


# ps aux - lsist every running process with owner

❯ ps aux
USER         PID %CPU %MEM    VSZ   RSS TTY      STAT START   TIME COMMAND
root           1  0.0  0.3  21800 12240 ?        Ss   12:06   0:02 /sbin/init
root           2  0.0  0.0   3120  1920 ?        Sl   12:06   0:00 /init
root           6  0.0  0.0   3136  1864 ?        Sl   12:06   0:00 plan9 --control-socket 7 --log-level 4 --server-fd 8 --pipe-fd 10 --log-truncate
root          58  0.0  0.3  66756 15272 ?        S<s  12:06   0:01 /usr/lib/systemd/systemd-journald
root         104  0.0  0.1  25280  6400 ?        Ss   12:06   0:00 /usr/lib/systemd/systemd-udevd
systemd+     157  0.0  0.3  21336 12544 ?        Ss   12:06   0:00 /usr/lib/systemd/systemd-resolved
systemd+     158  0.0  0.1  91028  7680 ?        Ssl  12:06   0:00 /usr/lib/systemd/systemd-timesyncd
root         171  0.0  0.0   4236  2688 ?        Ss   12:06   0:01 /usr/sbin/cron -f -P
message+     172  0.0  0.1   9632  4736 ?        Ss   12:06   0:00 @dbus-daemon --system --address=systemd: --nofork --nopidfile --systemd-activation --syslog-only
root         184  0.0  0.2  17964  8320 ?        Ss   12:06   0:00 /usr/lib/systemd/systemd-logind
root         187  0.0  0.3 1756096 13184 ?       Ssl  12:06   0:00 /usr/libexec/wsl-pro-service -vv
root         190  0.0  0.0   3160  2048 hvc0     Ss+  12:06   0:00 /sbin/agetty -o -p -- \u --noclear --keep-baud - 115200,38400,9600 vt220
syslog       193  0.0  0.1 222508  5120 ?        Ssl  12:06   0:00 /usr/sbin/rsyslogd -n -iNONE
root         211  0.0  0.0   3116  1792 tty1     Ss+  12:06   0:00 /sbin/agetty -o -p -- \u --noclear - linux
root         220  0.0  0.5 107012 22144 ?        Ssl  12:06   0:00 /usr/bin/python3 /usr/share/unattended-upgrades/unattended-upgrade-shutdown --wait-for-signal
root         314  0.0  0.0   3128   896 ?        Ss   12:06   0:00 /init
root         315  0.0  0.0   3144  1156 ?        S    12:06   0:00 /init
abstract     316  0.0  0.2  10888  9160 pts/0    Ss   12:06   0:06 -zsh
root         317  0.0  0.1   6664  4224 pts/1    Ss   12:06   0:00 /bin/login -f
abstract     363  0.0  0.2  20312 11392 ?        Ss   12:06   0:00 /usr/lib/systemd/systemd --user
abstract     364  0.0  0.0  21160  3516 ?        S    12:06   0:00 (sd-pam)
abstract     408  0.0  0.1   7144  5328 pts/1    S+   12:06   0:00 -zsh
abstract     476  0.0  0.1   8920  5072 pts/0    S    12:06   0:00 -zsh
abstract     510  0.0  0.1  10160  5916 pts/0    S    12:06   0:00 -zsh
abstract     512  0.0  0.1  10144  5660 pts/0    S    12:06   0:00 -zsh
abstract     513  0.0  0.0   4576  1536 pts/0    Sl   12:06   0:00 /home/abstract/.cache/gitstatus/gitstatusd-linux-x86_64 -G v1.5.4 -s -1 -u -1 -d -1 -c -1 -m -1 -v FATAL -t 16
polkitd     1061  0.0  0.1 308164  7680 ?        Ssl  13:01   0:00 /usr/lib/polkit-1/polkitd --no-debug
abstract    1738  100  0.1   8280  4224 pts/0    R+   14:15   0:00 ps aux
