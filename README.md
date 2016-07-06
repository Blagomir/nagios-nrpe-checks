# nagios-nrpe-checks


List of nagios commands I usually include to monitor remote machines via NRPE


## [check_supervisord_program](plugins/check_supervisord_program)

Check the status of a single program executed and managed via supervisord
Usage: check_supervisord_program <program_name_here>
Notes: This script requires root privileges if your supervisord is running under root
To do this, you can add the following to your /etc/sudoers file (assuming your nrpe process is running with user nagios)
nagios ALL=NOPASSWD: /usr/bin/supervisorctl


## [check_linux_raid](plugins/check_linux_raid)

I can't take credit for this but it's really useful when you want to monitor your RAID array with nagios
 

## [check_postfix_queue](plugins/check_postfix_queue)

Useful to check your postfix mail queue