# CHANGELOGS #

## ChangeLogs [Raghav] ##
###### * Imported the community cookbook [ntp] (https://github.com/opscode/cookbooks/tree/master/ntp "NTP Cookbook") ######
	* The importance of ntp (time synchronization service) stems from the fact that  all debugging, security, audit, 
	and authentication is founded on the basis of event correlation (knowing exactly what happened in what order, and 
	on which side), and that depends on good time synchronization.
	* This cookbook must be added to the base role, so that it is applied to all and any server started and configured
	 with Chef
