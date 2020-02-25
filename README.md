# module-5-physics-SiruiSong
module-5-physics-SiruiSong created by GitHub Classroom
Client with physics engine is on port 12683. Client without physics engine listens on port 12682. There's a trouble when using isTCPSocketOpen() for the first startup agent to determine whether its client is on. So have to run the without physics engine first..
Press 1 to drop an object.

Have a problem:
I check isTCPSocketOpen() before sending a message in the updateWorld(), for the first-start agent, isTCPSocketOpen() is always false no matter the state of its client. But it can send messages if not checking isTCPSocketOpen() after the second agent running.
