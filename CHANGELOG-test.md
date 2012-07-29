# CHANGELOGS #

## Indexes ##
```
GET-xxx = Get Initial Cookbook from community
BUG-xxx = Bug Fix
FEA-xxx = Feature additions/Improvements
```

[[GET-001] Imported the community cookbook [ntp] (https://github.com/opscode/cookbooks/tree/master/ntp "NTP Cookbook")] (https://github.com/remotesyssupport/test/blob/master/CHANGELOG-test.md#get-001-imported-the-community-cookbook-ntp)  
__GET-001: Imported the community cookbook [ntp]__  
__GET-002__    
  __GET-002:BUG-001__   
  __GET-002:FEA-001__   


## Change Logs by Raghav ##

##### GET-001: Imported the community cookbook [ntp] (https://github.com/opscode/cookbooks/tree/master/ntp "NTP Cookbook") #####

* In essence  all debugging, security, audit, and authentication is founded on the basis of event correlation (knowing exactly what happened in what order, and on which side), and that depends on good time synchronization. Hence NTP is critically important
* This cookbook must be added to the base role, so that it is applied to all and any server started and configured with Chef

---------

##### GET-002: Imported the community cookbook [cron] (https://github.com/opscode/cookbooks/tree/master/cron "CRON Cookbook") #####

* To schedule any event like backup or internal security audits, Cron is required. The community cron cookbook works sufficiently well for this purpose

	######  Changelog for the cookbook ######
		 [GET-002:BUG-001] 01111
		 [GET-002:FEA-001] 0122334  
