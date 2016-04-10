# *nix Scavenger Hunt

Complete the following challenges using the command-line interface on your favorite
Unix or Linux operating system. You are welcome and encouraged to consult any
additional documentation online or in books.

Please add your answers/responses/text pastes to the document after each prompt.

Note: For some of the challenges you will need to reference files included with
this repository, so you will need to fork the repo into your own Github account
and then clone it to your development environment.

# *nix Scavenger Hunt

Complete the following challenges using the command-line interface on your favorite
Unix or Linux operating system. You are welcome and encouraged to consult any
additional documentation online or in books.

Please add your answers/responses/text pastes to the document after each prompt.

Note: For some of the challenges you will need to reference files included with
this repository, so you will need to fork the repo into your own Github account
and then clone it to your development environment.

## The Challenges

### Navigating the Filesystem

* Get an idea of where you are in the operating system. Use the `pwd` command to find your "path to working directory"--your current location in the filesystem of your devbox. *Paste the output of the `pwd` command here:
~ $ pwd
/Users/donjohnson

* Discover more about this filesystem. Use `ls` (the "list" command)to see what is in this directory. *What directories and files do you see when you run `ls`?*
~ $ ls
Applications
Creative Cloud Files
Desktop
Documents
Downloads
Dropbox
Library
Movies
Music
Pictures
Public
johns325@seattleu.edu Creative Cloud Files

* You can use *options* to modify how a command runs. Try using `ls -alh` to see the contents of your current directory. *How are the results different when you use the `-alh` options?*
~ $ ls -alh
total 56
drwxr-xr-x+  27 donjohnson  staff   918B Feb 21 14:52 .
drwxr-xr-x    6 root        admin   204B Dec 25  2014 ..
-r--------    1 donjohnson  staff     7B Dec 25  2014 .CFUserTextEncoding
-rw-r--r--@   1 donjohnson  staff    10K Mar  8 18:45 .DS_Store
drwx------    9 donjohnson  staff   306B Mar  4 19:59 .Trash
drwxr-xr-x   12 donjohnson  staff   408B Jan  3 11:23 .atom
-rw-------    1 donjohnson  staff   243B Sep 13  2015 .bash_history
drwx------    4 donjohnson  staff   136B Feb  6 12:20 .config
drwx------    9 donjohnson  staff   306B Mar 31 20:50 .dropbox
drwxr-xr-x    3 donjohnson  staff   102B Feb  6 13:30 .freac
-rw-r--r--    1 donjohnson  staff   1.0K Feb  6 12:20 .gitconfig
drwxr-xr-x    3 donjohnson  staff   102B Sep 13  2015 .local
drwxr-xr-x    3 donjohnson  staff   102B Nov 22  2014 .mplayer
-rwxrwxrwx@   1 donjohnson  staff    41B Nov  8  2014 .orvkknhrc
drwx------    5 donjohnson  staff   170B Feb  6 12:20 .ssh
drwx------    4 donjohnson  staff   136B Oct 25 04:13 Applications
drwxrwxr-x@   3 donjohnson  staff   102B Mar  9 12:24 Creative Cloud Files
drwx------+ 113 donjohnson  staff   3.8K Apr  2 17:13 Desktop
drwx------+  14 donjohnson  staff   476B Dec  5 11:00 Documents
drwx------+ 229 donjohnson  staff   7.6K Mar 14 21:06 Downloads
drwx------@  49 donjohnson  staff   1.6K Mar 31 20:50 Dropbox
drwx------@  56 donjohnson  staff   1.9K Dec 17 20:23 Library
drwx------+   6 donjohnson  staff   204B Jul 22  2015 Movies
drwx------+   9 donjohnson  staff   306B Feb  6 12:10 Music
drwx------+   5 donjohnson  staff   170B Jul 22  2015 Pictures
drwxr-xr-x+   5 donjohnson  staff   170B Sep 27  2014 Public
drwxrwxr-x@   3 donjohnson  staff   102B Dec 14 12:08 johns325@seattleu.edu Creative Cloud Files

* The `man` ("manual") command tells you more about how any given command works. (*WARNING:* CodeAnywhere does not support the man command. You can click the following link to complete this task: http://linux.die.net/man/)Run `man` to see instructions about how to use `man`. Then use `man` to learn what the `a`, `l`, and `h` options mean when used with the `ls` command. *Write down what those options do?*
~ $ man
What manual page do you want?

* Commands can also take *arguments*, which are usually the names of files or locations that you want the command to work with. Try running `ls /` to see what files are in the *root* directory of the filesystem. *What files and directories do you see listed?*
~ $ ls /
Applications              bin                       private
Incompatible Software     cores                     sbin
Library                   dev                       tmp
Network                   etc                       usr
System                    home                      var
Users                     installer.failurerequests
Volumes                   net

* A Unix filesystem has a few special shortcuts to refer to specific locations. `/` indicates the *root* of the filesystem, meaning the top-most directory in the filesystem hierarchy. Use the `cd` ("change directory") command to move to the root directory. (Hint: Use `man` to look up the `cd` command if you have any issues) *Then run `pwd` and paste the output here:*

* Another special shortcut in Unix is the `~` location. This indicates the *user root* directory, meaning the top-most directory in the hierarchy that comes below your user account. Use `cd` to move to `~`. *Run `pwd` and paste the response here:*

* Change directory into the `challenge_files` directory. Use `ls` to find only the files with a `.demo` pattern. *How many files do you find?*
~ $ ls
Applications                               Library
Creative Cloud Files                       Movies
Desktop                                    Music
Documents                                  Pictures
Downloads                                  Public
Dropbox 

* Use the `cd` command to move "up" one directory. *Where are you in the filesystem now?*
$ cd

* Press the up arrow on your keyboard. *What just happened?*
It shows the last command
* Press the up arrow a few more times. *What do you see?*
It goes up to each previous command 
* Run the `history` command. *What do you see?*
~ $ history

ls
.demo
cd
man
cd/
/
ls /
history
hist
ls -alh
pwd
curl -fsSL http://git.io/QxUaOQ | sh
curl -fsSL http://git.io/7UHtNA | sh
git config --global user.name 'DONALD JOHNSON'
git config --global user.email JOHNSON.K.DONALD@GMAIL.COM
git config --global user.name DONALD JOHNSON
git --version
brew install git
git config --global user.name ‘DONALD JOHNSON'
git config --global user.email ‘JOHNSON.K.DONALD@GMAIL.COM'
git config --global user.name 'YOUR FULL NAME'
subl /etc/paths
echo $PATH
echo $EDITOR
:

### Observing the System

* Discover what account you are logged into using the `whoami` command. *What username are you currently using?*
~ $ whoami
donjohnson
* Discover who else is on your system with the `who` command. *Are any other users using your system? If so, list them here:*
~ $ who
donjohnson console  Mar 31 20:46 
donjohnson ttys000  Apr 10 12:21 
* How long has your system been running? Use `uptime` to see, and *paste the result here:*
~ $ uptime
12:32  up 9 days, 15:48, 2 users, load averages: 2.21 2.09 2.16
* Run `ps aux` and review the results. (Hint: Use `man` to learn more about the `ps` command and options.) *How do you interpret what you see here?*
USER              PID  %CPU %MEM      VSZ    RSS   TT  STAT STARTED      TIME COMMAND
donjohnson      61049  61.8  1.4  4534584  58272   ??  U    Tue08PM  69:32.51 /Applications/Sa
_windowserver     153  55.2  1.8  3680232  74096   ??  Us   31Mar16 118:21.78 /System/Library/
donjohnson      25369  15.0  4.6  4319188 194952   ??  Us   10:49AM   4:45.40 /System/Library/
donjohnson        367   2.3  0.3  1166520  13244   ??  S    31Mar16  52:36.25 /Applications/Ut
donjohnson      48440   1.9  0.8  2644860  33156   ??  S    11:51AM   0:25.86 /Applications/Ut
donjohnson        671   1.6  3.0  3534592 127548   ??  S    31Mar16  45:17.36 /Applications/Go
root            66082   1.0  0.0  2441148    824 s000  R+   12:37PM   0:00.00 ps aux
donjohnson        321   0.9  0.9  2927816  38848   ??  S    31Mar16  31:44.38 /Applications/Go
donjohnson        678   0.6  0.9  2874484  36352   ??  S    31Mar16  12:02.82 /Applications/Go
donjohnson        497   0.6  0.3   861088  13484   ??  S    31Mar16   3:53.36 /Library/Applica
donjohnson      61083   0.5  0.3  3630484  14388   ??  Ss   Tue08PM   1:42.57 /System/Library/
donjohnson      59887   0.4  0.0  2461312   1700 s000  S    12:21PM   0:00.32 -fish
root             1755   0.3  0.2  6335832   8708   ??  Ss    2Apr16   7:33.84 /System/Library/
donjohnson        556   0.3  0.1  2460652   4524   ??  S    31Mar16   3:51.42 /Applications/Ut
donjohnson      13667   0.3  2.7  3592272 111604   ??  S    10:18AM   1:24.84 /Applications/Go
donjohnson        555   0.2  0.2   864856   7816   ??  S    31Mar16  29:51.35 /Library/Applica
_softwareupdate  1612   0.2  0.2  3601376   9900   ??  Ss    2Apr16   8:11.60 /System/Library/
donjohnson        669   0.1  2.7  4127144 114760   ??  S    31Mar16  39:55.97 /Applications/Go
donjohnson        237   0.1  2.8  3408588 115964   ??  S    31Mar16  34:49.39 /Applications/Go
root            12161   0.1  0.0   632116   1356   ??  S    10:29PM   0:26.77 /var/folders/zz/
root            20485   0.1  0.0   632636   1236   ??  S    Thu06PM   1:22.79 /var/folders/zz/
donjohnson        563   0.1  0.3   894824  10608   ??  S    31Mar16  13:27.79 /Library/Applica
donjohnson        499   0.1  0.1  2460652   4524   ??  S    31Mar16   3:50.98 /Library/Applica
donjohnson      19738   0.0  1.3  3524296  52832   ??  S    10:34AM   0:41.36 /Applications/Go
root            13290   0.0  0.0  2469216    280   ??  SNs  10:17AM   0:00.01 /usr/libexec/per
_netbios        13230   0.0  0.1  2470004   4412   ??  SNs  10:17AM   0:00.05 /usr/sbin/netbio
root            12200   0.0  0.1  2470640   4780   ??  S    10:29PM   0:00.42 /System/Library/
root            12162   0.0  0.3  3639928  12656   ??  S    10:29PM   0:12.86 /usr/sbin/instal
root            12046   0.0  0.1  2511832   5100   ??  Ss   10:29PM   0:04.49 /System/Library/
donjohnson       9273   0.0  0.0  2495812   1868   ??  Ss   10:21PM   0:00.12 /System/Library/
donjohnson       9210   0.0  0.1  2471504   4000   ??  Ss   10:21PM   0:00.03 /System/Library/
donjohnson       8523   0.0  1.8  4067064  77580   ??  S    10:19PM   1:02.46 /Applications/Sk
_iconservices    8460   0.0  0.0  2469404   1764   ??  Ss   10:19PM   0:00.03 /System/Library/
donjohnson       8459   0.0  0.1  2504444   2552   ??  S    10:19PM   0:00.22 /System/Library/
donjohnson       6037   0.0  0.3  2541520  12828   ??  S    10:13PM   0:00.23 /System/Library/
donjohnson       5686   0.0  0.1  2471100   2492   ??  S    10:12PM   0:00.09 /System/Library/
root             3168   0.0  0.1  2459668   4016   ??  Ss   10:05PM   0:00.02 /System/Library/
donjohnson       2804   0.0  0.6  2507796  25596   ??  Ss   10:04PM   0:04.38 /System/Library/
donjohnson       2756   0.0  0.2  2500988   9772   ??  S    10:04PM   0:00.18 /System/Library/
donjohnson       2728   0.0  0.4  2506320  15480   ??  Ss   10:04PM   0:01.73 /System/Library/
donjohnson       2721   0.0  0.2  2516384  10144   ??  Ss   10:04PM   0:05.30 /System/Library/
donjohnson       2657   0.0  0.1  2544740   5948   ??  S    10:04PM   0:02.23 /usr/libexec/Saf
donjohnson       2656   0.0  0.2  2503688   8568   ??  S    10:04PM   0:00.20 /System/Library/
root             2407   0.0  0.0  2469836   1820   ??  Ss   10:03PM   0:00.07 /System/Library/
root             1937   0.0  0.0  2521212   2072   ??  Ss   10:02PM   0:00.20 /usr/libexec/san
donjohnson       1871   0.0  0.1  2544504   5528   ??  Ss   10:02PM   0:00.22 /System/Library/
donjohnson       1732   0.0  0.2  2534604   8184   ??  S    10:01PM   0:00.31 /System/Library/
root             1531   0.0  0.0  2449796    256   ??  Ss   10:01PM   0:00.01 /usr/sbin/aslman
root            99085   0.0  0.1  2495996   2732   ??  Ss   Thu10PM   0:00.16 /System/Library/
donjohnson      85085   0.0  0.2  2496220   6312   ??  S    Thu09PM   0:00.57 /System/Library/
donjohnson      71150   0.0  0.6  2852508  25200   ??  S    Thu09PM   0:16.25 /Applications/Go
donjohnson      64736   0.0  0.1  2495112   3620   ??  S    Thu08PM   0:00.38 /System/Library/
donjohnson      63703   0.0  0.4  2497524  17112   ??  S    Thu08PM   0:02.81 /System/Library/
donjohnson      62517   0.0  0.2  2546028   6716   ??  Ss   Thu08PM   0:02.68 /System/Library/
root            54845   0.0  0.1  2494612   2412   ??  Ss   Thu08PM   0:00.73 /usr/libexec/amf
donjohnson      50899   0.0  0.1  2468896   4792   ??  Ss   Thu08PM   0:00.02 /System/Library/
donjohnson      50867   0.0  0.3  2502696  12232   ??  S    Thu08PM   0:00.66 /System/Library/
donjohnson      50866   0.0  0.1  2497652   5292   ??  S    Thu08PM   0:00.14 /System/Library/
root            47389   0.0  0.0  2495416   1396   ??  Ss   Thu08PM   0:00.08 /usr/libexec/dia
root            44126   0.0  0.1  2469560   2320   ??  Ss   Thu07PM   0:00.05 /System/Library/
root            43412   0.0  0.0  2468048   1676   ??  Ss   Thu07PM   0:00.03 /System/Library/
donjohnson      40990   0.0  0.3  2499296  10608   ??  Ss   Thu07PM   0:00.91 /System/Library/
donjohnson      39439   0.0  0.1  2498404   6220   ??  S    Thu07PM   0:00.45 /usr/libexec/pkd
donjohnson      38352   0.0  0.1  2497152   3236   ??  S    Thu07PM   0:00.54 /usr/libexec/sec
donjohnson      38350   0.0  0.2  2555104   9568   ??  S    Thu07PM   0:00.33 /System/Library/
root            38349   0.0  0.0  2471788    908   ??  Us   Thu07PM   0:00.13 /System/Library/
donjohnson      38348   0.0  0.4  2558888  16260   ??  S    Thu07PM   0:00.98 /System/Library/
root            38190   0.0  0.0  2470480   1840   ??  Ss   Thu07PM   0:00.50 /System/Library/
donjohnson      38158   0.0  0.1  2472664   2328   ??  S    Thu07PM   0:00.04 /usr/libexec/spi
root            38157   0.0  0.1  2561184   5432   ??  Ss   Thu07PM   0:02.30 /usr/sbin/spindu
root            37845   0.0  0.0  2473860   1548   ??  Ss   Thu07PM   0:07.72 /usr/libexec/sys
root            37844   0.0  0.0  2469336   1588   ??  Ss   Thu07PM   0:01.55 sysmond
donjohnson      37812   0.0  0.2  2499516   7460   ??  S    Thu07PM   0:03.02 /System/Library/
donjohnson      37650   0.0  0.1  2498512   2876   ??  S    Thu07PM   0:00.12 /System/Library/
root            37407   0.0  0.0  2469224    776   ??  Ss   Thu07PM   0:00.05 /usr/libexec/net
donjohnson      37214   0.0  0.1  2473144   2264   ??  S    Thu07PM   0:02.85 /usr/sbin/cfpref
root            37095   0.0  0.1  2470452   2384   ??  Ss   Thu07PM   0:01.79 /System/Library/
_nsurlstoraged  37063   0.0  0.0  2469324   1948   ??  Ss   Thu07PM   0:00.11 /usr/libexec/nsu
root            37062   0.0  0.1  2472916   2244   ??  Ss   Thu07PM   0:04.17 /usr/sbin/cfpref
root            37061   0.0  0.1  2471524   2264   ??  Ss   Thu07PM   0:00.10 /System/Library/
donjohnson      37044   0.0  0.1  2500460   4252   ??  U    Thu07PM   0:01.73 /System/Library/
donjohnson      37038   0.0  0.1  2493380   4664   ??  S    Thu07PM   0:00.33 /usr/libexec/sec
donjohnson      37037   0.0  0.3  2533456  11996   ??  S    Thu07PM   0:00.84 /System/Library/
donjohnson      33205   0.0  0.0  2495860   1976   ??  S    Thu07PM   0:00.07 /System/Library/
donjohnson      32273   0.0  0.0  2469404   1656   ??  S    Thu07PM   0:00.02 /System/Library/
donjohnson      32272   0.0  0.5  2522792  22348   ??  S    Thu07PM   0:11.79 /System/Library/
root            20561   0.0  0.1  2470640   4776   ??  S    Thu06PM   0:01.25 /System/Library/
root            20529   0.0  0.0  2472828   1708   ??  Ss   Thu06PM   0:00.05 /usr/sbin/diskma
root            20488   0.0  0.3  3637668  12336   ??  S    Thu06PM   0:37.96 /usr/sbin/instal
root            20286   0.0  0.1  2505164   5084   ??  Ss   Thu06PM   0:03.87 /System/Library/
donjohnson      16824   0.0  0.0  2495860   1936   ??  S    Thu06PM   0:00.07 /System/Library/
donjohnson      16349   0.0  0.0  2495860   1936   ??  S    Thu06PM   0:00.07 /System/Library/
donjohnson      15832   0.0  0.4  2512040  17296   ??  Ss   Thu06PM   0:18.56 /System/Library/
donjohnson      15269   0.0  0.6  2519092  23832   ??  S    Thu06PM   0:31.56 /System/Library/
donjohnson      15088   0.0  0.9  2588488  39696   ??  S    Thu06PM   0:25.52 /System/Library/
donjohnson      62849   0.0  0.2  2498320  10408   ??  S    Tue08PM   0:16.21 /usr/libexec/nsu
donjohnson      62848   0.0  0.7  2527512  27580   ??  S    Tue08PM   0:32.19 /System/Library/
donjohnson       3116   0.0  1.0  3475160  40884   ??  S    Mon08PM   1:46.19 /Applications/Go
donjohnson      69471   0.0  0.1  2504468   4912   ??  Ss   Sun08PM   0:00.14 /System/Library/
root            70100   0.0  0.0  2493000   2084   ??  Ss    3Apr16   0:00.07 /System/Library/
root            55682   0.0  0.3  2506752  14128   ??  Ss    2Apr16  33:53.37 /usr/libexec/cor
donjohnson      42189   0.0  0.1  2469424   3960   ??  S     2Apr16   0:00.04 /usr/libexec/USB
donjohnson       1771   0.0  0.3  2564492  12144   ??  S     2Apr16  12:50.70 ./Tools/AlertAll
root             1770   0.0  0.0  2452612   1572   ??  S     2Apr16   0:00.02 /usr/bin/sudo -u
root             1769   0.0  0.0  2452552    504   ??  S     2Apr16   0:00.04 /usr/bin/perl /p
root             1764   0.0  0.0  2453536    496   ??  S     2Apr16   0:00.03 /usr/bin/perl /t
_spotlight       1763   0.0  0.1  2472704   4216   ??  S     2Apr16   0:00.78 /System/Library/
root             1760   0.0  0.0  2460696   1604   ??  S     2Apr16   0:00.01 /System/Library/
root             1746   0.0  0.0  2460000    276   ??  S     2Apr16   0:00.01 /System/Library/
donjohnson       1623   0.0  0.2  2544728   8008   ??  S     2Apr16   0:01.73 /System/Library/
root             1616   0.0  0.1  2469672   3996   ??  Ss    2Apr16   0:00.05 /System/Library/
root             1613   0.0  0.0  2469772    528   ??  Us    2Apr16   0:00.04 /usr/libexec/sys
donjohnson        758   0.0  0.2  3607204   7676   ??  S     1Apr16   0:01.46 /System/Library/
donjohnson        728   0.0  0.7  4024640  30620   ??  S    31Mar16   0:21.52 /Applications/Go
donjohnson        694   0.0  0.1  2477352   5980   ??  S    31Mar16   0:09.89 /usr/libexec/nsu
donjohnson        675   0.0  0.8  3433056  34052   ??  S    31Mar16   0:12.37 /Applications/Go
donjohnson        673   0.0  1.6  4771936  68628   ??  S    31Mar16  16:59.27 /Applications/Go
donjohnson        672   0.0  0.7  3412332  30912   ??  S    31Mar16   1:28.32 /Applications/Go
donjohnson        668   0.0  0.0  2469216    556   ??  S    31Mar16   0:01.45 /System/Library/
donjohnson        663   0.0  0.1  2504372   4116   ??  S    31Mar16   0:00.61 /System/Library/
donjohnson        656   0.0  0.1  2474596   4180   ??  S    31Mar16   0:00.16 /System/Library/
donjohnson        621   0.0  0.0  2496884   1900   ??  S    31Mar16   0:00.18 /System/Library/
donjohnson        561   0.0  0.2  2544352   7368   ??  S    31Mar16   0:00.76 /System/Library/
root              526   0.0  0.0  2469216   1672   ??  Ss   31Mar16   0:00.04 /System/Library/
donjohnson        517   0.0  0.8  3090324  35196   ??  S    31Mar16   0:48.80 /Applications/Ut
donjohnson        516   0.0  0.2  2614340   8120   ??  S    31Mar16   0:26.20 /Applications/Ut
donjohnson        515   0.0  0.1  2504468   4844   ??  Ss   31Mar16   0:00.30 /System/Library/
donjohnson        511   0.0  0.1  2504468   4844   ??  Ss   31Mar16   0:00.33 /System/Library/
donjohnson        496   0.0  0.1   704208   2400   ??  S    31Mar16   1:52.60 /Applications/Ut
donjohnson        482   0.0  0.2  2538840   6800   ??  Ss   31Mar16   0:00.84 /Applications/Dr
donjohnson        452   0.0  0.1   860024   4240   ??  S    31Mar16   0:04.72 /Library/Applica
donjohnson        430   0.0  0.1  2460652   4528   ??  S    31Mar16   3:52.04 /Applications/Ut
donjohnson        427   0.0  0.2  2543636   7292   ??  S    31Mar16   0:00.71 /System/Library/
donjohnson        425   0.0  0.8  3442872  33240   ??  S    31Mar16   0:36.04 /Applications/Go
donjohnson        415   0.0  1.3  3484580  56016   ??  S    31Mar16   1:44.20 /Applications/Go
donjohnson        414   0.0  1.8  3559892  75812   ??  S    31Mar16   0:34.16 /Applications/Go
donjohnson        409   0.0  0.8  3416936  32460   ??  S    31Mar16   1:30.38 /Applications/Go
donjohnson        404   0.0  0.7  3417072  27932   ??  S    31Mar16   1:29.99 /Applications/Go
root              403   0.0  0.1  2614520   5708   ??  Ss   31Mar16   2:31.85 /System/Library/
root              397   0.0  0.0  2493292   1924   ??  Us   31Mar16   0:00.31 /System/Library/
donjohnson        381   0.0  1.1  4004152  46324   ??  S    31Mar16   3:25.62 /Applications/Dr
donjohnson        375   0.0  0.1  2498844   2980   ??  S    31Mar16   0:00.24 /Applications/iT
donjohnson        369   0.0  0.1  2499320   5776   ??  S    31Mar16   0:02.30 /System/Library/
donjohnson        368   0.0  0.2  2535176   6948   ??  S    31Mar16   0:03.39 /System/Library/
donjohnson        363   0.0  0.2  2492964   7788   ??  S    31Mar16   0:00.33 /System/Library/
donjohnson        356   0.0  0.2  2649468   9864   ??  S    31Mar16   0:09.27 /System/Library/
donjohnson        353   0.0  0.2  2543764  10336   ??  S    31Mar16   0:00.73 /System/Library/
donjohnson        351   0.0  0.1  2494992   6104   ??  S    31Mar16   0:01.12 /System/Library/
donjohnson        337   0.0  0.2  2570768   7832   ??  S    31Mar16   0:03.72 /System/Library/
donjohnson        329   0.0  0.7  3283944  28180   ??  S    31Mar16   2:08.49 /Applications/Go
donjohnson        325   0.0  1.2  3372572  49372   ??  S    31Mar16   0:49.30 /Applications/Go
donjohnson        307   0.0  0.1  2494624   4516   ??  S    31Mar16   0:00.79 /Applications/Go
donjohnson        303   0.0  0.2  2500864   6660   ??  S    31Mar16   5:45.05 /System/Library/
donjohnson        300   0.0  0.1  2500248   5112   ??  S    31Mar16   0:00.28 /System/Library/
donjohnson        299   0.0  0.3  2545488  10560   ??  Ss   31Mar16   0:01.17 /System/Library/
donjohnson        298   0.0  0.1  2468920   4100   ??  S    31Mar16   0:00.15 /System/Library/
donjohnson        296   0.0  0.2  2495764   9312   ??  S    31Mar16   0:01.03 /usr/libexec/fmf
donjohnson        287   0.0  0.2  2496656   8592   ??  S    31Mar16   0:02.44 /System/Library/
donjohnson        279   0.0  0.1  2472056   2852   ??  Ss   31Mar16   0:06.23 /System/Library/
donjohnson        276   0.0  0.3  2509228  11156   ??  S    31Mar16   0:06.66 /System/Library/
donjohnson        275   0.0  0.2  2497920   9224   ??  S    31Mar16   0:01.57 /System/Library/
donjohnson        273   0.0  0.2  2537716   6828   ??  Ss   31Mar16   0:01.00 /Applications/Ut
donjohnson        268   0.0  0.2  2515140   9964   ??  S    31Mar16   0:04.79 /System/Library/
root              266   0.0  0.1  2474736   2868   ??  Ss   31Mar16   0:01.39 /usr/sbin/fileco
donjohnson        263   0.0  0.3  2592996  11912   ??  S    31Mar16   0:03.44 /System/Library/
donjohnson        259   0.0  0.0  2528080   1932   ??  S    31Mar16   0:23.15 /System/Library/
donjohnson        256   0.0  0.2  2508636   9664   ??  S    31Mar16   0:04.61 /usr/libexec/sha
root              254   0.0  0.2  2470264   7688   ??  Ss   31Mar16   0:00.21 /System/Library/
donjohnson        250   0.0  0.0  2468604    468   ??  S    31Mar16   0:00.02 /usr/sbin/pboard
_coreaudiod       248   0.0  0.2  2501980   6904   ??  Ss   31Mar16   9:14.51 /usr/sbin/coreau
donjohnson        247   0.0  0.4  2742256  18252   ??  S    31Mar16   0:15.76 /System/Library/
donjohnson        246   0.0  0.3  2576268  13624   ??  U    31Mar16   0:30.97 /System/Library/
donjohnson        244   0.0  0.4  2670440  16612   ??  S    31Mar16   0:11.77 /System/Library/
donjohnson        242   0.0  0.0  2453972     16   ??  T    31Mar16   0:00.00 /Applications/iT
donjohnson        232   0.0  0.3  2533232  11780   ??  S    31Mar16   1:06.00 /System/Library/
donjohnson        231   0.0  0.1  2496792   2528   ??  S    31Mar16   0:04.20 /usr/sbin/userno
donjohnson        227   0.0  0.1  2470788   5324   ??  S    31Mar16   0:50.16 /usr/sbin/distno
donjohnson        225   0.0  0.2  2500396  10384   ??  S    31Mar16   0:18.62 /usr/libexec/Use
root              223   0.0  0.0  2493372   1264   ??  Ss   31Mar16   0:00.72 /usr/libexec/sec
root              211   0.0  0.5  3113276  19128   ??  Ss   31Mar16   1:32.82 /System/Library/
root              195   0.0  0.1  2495580   4464   ??  Ss   31Mar16   0:00.31 /System/Library/
root              188   0.0  0.0  2504204    512   ??  Ss   31Mar16   0:00.41 /System/Library/
root              177   0.0  0.1  2581164   5788   ??  Ss   31Mar16   1:06.72 /System/Library/
root              176   0.0  0.1  2469584   2176   ??  Ss   31Mar16   0:00.50 /usr/libexec/cor
root              172   0.0  0.1  2492900   4448   ??  Ss   31Mar16   0:01.31 /usr/libexec/usb
root              171   0.0  0.0  2471156    888   ??  Ss   31Mar16   0:08.56 /usr/sbin/ntpd -
root              167   0.0  0.1  2469416   3920   ??  Ss   31Mar16   0:09.67 /usr/libexec/wat
_networkd         163   0.0  0.1  2499380   4256   ??  Ss   31Mar16   0:26.00 /usr/libexec/net
root              139   0.0  0.0  2471660   1680   ??  Ss   31Mar16   0:00.04 /System/Library/
root              124   0.0  0.1  2497344   4436   ??  Ss   31Mar16   0:15.05 /System/Library/
_distnote          99   0.0  0.0  2470788   1484   ??  Ss   31Mar16   0:09.53 /usr/sbin/distno
root               97   0.0  0.1  2506208   3944   ??  Ss   31Mar16   0:04.77 /System/Library/
root               95   0.0  0.1  2494596   3864   ??  Ss   31Mar16   0:13.15 /usr/libexec/tas
root               94   0.0  0.0  2471856   1916   ??  Ss   31Mar16   6:07.83 /usr/sbin/notify
root               93   0.0  0.1  2470036   2836   ??  Ss   31Mar16   1:02.29 /usr/libexec/hid
root               91   0.0  0.0  2469240    488   ??  Ss   31Mar16   0:00.02 /usr/sbin/Kernel
root               90   0.0  0.0  2470972   1652   ??  Ss   31Mar16   0:00.20 /System/Library/
donjohnson         89   0.0  0.3  2570660  10816   ??  Ss   31Mar16   0:17.43 /System/Library/
root               88   0.0  0.0  2496796   2096   ??  Us   31Mar16   0:00.33 /System/Library/
root               87   0.0  0.0  2469260    520   ??  Ss   31Mar16   0:00.09 /usr/libexec/sta
_mdnsresponder     85   0.0  0.1  2496076   4144   ??  Ss   31Mar16   0:24.94 /usr/sbin/mDNSRe
root               82   0.0  0.0  2469524   1648   ??  Ss   31Mar16   0:00.05 autofsd
root               81   0.0  0.1  2494032   2860   ??  Ss   31Mar16   0:05.13 /usr/sbin/blued
_locationd         78   0.0  0.2  2506468   6712   ??  Ss   31Mar16   1:05.60 /usr/libexec/loc
root               76   0.0  0.1  2496576   3532   ??  Ss   31Mar16   0:10.54 /usr/sbin/securi
_usbmuxd           75   0.0  0.0  2471648   2044   ??  Ss   31Mar16   0:02.52 /System/Library/
root               74   0.0  0.2  2496796   6832   ??  Ss   31Mar16   0:17.58 /System/Library/
root               73   0.0  0.0   657380    364   ??  Ss   31Mar16   3:26.29 /Library/Applica
root               72   0.0  0.2  2498504   9732   ??  Ss   31Mar16   0:31.24 /System/Library/
root               70   0.0  0.0  2473064   1772   ??  Ss   31Mar16   0:00.55 /usr/sbin/wirele
root               69   0.0  0.2  2510916   9024   ??  Ss   31Mar16   3:37.33 /usr/libexec/ope
root               68   0.0  0.0   430888   1576   ??  Ss   31Mar16   0:00.48 /usr/sbin/qmaste
root               60   0.0  0.0  2494736   1304   ??  Ss   31Mar16   0:00.76 /usr/libexec/dis
root               54   0.0  0.3  2590548  14668   ??  Ss   31Mar16   2:18.58 /System/Library/
root               53   0.0  0.1  2472080   4512   ??  SNs  31Mar16   0:00.49 /usr/libexec/war
root               51   0.0  0.1  2506000   4912   ??  Ss   31Mar16   2:56.66 /usr/libexec/air
root               48   0.0  0.0  2494844   1824   ??  Ss   31Mar16   0:15.18 /System/Library/
root               47   0.0  0.1  2500072   3780   ??  Ss   31Mar16   1:29.74 /usr/libexec/con
_appleevents       46   0.0  0.1  2496072   2764   ??  Ss   31Mar16   0:00.79 /System/Library/
root               44   0.0  0.1  2469012   4444   ??  Ss   31Mar16   0:03.32 /usr/libexec/the
root               42   0.0  0.0  2479564   1788   ??  Ss   31Mar16   1:22.99 /System/Library/
root               41   0.0  0.1  2496128   2208   ??  Ss   31Mar16   0:01.96 /usr/libexec/kex
root               39   0.0  0.0  2474528   1408   ??  Ss   31Mar16  10:47.56 /usr/sbin/syslog
root               38   0.0  0.3  2503676  13752   ??  Ss   31Mar16   1:20.41 /usr/libexec/Use
root                1   0.0  0.2  2482892   9232   ??  Ss   31Mar16   8:24.54 /sbin/launchd
donjohnson      66016   0.0  0.4  2497944  15528   ??  S    12:37PM   0:00.59 /System/Library/
root            65022   0.0  0.1  2452640   2804   ??  Ss   12:34PM   0:00.02 /usr/sbin/ocspd
donjohnson      64709   0.0  0.2  2474128   6672   ??  S    12:33PM   0:00.10 /System/Library/
donjohnson      64677   0.0  0.2  2474128   6468   ??  S    12:33PM   0:00.06 /System/Library/
donjohnson      61682   0.0  0.2  2493840   6972   ??  U    12:25PM   0:00.13 /System/Library/
root            59886   0.0  0.1  2469496   2364 s000  Us   12:21PM   0:00.17 login -pf donjoh
_spotlight      57453   0.0  0.2  2474860   6748   ??  S    12:14PM   0:00.04 /System/Library/
donjohnson      46603   0.0  1.2  3834840  49600   ??  Ss   11:46AM   0:02.65 /System/Library/
donjohnson      45262   0.0  1.8  3368912  75780   ??  S    11:42AM   0:11.33 /Applications/Go
donjohnson      42935   0.0  0.0  2493764   1896   ??  Ss   11:36AM   0:00.08 /System/Library/
donjohnson      42924   0.0  0.1  2469980   4332   ??  Us   11:36AM   0:00.03 /System/Library/
donjohnson      42560   0.0  1.6  4033432  68376   ??  Ss   11:35AM   0:22.63 /System/Library/
donjohnson      41873   0.0  0.4  2648316  18528   ??  S    11:33AM   0:04.23 /Applications/Su
donjohnson      39600   0.0  0.0  2493764   1892   ??  Ss   11:27AM   0:00.08 /System/Library/
donjohnson      39567   0.0  0.1  2541764   5580   ??  Ss   11:27AM   0:04.39 /System/Library/
donjohnson      39566   0.0  0.1  2469456   4324   ??  Ss   11:27AM   0:00.02 /System/Library/
donjohnson      39438   0.0  2.3  4233760  97096   ??  Ss   11:27AM   0:49.98 /System/Library/
donjohnson      34633   0.0  1.7  3525032  70252   ??  U    11:14AM   1:26.31 /Applications/Go
donjohnson      26371   0.0  0.2  2495124   7688   ??  S    10:52AM   0:00.05 /System/Library/
donjohnson      25608   0.0  0.1  2494984   3536   ??  S    10:50AM   0:00.12 /System/Library/
donjohnson      25467   0.0  0.0  2494288   1888   ??  Us   10:49AM   0:00.08 /System/Library/
donjohnson      25466   0.0  0.1  2469980   4328   ??  Us   10:49AM   0:00.02 /System/Library/
* Run `top` and review the results. (Hint: You may need to use `ctrl-c` to get out of this app.) *How do you interpret what you see here?*
Processes: 248 total, 3 running, 21 stuck, 224 sleeping, 1332 threads
12:36:51 Load Avg: 2.67, 2.31, 2.22
CPU usage: 28.90% user, 8.5% sys, 63.3% idle
SharedLibs: 12M resident, 12M data, 0B linkedit.
MemRegions: 54103 total, 1123M resident, 40M private, 320M shared.
PhysMem: 3946M used (1074M wired), 20M unused.
VM: 625G vsize, 1065M framework vsize, 518060(62) swapins, 848656(0) swa
Networks: packets: 1932068/1828M in, 1520803/282M out.
Disks: 1518209/33G read, 1831389/36G written.

PID    COMMAND      %CPU  TIME     #TH   #WQ  #PORT MEM    PURG   CMPRS
99085  awdd         0.0   00:00.16 2     0    62    16K    0B     1848K
85085  mapspushd    0.0   00:00.56 4     0    97    616K   0B     3188K
71150  Google Chrom 0.0   00:16.21 9     0    51    2384K  0B     22M
70100  nbstated     0.0   00:00.07 2     0    31    8192B  0B     1332K
69471  diskimages-h 0.0   00:00.14 3     0    65    16K    0B     6152K
65302  top          4.0   00:03.80 1/1   0    19    2280K  0B     0B
65022  ocspd        0.0   00:00.01 1     0    19    944K   0B     0B
64990  syncdefaults 0.0   00:00.84 4     0    104   8080K  0B     0B
64736  com.apple.ge 0.0   00:00.38 5     0    78    588K   0B     3040K
64709  mdworker     0.0   00:00.10 3     0    50    1764K  0B     0B
64677  mdworker     0.0   00:00.06 3     0    51    1568K  0B     0B
63703  recentsd     0.0   00:02.77 2     0    77    7296K  0B     5180K
62849  nsurlsession 0.0   00:16.17 4     0    112   4336K  0B     1384K

### Finding and Viewing Files

* Make sure you are in the `challenge_files` directory. Use the `*` wildcard to find all the files that have the word "credit" in the filename. *How many files did you find?*

* Use the `more` command to view one of the `credit_cards` files you just discovered. (Hint: Type `q` to quit viewing the file. Press the `spacebar` to page down. Use your keyboard arrows to move up/down.) *What is the date in the file you have viewed?*
~ $ more
Missing filename ("less --help" for help)
* Use the `find` command to search for files more effectively. Search the sub-directories under `challenge_files` to find the location of the file named `modi_laboriosam.txt`. *Where is that file located?*
~ $ find
usage: find [-H | -L | -P] [-EXdsx] [-f path] path ... [expression]
       find [-H | -L | -P] [-EXdsx] -f path [path ...] [expression]
* Use the `grep` command to search for text within a file. Use `grep` on all the `.user` files in `challenge_files` to find which files contain "WA" (the abbreviation for Washington state). *How many files did you find?*
~ $ grep
usage: grep [-abcDEFGHhIiJLlmnOoqRSsUVvwxZ] [-A num] [-B num] [-C[num]]
	[-e pattern] [-f file] [--binary-files=value] [--color=when]
	[--context[=num]] [--directories=action] [--label] [--line-buffered]
	[--null] [pattern] [file ...]
* Use the `-r` option of `grep` to *recursively* find the text "Waldo" hidden in a file somewhere under the `challenge_files` directory. *Paste the result showing the file and line where the word "Waldo" shows up.*

### Pipes and Connecting Commands

* Sometimes it's useful to output the results of a command to a text file for further analysis, reference, or processing. Try running `ls > files.txt`. Notice that the file `files.txt` was created. View that file using `more`. *What do you see in the `files.txt` file?*

* Notice that if you run `ls -alh` in the `challenge_files` directory, the files scroll by very quickly. Sometimes it would be better to get the results in a paginated format. Try running `ls -alh | more`. *Describe what you see when you run `ls -alh | more`.*
~ $ ls -alh | more
total 64
drwxr-xr-x+  28 donjohnson  staff   952B Apr 10 12:41 .
drwxr-xr-x    6 root        admin   204B Dec 25  2014 ..
-r--------    1 donjohnson  staff     7B Dec 25  2014 .CFUserTextEncoding
-rw-r--r--@   1 donjohnson  staff    10K Mar  8 18:45 .DS_Store
drwx------    9 donjohnson  staff   306B Mar  4 19:59 .Trash
drwxr-xr-x   12 donjohnson  staff   408B Jan  3 11:23 .atom
-rw-------    1 donjohnson  staff   243B Sep 13  2015 .bash_history
drwx------    4 donjohnson  staff   136B Feb  6 12:20 .config
drwx------    9 donjohnson  staff   306B Mar 31 20:50 .dropbox
drwxr-xr-x    3 donjohnson  staff   102B Feb  6 13:30 .freac
-rw-r--r--    1 donjohnson  staff   1.0K Feb  6 12:20 .gitconfig
drwxr-xr-x    3 donjohnson  staff   102B Sep 13  2015 .local
drwxr-xr-x    3 donjohnson  staff   102B Nov 22  2014 .mplayer
-rwxrwxrwx@   1 donjohnson  staff    41B Nov  8  2014 .orvkknhrc
drwx------    5 donjohnson  staff   170B Feb  6 12:20 .ssh
drwx------    4 donjohnson  staff   136B Oct 25 04:13 Applications
drwxrwxr-x@   3 donjohnson  staff   102B Mar  9 12:24 Creative Cloud Files
drwx------+ 113 donjohnson  staff   3.8K Apr  2 17:13 Desktop
drwx------+  14 donjohnson  staff   476B Dec  5 11:00 Documents
drwx------+ 229 donjohnson  staff   7.6K Mar 14 21:06 Downloads
drwx------@  49 donjohnson  staff   1.6K Mar 31 20:50 Dropbox
drwx------@  56 donjohnson  staff   1.9K Dec 17 20:23 Library
drwx------+   6 donjohnson  staff   204B Jul 22  2015 Movies
drwx------+   9 donjohnson  staff   306B Feb  6 12:10 Music
drwx------+   5 donjohnson  staff   170B Jul 22  2015 Pictures
drwxr-xr-x+   5 donjohnson  staff   170B Sep 27  2014 Public
-rw-r--r--    1 donjohnson  staff   160B Apr 10 12:42 files.txt
:
