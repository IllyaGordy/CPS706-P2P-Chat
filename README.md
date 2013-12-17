CPS706 - Computer Networking 
P2P Chat Application

Group Members:
Julian Tompkins
Yuriy Demchuk
Illya Gordiyenko

How To Compile Application:
-------------
- 1.	Copy and paste all individual files into your eclipse workspace, creating classes for each specified file – PeerServer, DirectoryServer,ChatMain

Or

2.	Import the project into your eclipse workspace (Should be included in Zip File as SimpleChat)
How to run application:
1.	Execute the jar files received in the Zip file
Or
2.	Run the files directly from your eclipse workspace after importing them
Using the Application:
1.	Directory Server must be running initially before attempting to use the ChatMain file. Execute the DirServer.jar file first and click start, then execute multiple Chat.jar files.
2.	In the ChatMain menu, enter a username then click goOnline to join the directory server
a.	You may click goOffline to test if required
3.	Once you have joined the directory server you can now host a chat room.
a.	Enter the port for which you want to host a chat room on, and click host
4.	Two new windows should appear, (Peer to Peer server hosting on Port: X) and you should be connected in a chat room, capable of typing or disconnecting. 
a.	Clicking disconnect will return you to the main menu where you will have to input your information again
5.	At this point, execute another Chat.jar or ChatMain/Chat Client. Enter a new username and click goOnline.
6.	Attempt to use the query for peers button, the Host Servers and Online User fields should populate.
a.	NOTE: YOU WILL HAVE TO CLICK MULTIPLE TIMES ON THE QUERY FOR PEERS BUTTON – SPAM IT, IT SHOULD WORK EVENTUALLY. DO NOT PROCEED BEYOND THIS POINT IF YOU HAVE A CHAT ROOM CURRENTLY BEING HOSTED, BUT CANNOT SEE A HOST SERVER IN THE LIST OF HOST SERVERS.
7.	Once you see a user hosting a server in the Host Servers text field, (format should be: username R:X where X is the rating) you may now join that specific user.
8.	Enter the username of the person you see in the Host Server field into the text field next to the Join button. Click the Join button.
9.	You should now be in a chat room with that user, and be able to chat with him.
Key Notes:
-	You must be connected to the directory server to use the host button/query buttons/join buttons
-	You must query for peers and get all necessary information appearing in the text fields in order to use the join button.
-	Ratings are shown in the Host Servers text field next to the username (R:X).

Known Issues:
-	Directory Server/Client may crash if invalid input entered into text fields.
-	Query for Peers must be clicked multiple times in order for the text fields to be populated.
-	Ratings Update when user enters a chat room, but in some cases do not if a user disconnects the chat room.
-	Disconnecting the chat room to a point where it is empty will not close the peer to peer server associated with it
o	Also disconnecting the host will not close it either
o	Also disconnecting can result in the rest of the program to not function, I.E no new messages can be sent. It’s best to restart the program after you disconnect from a chat room.
-	No distinguishing between Hosting Users and Joining Users in directory server.
-	Disconnecting from a chat room results in the main chat menu restoring defaults instead of previously defined information.
-	Can host on the same port (results in error for instantiated peer server, but will result in user joining said chat room on specified port)
**** Not sure if this works on multiple computers, only works on a single computer.

