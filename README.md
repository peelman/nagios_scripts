nagios_scripts
==============

Nagios scripts for a variety of uses

=== check_git.py ===

Used to do a check of a Git reposistory via Nagios' NRPE daemon. Will generate warnings when there are commits on `origin master` that aren't merged locally.

Was deemed necessary to remind forgetful admins to pull their changes onto servers after pushing to master.

Unfortunately, due to permissions, it will probably be necessary to set up a cron job to regularly do a `git fetch`.

