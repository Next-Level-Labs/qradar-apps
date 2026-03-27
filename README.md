I have to catch up here !!! 

This is old, the architechture is probably still good for the realtime QRadar extension.

Its bassically a python connection from QRadar Alert I think, to my remote system running Debian Linux.
I would have used syslog-ng to peel in the data and redirect it to my palao aloto C plugin
that would access the Palo Alot API and make the apporitate firewall or "wehatever was API enabled"

Then the plugin would return the data and send it to ServiceNow and create a ticket in the right "area" 
grab the new ticket number and update the Qradar Interface with the "what" "Why" "How" and Ticket number.

I allowed for rollback when the analyst "ticket" was resolved

this was repeatable and configuarable in the QRadar GUI for any Alerts but, I only programmed Palo Alto API, they had good documentation.
Others would be asy to program into a template, such as Fortinet

I don't have any code and if I did it was QRadar 3.2 I think
