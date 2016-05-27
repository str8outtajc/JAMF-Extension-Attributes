#Extension Attributes for JAMF

by Jeffrey Compton

### Google Chrome Extensions

Displays Name, Version and ID of installed Google Chrome Extensions for current or last user. 

By default, data is displayed as: Name: Extension Name Version: Extension Version ID: Extension ID. 

However, if further data analysis is needed, an alternate output is available: Name;Version;ID 

The default output looks much prettier in the JSS, but the alternative output may be more useful. 

To use the alternate output, simply comment out line:

`echo -e "Name: $reportedName \nVersion: $version \nID: $extID \n" `

And uncomment line:

`echo -e "$reportedName;$version;$extID"`

