# sertificateForPushNotificationMergePemFile

cd ~/Desktop/keys/ 
openssl pkcs12 -clcerts -nokeys -out cert.pem -in cert.p12 
openssl pkcs12 -nocerts -out key.pem -in key.p12 
openssl rsa -in key.pem -out key.unencrypted.pem 
cat cert.pem key.unencrypted.pem > ck.pem
