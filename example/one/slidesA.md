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
You forgot to rotate your logs

!SLIDE center
# You're not alone #

* This is actually one of the most common ways a junior sys-admins can mess up a server.
* It's surprisingly easy to avoid.

!SLIDE subsection
# Enter logrotate #

!SLIDE transition=fade
# What Is It? #

* a utility to manage and administer log files
* most operating systems have it installed

!SLIDE bullets incremental
# How it Works #

* runs as a daily cron job
* takes what's in production.log
* puts it in another file that is timestamped in a directory you specify
* older logs deleted after certain time

!SLIDE bullets incremental
# Features #

* rotated a number of times before getting deleted
* options (daily, weekly, monthly, notifempty, compress, create…)
* I get a score, suggestions for improvement

!SLIDE subsection
# When isn't it useful? #

!SLIDE bullets incremental transition=scrollUp
# It's always useful #

* It's an easy way to stay organized and keep your logs manageable
* And therefore stay...performant?