wol.bundle
===========================
Wake on LAN Plugin for Plex
===========================

SpacemanJT  - spacemanjt@yahoo.co.uk 02-06-16

Many thanks to the valuable contributions from the community in the development of this Plugin.

Basic Functionality: To send WAKE on LAN packets from the Plex Media Server to systems to be woken up.
This allows the user to bring online additional resources which might be turned off, such as DVR boxes,
NAS drives or other hosts of library content.

Please note that this Plugin does not wake the PMS from the client App. The PMS needs to be available.

This Plugin allows the user to configure up to 12 systems, which can be woken individually. Each system can be disabled, so that it doesn't appear on the list of systems that can be woken.

In addition the plugin supports up to three Wake-up Groups, where Wake requests can be sent to any of the specified 12 systems, even if the system is disable from appearing on the main list. Each Wake up group can be staggered to add a delay between machines of 0, 0.5,1 or 2 seconds.

The Plugin does its best to error check and where possible correct user preferences. Failures to send WOL requests are also reported and logged in C:\Users\Administrator\AppData\Local\Plex Media Server\Logs\PMS Plugin Logs or wherever your Plex server is located. Look for com.plexapp.plugins.wol

How to Use
==========
After installing the Plugin, configure its preferences.
1/ Edit System 1 and specify its MAC address - this is the most important piece of information
2/ Change the System 1 Friendly name to make it more useful - i.e. PC DVR
3/ Leave the Port at 7 for most networks and systems.
4/ Leave the broadcast IP address at 255.255.255.255 in most situations - this will broadcast the WOL packet on your local LAN. Specify a different IP address if you want the packet to go across a router or the internet, but bear in mind you will need a port forward active.
4/ Only one machine is enabled initially. Tick the box to enable more machines and then configure them if required.
5/ If you want to wake several machines in one go, select the option to add each machine to Group 1, Group 2, or both Groups.
6/ Each Group can also be given a friendly name
7/ Lastly, instead of trying to switch perhaps 10 machines on in literally one go, you may wish to add a small delay in between each request - select the option for each group for a staggering the machines.

Revision History:
 1.00 10-04-16 Initial Release
 1.01 10-04-16 Code tidied
 1.02 10-04-16 Added support for two WOL Groups and staggered startups
 1.03 10-04-16 Renamed the files in preparation for UAS submission
 1.04 14-04-16 Add Support for 1.5 second group delay; WOL Default Group Delay now 0.5 seconds instead of 0
               Additional logging information for the processing of preferences and Group WOL actions
               Tidied up some of the terminology - Systems not "enabled" can still be used in Group wake up
               so "enabled" has been replaced with "Show in List"
               Cured a bug where a system that was enabled, and specified to be used in a group but had
               invalid settings would still be added to the group wake up
 1.05 14-05-16 Changed the number of servers supported from 10 to 12
               Changed the number of groups from 2 to 3
 1.06 02-06-16 Changed graphics to use smaller JPG files to reduce loading times
 
