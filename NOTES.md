# CHANGELOGS #

## Indexes ##
```
BUG-xxx = Bug Fix
FEA-xxx = Feature additions/Improvements
GET-xxx = Get Initial Cookbook from community
REM-xxx = Remove a feature
```

## Change Logs by Raghav ##

##### `[GET-001]` Imported the community cookbook [ntp] (https://github.com/opscode/cookbooks/tree/master/ntp "NTP Cookbook") to vendor-cookbooks #####

* In essence  all debugging, security, audit, and authentication is founded on the basis of event correlation (knowing exactly what happened in what order, and on which side), and that depends on good time synchronization. Hence NTP is critically important
* This cookbook must be added to the base role, so that it is applied to all and any server started and configured with Chef

---------

##### `[GET-002]` Imported the community cookbook [cron] (https://github.com/opscode/cookbooks/tree/master/cron "CRON Cookbook") to vendor-cookbooks #####

* To schedule any event like backup or internal security audits, Cron is required.
* The community cron cookbook works sufficiently well for this purpose

--------

##### `[GET-003]` Imported the community cookbook [rsyslog] (https://github.com/opscode/cookbooks/tree/master/rsyslog "CRON Cookbook") to cookbooks ####

* Rsyslog server-client setup is chosen for the Centralized Logging System
* The initial import of the community cookbook is done only for historical purposes and for tracking/changelog.
* The community cookbook *__`DOESNOT`__* satify most of our requirements, so completely refactoring it. Please check the ChangeLog below:

	###### **_`COMPLETE REFACTORING OF COOKBOOK RSYSLOG - CHANGELOG`_** ######
	* `[GET-003:FIX-001] - Rehaul rsyslog::default (standalone system logger)`
		* `[FIX-001:REM-001]` - Remove support for old ubuntu systems.
		* `[FIX-001:FIX-001]` - Security Fix, drop privileges to `syslog:adm` from `root:root`.
		* `[FIX-001:FIX-002]` - Add better handling of rsyslog.conf
		* `[FIX-001:FEA-001]` - Add default rules for ufw and postfix, to better support Ubuntu 12.04.
		* `[FIX-001:FEA-002]` - Log rotation via logrotate

	* `[GET-003:FIX-002] - Rehaul rsyslog::server`
		* `[FIX-002:REM-001]` - Remove dependency on cron
		* `[FIX-002:REM-002]` - Remove old remote server based configs
		* `[FIX-002:FIX-001]` - Security Fix, drop privileges to `syslog:adm` from `root:root`.
		* `[FIX-002:FEA-001]` - Adding support for Client Host per Directory Logging
		* `[FIX-002:FEA-002]` - Add support for audit.log

