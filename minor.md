## v2.0.0:  
**_`BUMPED UP THE VERSION AS A COMPLETE REFACTORING IS NEEDED`_**

* `[GET-003:FIX-001] - Rehaul rsyslog::default (standalone system logger)`
    * `[GET-003:FIX-001a]` - Remove support for old ubuntu systems.
    * `[GET-003:FIX-001b]` - Security Fix, drop privileges to `syslog:adm` from `root:root`.
    * `[GET-003:FIX-001c]` - Add default rules for ufw and postfix, to better support Ubuntu 12.04.
    * `[GET-003:FIX-001d]` - Add better handling of rsyslog.conf


## v1.0.0:

* [COOK-836] - use an attribute to specify the role to search for
  instead of relying on the rsyslog['server'] attribute.
* Clean up attribute usage to use strings instead of symbols.
* Update this README.
* Better handling for chef-solo.

