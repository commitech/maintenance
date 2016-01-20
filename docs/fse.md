# FSE (Frequently Solved Errors)

Here are the common errors that are happening on our PCs.

## First things first

First things first, if the problem is a connection problem (e.g. can't login, can't access   internet), please try to unplug and plug back the Ethernet (LAN) cable on the computer.  
If that still doesn't fix the problem, try to restart the computer.  
If that still doesn't fix the problem, then read the rest of this document

## Trust relationship issue

If you see the following error

![](/images/trustissue.jpg)

TBA :p

`TODO (Jonathan) : Explain how to change domain thing`

## Can't install printer
Note: Do EVERYTHING below using admin access.

Press windows button on keyboard, right click on computer, choose Manage  
Open Services, wait for a while(it's loading)  
Right click on spooler, restart  
try connecting the printer again

If the first one doesn't work:  
Right click on spooler, stop  
open C:/windows/system32/spool  
delete SERVER, DRIVER, PRINTER(permanently by using shift+delete)  
restart the spooler service
try installing the printer again
