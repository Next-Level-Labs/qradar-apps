I have to catch up here !!! 

This is old, the architechture is probably still good for the realtime QRadar extension.

Its bassically a python connection from QRadar Alert I think, to my remote system running Debian Linux.
I would have used syslog-ng to peel in the data and redirect it to my Palo Alto API C plugin
that would access the Palo Alto API and make the apporitate firewall or "whatever was API available/enabled" by vendor.

Then the plugin would return the data from the API and send it to ServiceNow and create a ticket in the right "area" 
grab the new ticket number and update the QRadar Interface with the "what" "Why" "How" and Ticket number.  I think I may have created the ticket first before the Palo Alto API calls. 

I allowed for rollback when the analyst "ticket" was resolved from the QRadar GUI that would reverse the Firewall and update the Tickets.

This was repeatable and configuarable in the QRadar GUI for any Alerts but, I only programmed Palo Alto API at the time, they had good documentation.
Others would be asy to program into a template, such as Fortinet

I don't have any code and if I did it was QRadar 3.2 ish and would be outdated anyways.

