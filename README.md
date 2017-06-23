# Media-Server using TCP 

1. Server Dependencies
a. My SQL
Install MYSQL DataBase-- Command -- sudo apt-get install mysql-server


2. Client Dependencies
a. GTK 
Install gtk library -- command -- sudo apt-get install libgtk2.0-dev
build gtk -- command -- sudo apt-get build-dep gedit
b. VLC


Server Compile and run
gcc -o 13_server 13_server.c $(mysql -config --cflags) $(mysql -config --libs) -lpthread

Client Compile and run
gcc -o 13_client 13_client.c `pkg-config --libs --cflags gtk+-2.0` -lpthread