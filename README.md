# Messaging App

Nicholas Maltbie

Example messaging app made using Docker, React, Rest, RabbitMQ, and PostgreSQL.

# Goals

Make a messaging app where a user can either join or create a room.
The user should be prompted to make a name when joining or creating
a room and the program should ensure that each name in the room
is unique. 

While in the room, users will send their messages as POST requests to the server.
Once the users sends their message to the server, the server will enter the
message into a queue that all other users in the room are listening to.

Messages will be logged in the database and when a new user joins a room they
will be sent the message log from the database. This sums up the basic flow
of this application.
