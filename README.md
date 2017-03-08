This is a self learning project to learn the basic ideas of socket programming. The server delivers the classic time-tested "knock knock" jokes. The client should play along, and if not the server will correct the client by sending a useful message. At a very basic level this is how most application layer protocols work i.e a mutual understanding between client and server.


The server code attaches a socket to a specified port and waits for an incoming TCP connection.
The client connects to the server at which point the server initiates the knock knock joke.

== Build & Run server ==
cd server
mvn package
java -cp target/server-1.0-SNAPSHOT.jar KnockKnockProtocol 4444


== Build & Run client ==
cd client
mvn package
java -cp target/client-1.0-SNAPSHOT.jar KnockKnockClient 127.0.0.1 4444

