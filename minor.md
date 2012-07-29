## v2.0.0:  
`Bumped up the version as a complete refactoring is needed`

* [GET-003:FIX-001] - rsyslog::default (standalone system logger) fixes.
	1 [GET-003:FIX-001a] - Remove support for old ubuntu systems.
	2 [GET-003:FIX-001b] - Security Fix, drop privileges to `syslog:adm` from `root:root`.
	3 [GET-003:FIX-001c] - Add default rules for ufw and postfix, to better support Ubuntu 12.04.
	4 [GET-003:FIX-001d] - Add better defintion to the service rsyslog



## v1.0.0:

* [COOK-836] - use an attribute to specify the role to search for
  instead of relying on the rsyslog['server'] attribute.
* Clean up attribute usage to use strings instead of symbols.
* Update this README.
* Better handling for chef-solo.

