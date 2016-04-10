wol.bundle
===========================
Wake on LAN Plugin for Plex
===========================

Many thanks to the valuable contributions from the community in the development of this Plugin.

Basic Functionality: To send WAKE on LAN packets from the Plex Media Server to systems to be woken up.
This allows the user to bring online additional resources which might be turned off, such as DVR boxes,
NAS drives or other hosts of library content.

Please note that this Plugin does not wake the PMS from the client App. The PMS needs to be available.

This Plugin allows the user to configure up to 10 systems, which can be woken individually. Each system can be disabled, so that it doesn't appear on the list of systems that can be woken.

In addition the plugin supports up to two Wake-up Groups, where Wake requests can be sent to any of the specified 10 systems, even if the system is disable from appearing on the main list. Each Wake up group can be staggered to add a delay between machines of 0, 0.5,1 or 2 seconds.

The Plugin does its best to error check and where possible correct user preferences. Failures to send WOL requests are also reported and logged in C:\Users\Administrator\AppData\Local\Plex Media Server\Logs\PMS Plugin Logs or wherever your Plex server is located. Look for com.plexapp.plugins.wol

Revision History:
 1.00 10-04-16 Initial Release
 1.01 10-04-16 Code tidied
 1.02 10-04-16 Added support for two WOL Groups and staggered startups
 1.03 10-04-16 Renamed the files in preparation for UAS submission
 
