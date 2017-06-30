SocialAspProject:	Version v1.1
Author:			Sk Farhad
Development start: 	June 29, 2017
Location: 		Kurigram

URL: http://farhadasp01-001-site1.gtempurl.com/

Database info:
Hosting Account ID:	aspcareerfarhad-001
 FTP Address :		FTP.SMARTERASP.NET
 FTP Password :		skfarhadmay12,1989
Database name: 		db_9f3dca_webapp
DB login name:		9f3dca_webapp
DB password:		skfarhadmay12

Bug fixes/Improvements from v0:
1.	Real time messaging "updateMessage", fixing.

2.	Real-Messages storing in Database.

3.	Dulal line View of message list.

4.	Not-loggedin page request correcting (adding 'else' with 'if' in 
	NewMesssagePage.aspx.cs, inboxPage.aspx.cs).

5.	Real-time update from NewMesssagePage.aspx to inboxPage.aspx 
	(adding server+client methods to NewMesssagePage almost same as inboxPage)

6.	Background color improvement for all the pages.

7.	Special characters in ststus post.

8.	Special characters in real-time/stored message.
	
9.	Date time format matching in real-time/stored messages(Still some leading zero in stored messgses' time)

10.	Username validation in NewMessagePage.aspx with ajax+JavaScript methods.

11.	Not updating the message box for RT message if the receipient client is in other user's message page

12.	Fix for BUG1: not redirecting from NewMessagePage.aspx to inboxPage.aspx. Not leaving any if-else
	control open.
13.	REmoving all old build files and naming the assembly name as the root folder
	"empty_site" supressed some errors.
14.	Unhandled connection exception on hosted app was fixed by adding "using(){}"
	block to all the connection opening statements. This block handles connecton
	timeout exception by itself.

Found BUG list (development environment):

1. URT messages from IE and FF being updated like RT but is not being stored database. For chrome works fine.

BUGS on hosted app:

1. 	RunTime erron whenever reloading loggedIn.aspx for 2nd time .
	Okay for other pages.

2.	Error 1 seems to be fixed after some time.(Needs correction)

3.	Error 1 was due to unhandled open connection to the database. (14) is the 
	solution.

