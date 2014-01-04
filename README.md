nagios-plugins
==============

Nagios Plugins
## check_crashplan
This script checks Crashplan backups on linux.  It will check for inprogress backups as well as completed backups.  This is useful if there is a large backup running and you want to alert differently vs. alerting only on completed backups.  Critical alerts: if the inital backup is not done, if there is a backup older than critHours, or there is a backup in progress but no completed backup within critHours, or if there is a backup in progress that has stagnated for 1 hour (could be changed to a variable in a later release)

