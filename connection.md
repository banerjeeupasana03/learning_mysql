### How to set up mySQL clients?
For connecting to mySQL the best way is by mycli
Similar to `mycli` there is another mySQL client called `mysql`

To install mycli in MAC with homebrew
```sh
brew install mycli # to install mycli
command -v mycli # to check whether mycli is installed
```

To install telnet
```sh
brew install telnet # to install telnet
```

### How to connect to mySQL server using mySQL clients?
To connect using a mySQL client first you need the "End point" of the mySQL server.
If you are running the mySQL server on your local machine that End point is `localhost`
The default port of mySQL server is `3306`.

```sh
# dig is a tool that verifies dns(domain name servers) entries.
# The domain name of the end point you provide should return back an ANSWER SECTION
# If there is no ANSWER SECTION then the end poimnt you have provided is wrong. 
dig <endpoint>

# Telnet is a tool that checks connections to servers on port number.
# The port number for mySQL servers is 3306
# If that port is open on the end point then telnet will connect when you  run the command, 
# Otherwise telnet will timeout indicating that the port is not open on the server.
telnet <end point> 3306 # To check the connection

# mycli is a tool which is used to run commands on the mySQL server
mycli -h <End point> -u <username of database> # To connect to mySQL server
```
