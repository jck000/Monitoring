###Status
[![Build Status](https://travis-ci.org/szabgab/Perl-Maven.png)](https://travis-ci.org/szabgab/Perl-Maven)


Monitoring web sites


Create a configuration file similar to the monitor-skel.yml
Run

    perl -Ilib bin/monitor.pl --config path/to/monitor.yml  --verbose

to check the web site and save the data.

Run

    perl -Ilib bin/email-report.pl --config path/to/monitor.yml --verbose

to send the reports.


Better yet, set up a cron-job

12 *  * * * (cd /path/to/dir; perl -Ilib bin/monitor.pl --config path/to/monitor.yml)

