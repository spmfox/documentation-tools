# ssmtp

This is a quick cheat sheet for my scripts usage of ssmtp. Nothing fancy, just the bare minimum to send an email to a SSL enabled smtp server.

## Configuration Files

`/etc/ssmtp/ssmtp.conf`
```
mailhub=<domain.com:port>
UseTLS=YES
AuthUser=<user@domain.com>
AuthPass=<password>
FromLineOverride=YES
TLS_CA_File=/etc/pki/tls/certs/ca-bundle.crt
```

`/etc/ssmtp/revaliases`
```
root:user@domain.com:domain.com:port
```

## Usage
Create a text file:
```
To: email@domain.com
From: email@domain.com
Subject: <Subject>

<Message>
```

Run this command against the text file:
`sudo ssmtp email@domain.com < message.txt`
