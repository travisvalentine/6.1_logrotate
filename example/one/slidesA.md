!SLIDE center transition=scrollUp
# Logrotate #

!SLIDE subsection
# Pop quiz, hot shot #

!SLIDE bullets
# The scenario... #

* You put a ton of effort into building a great app
* It's fast
* It's tested

!SLIDE subsection
# Just one problem #

!SLIDE center transition=scrollUp
# The server is crashing #

!SLIDE bullets incremental
# WTF #

* Turns out the logs are too big
* There is no disk space as a result
* This causes the server to crash

!SLIDE subsection
# What just happened? #

!SLIDE center transition=scrollUp
# You forgot to rotate your logs #

!SLIDE center
# You're not alone #

* This is actually one of the most common ways a junior sys-admin can mess up a server.
* It's surprisingly easy to avoid.

!SLIDE subsection
# Enter logrotate #

!SLIDE transition=fade
# What Is It? #

* a utility to manage and administer log files
* most operating systems have it installed

!SLIDE bullets incremental
# How it Works #

* set up in a config file
* runs as a daily cron job
* takes what's in the log file
* copies the data into another file that is timestamped in a directory you specify
* older logs deleted after time

!SLIDE bullets incremental
# Features #

* rotated a number of times before getting deleted
* allows automatic rotation, compression, removal, and mailing of log files
* each log file may be handled daily, weekly, monthly, or when it grows too large
* will not  modify  a log  multiple  times  in  one  day unless that log is based on the log’s size and logrotate is being run multiple times  each day, or unless the -f or -force option is used.

!SLIDE subsection
# When isn't it useful? #

!SLIDE bullets incremental transition=scrollUp
# It's always useful #

* It's an easy way to stay organized and keep your logs manageable
* And therefore stay...performant?

!SLIDE center bullets
# Resources #

* Logrotate on [linuxcommand.org](http://linuxcommand.org/man_pages/logrotate8.html)
* Rails and logrotate