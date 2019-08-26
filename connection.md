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
mycli -h <End point> -u <username of database>
```
