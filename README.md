------------------------------Instruction Set To Generate LocalHost Certificate with Key------------------

Place the req.cnf file in a folder. Change the content of the text file (req.cnf) if necessary. Then run the following command using openssl in the same folder.

openssl req -x509 -nodes -days 7300 -newkey rsa:2048 -keyout cert.key -out cert.pem -config req.cnf -sha256

It will generate a private key 'cert.key' and a certificate 'cert.pem' just like inside Certs folder. These files can be used in local server as SSL certificate and key.
