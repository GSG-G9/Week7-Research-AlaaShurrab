# Week7-Research-AlaaShurrab

## HTTP vs HTTPS:.

### How does HTTPS work?

- The HTTPS works almost the same as the HTTP but the maijor diffrence it that it adds a ssl leayer to the protocols leayers.

### What are TLS/SSL certificates?

- The SSL is a security technology that encrypts the data sent between the server & the browser, the encryption happens using two keys (public and private) the publicis for the user and the other is for the server.

### Why is this important to implement in your projects?

- it makes the connection between the server & the user more privet and makes it hard for the attacker to get the data.

### how to generate certificates and use them in a node project?

- first you must get a certificate signed by a trusted certificate authority (CA) on Certbot and they'll mack sure if you are a real server or a fake one.
- then its mostly like the http server you require the https from the root (const https = require("https")).
- then you read the file to create the keys and adding them to the options of the server.
- (~~there are a lot more in here to be written ~~ ).

## Stateless vs stateful authentication:.

### What is session based authentication (stateful) vs token based authentication (stateless)?

- the deffrence is that stateful is storing the info about the user in the database and the user gets the session id but the token is created then sent to the user with to check if the user changed his cookies.

### diagrams to show the steps involved in each process

- https://www.figma.com/file/SdWKY2H2BeubK7SGIEGqeO/Untitled?node-id=1%3A23

### What are the advantages and disadvantages of each?

- the session is more safe but is takes memory but the token is sent to the user 

## Attacks

### types of attack

### 1 - Man In The Middle (MITM)

- it is an interferance of an attacker to a connication between two other users while they think that the connection is safe so that he gets the data 

### 2 - Cross Site Scripting (XSS)

- it is to insert code in a website using any text field or the console with the intent to bypass the website authentication to get data.

### 3 - Cross Site Request Forgery (CSRF)

- it is to use a website vulnerability to send the users fake requists like (to change the password or or the email )thinking that they are from the real website and by doing them the attacer gets what he wants.

### How can you defend against each of them?

- man in the meddle attacke needs realtime connection and neeeds alot of stealth so let the mantinance team handel them the moment they are ditacted before they get any usful data
 
