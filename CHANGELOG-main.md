# CHANGELOGS #

## Indexes ##
```
GET-xxx = Get Initial Cookbook from community
BUG-xxx = Bug Fix
FEA-xxx = Feature additions/Improvements
```

## Change Logs by Raghav ##

##### [GET-001] Imported the community cookbook [ntp] (https://github.com/opscode/cookbooks/tree/master/ntp "NTP Cookbook") to vendor-cookbooks #####

* In essence  all debugging, security, audit, and authentication is founded on the basis of event correlation (knowing exactly what happened in what order, and on which side), and that depends on good time synchronization. Hence NTP is critically important
* This cookbook must be added to the base role, so that it is applied to all and any server started and configured with Chef

---------

##### [GET-002] Imported the community cookbook [cron] (https://github.com/opscode/cookbooks/tree/master/cron "CRON Cookbook") to vendor-cookbooks #####

* To schedule any event like backup or internal security audits, Cron is required.
* The community cron cookbook works sufficiently well for this purpose

--------

##### [GET-003] Imported the community cookbook [rsyslog] (https://github.com/opscode/cookbooks/tree/master/rsyslog "CRON Cookbook") to cookbooks ####

* Rsyslog server-client setup is chosen for the Centralized Logging System
* The initial import of the community cookbook is done only for historical purposes and for tracking/changelog.
* The community cookbook *__`DOESNOT`__* satify most of our requirements, so completely refactoring it. Please check the ChangeLog below:
