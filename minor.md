## v2.0.0:  
**_`BUMPED UP THE VERSION AS A COMPLETE REFACTORING IS NEEDED`_**

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

   


## v1.0.0:

* [COOK-836] - use an attribute to specify the role to search for
  instead of relying on the rsyslog['server'] attribute.
* Clean up attribute usage to use strings instead of symbols.
* Update this README.
* Better handling for chef-solo.

