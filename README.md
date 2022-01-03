# Private-Key-Infrastructure-PKI

# Task 1

mkdir PKI
            cp "/usr/lib/ssl/openssl.cnf" "/home/seed/PKI/"
mkdir demoWK
cd demoWK
mkdir certs crl newcerts
echo 1000 > serial
gedit index.txt

            openssl req -new -x509 -keyout ca.key -out ca.crt -config openssl.cnf


Generating a 2048 bit RSA private key
writing new private key to 'ca.key'
Enter PEM pass phrase:

Verifying - Enter PEM pass phrase:
You are about to be asked to enter information that will be incorporated
into your certificate request.
What you are about to enter is what is called a Distinguished Name or a DN.
There are quite a few fields but you can leave some blank
For some fields there will be a default value,
If you enter '.', the field will be left blank.

            Country Name (2 letter code) [AU]:PK
            State or Province Name (full name) [Some-State]:PUNJAB
            Locality Name (eg, city) []:Sahiwal
            Organization Name (eg, company) [Internet Widgits Pty Ltd]:STC
            Organizational Unit Name (eg, section) []:STCS
            Common Name (e.g. server FQDN or YOUR name) []:
            Email Address []:elham@elham.com
            

![alt tag](https://github.com/shoaibqureshi6/Private-Key-Infrastructure-PKI/blob/main/1.1.jpeg)
![alt tag](https://github.com/shoaibqureshi6/Private-Key-Infrastructure-PKI/blob/main/1.2.jpeg)

# Task 2
             
            openssl genrsa -aes128 -out server.key 1024
            openssl rsa -in server.key -text



Private-Key: (1024 bit)
modulus:
            00:b9:a6:ae:c1:a1:db:0d:40:5b:1e:33:c7:85:d8:
            10:39:e2:ba:54:dd:0a:43:58:72:af:2c:12:ae:ba:
            9e:1a:47:f0:b9:62:70:3e:e7:0d:8d:32:57:a6:e5:
            8a:8d:8b:99:88:9f:5e:5d:2d:c2:95:b8:c1:d3:6e:
            f1:ba:69:9c:26:0e:be:0c:d6:48:db:b7:45:6b:ac:
            ef:43:f7:76:c8:46:0c:14:d8:fe:aa:39:ad:eb:c3:
            d4:73:51:b6:80:3f:50:60:a5:64:0a:c3:0f:ea:46:
            6e:5d:e9:1d:0a:f5:db:86:0f:bc:3e:19:15:ea:2b:
            1d:fd:b3:4a:1d:e7:9c:97:61

publicExponent: 65537 (0x10001)
privateExponent:

         6e:d5:ba:43:53:b4:09:47:40:9e:d9:5e:e6:e3:45:
            5c:a9:a5:80:80:ae:5d:e2:72:25:6e:74:80:e8:5c:
            f7:67:b7:a9:95:c1:59:6c:6b:c4:be:27:62:36:6b:
            ef:71:46:6a:30:6b:0f:c9:ff:ff:8e:db:f8:b4:a5:
            90:1a:f8:e3:21:62:0e:59:0b:12:5e:45:d8:99:ff:
            4a:11:2b:5c:b7:e5:e7:13:85:d8:2e:8d:fb:dd:f9:
            57:fd:b1:3f:5a:6b:cc:44:42:f2:cc:9e:e0:bb:54:
            51:b2:20:68:4b:87:c0:76:02:a6:6b:0d:9a:be:5b:
            28:ec:66:71:bf:89:09:d9

prime1:
            00:f6:af:cc:88:a5:79:bc:d2:f4:8c:29:50:18:ca:
            9d:65:2f:12:8e:76:e1:0e:ab:d3:8b:40:a0:73:cb:
            08:09:ee:bd:66:5c:1a:ca:9b:8f:f1:04:42:04:64:
            5d:7a:05:00:12:c2:02:42:6f:64:47:d8:ce:fe:1e:
            7b:e8:fa:4c:ef

prime2:
            00:c0:a8:fb:1f:b5:dd:29:12:25:ae:a6:ce:c4:a9:
            54:1d:f1:c1:c1:4e:2b:9f:b8:71:ba:a1:6b:92:a7:
            8f:52:08:34:36:34:00:fc:2c:4a:fb:85:37:5e:f8:
            2e:50:aa:cd:a9:4f:d6:cd:d1:3c:9e:b3:5b:8a:ff:
            a6:67:9e:00:af

exponent1:
            5e:8b:d6:5a:71:01:8d:8b:54:ca:fb:72:85:6d:f2:
            91:3b:4f:63:66:d0:af:2c:cf:f1:49:1d:b6:03:94:
            db:29:b3:51:ad:ef:5e:c3:ec:91:35:4e:90:1c:5f:
            6f:4a:c7:52:69:25:30:8d:3c:e4:04:86:a1:02:d1:
            fe:e3:1f:e5

exponent2:
            7a:26:a9:91:e1:6c:e7:ad:69:d6:e2:4c:16:c4:85:
            60:b6:f7:71:e8:6e:20:46:81:55:23:23:61:48:7b:
            c6:37:0d:63:90:75:4f:6d:85:dd:13:09:98:5d:22:
            80:62:cb:22:9e:4c:43:12:76:ac:e8:6b:12:26:25:
            0b:6d:52:61

coefficient:
            77:82:59:c8:6f:71:6c:3f:51:30:41:e9:70:f1:a6:
            3b:7d:ae:ae:5a:c3:e6:bf:fe:bc:43:9d:f0:2d:9d:
            63:fc:a4:45:be:da:4c:22:3d:b7:b3:1e:03:46:0b:
            cf:a2:ae:89:02:4b:99:af:9b:97:1d:89:6e:be:d6:
            15:90:a4:8c


![alt tag](https://github.com/shoaibqureshi6/Private-Key-Infrastructure-PKI/blob/main/2.1.jpeg)
![alt tag](https://github.com/shoaibqureshi6/Private-Key-Infrastructure-PKI/blob/main/2.2.jpeg)
![alt tag](https://github.com/shoaibqureshi6/Private-Key-Infrastructure-PKI/blob/main/2.3.jpeg)


# writing RSA key
-----BEGIN RSA PRIVATE KEY-----
            MIICWwIBAAKBgQC5pq7BodsNQFseM8eF2BA54rpU3QpDWHKvLBKuup4aR/C5YnA+
            5w2NMlem5YqNi5mIn15dLcKVuMHTbvG6aZwmDr4M1kjbt0VrrO9D93bIRgwU2P6q
            Oa3rw9RzUbaAP1BgpWQKww/qRm5d6R0K9duGD7w+GRXqKx39s0od55yXYQIDAQAB
            AoGAbtW6Q1O0CUdAntle5uNFXKmlgICuXeJyJW50gOhc92e3qZXBWWxrxL4nYjZr
            73FGajBrD8n//47b+LSlkBr44yFiDlkLEl5F2Jn/ShErXLfl5xOF2C6N+935V/2x
            P1przERC8sye4LtUUbIgaEuHwHYCpmsNmr5bKOxmcb+JCdkCQQD2r8yIpXm80vSM
            KVAYyp1lLxKOduEOq9OLQKBzywgJ7r1mXBrKm4/xBEIEZF16BQASwgJCb2RH2M7+
            Hnvo+kzvAkEAwKj7H7XdKRIlrqbOxKlUHfHBwU4rn7hxuqFrkqePUgg0NjQA/CxK
            +4U3XvguUKrNqU/WzdE8nrNbiv+mZ54ArwJAXovWWnEBjYtUyvtyhW3ykTtPY2bQ
            ryzP8UkdtgOU2ymzUa3vXsPskTVOkBxfb0rHUmklMI085ASGoQLR/uMf5QJAeiap
            keFs561p1uJMFsSFYLb3cehuIEaBVSMjYUh7xjcNY5B1T22F3RMJmF0igGLLIp5M
            QxJ2rOhrEiYlC21SYQJAd4JZyG9xbD9RMEHpcPGmO32urlrD5r/+vEOd8C2dY/yk
            Rb7aTCI9t7MeA0YLz6KuiQJLma+blx2Jbr7WFZCkjA==

-----END RSA PRIVATE KEY-----

![alt tag](https://github.com/Waleed-gif/Public-Key-Infrastructure-PKI-/blob/main/task2d.jpg)


           openssl req -new -key server.key -out server.csr -config openssl.cnf
  

Enter pass phrase for server.key:
You are about to be asked to enter information that will be incorporated
into your certificate request.
What you are about to enter is what is called a Distinguished Name or a DN.
There are quite a few fields but you can leave some blank
For some fields there will be a default value,

If you enter '.', the field will be left blank.

            Country Name (2 letter code) [AU]:PK
            State or Province Name (full name) [Some-State]:Punjab
            Locality Name (eg, city) []:sahiwal
            Organization Name (eg, company) [Internet Widgits Pty Ltd]:STC
            Organizational Unit Name (eg, section) []:STCS
            Common Name (e.g. server FQDN or YOUR name) []:SEEDPKILab2020.com
            Email Address []:elham@elham.com   

Please enter the following 'extra' attributes
to be sent with your certificate request
A challenge password []:abc123
An optional company name []:





          openssl ca -in server.csr -out server.crt -cert ca.crt -keyfile ca.key \
          -config openssl.cnf



Using configuration from openssl.cnf
Enter pass phrase for ca.key:
Check that the request matches the signature
Signature ok
Certificate Details:
              Serial Number: 4096 (0x1000)
              Validity
                  Not Before: Dec 24 12:21:24 2021 GMT
                  Not After : Dec 24 12:21:24 2022 GMT
              Subject:
                  countryName               = PK
                  stateOrProvinceName       = sahiwal
                  organizationName          = STC
                  organizationalUnitName    = STCS
                  commonName                = SEEDPKILab2020.com
                  emailAddress              = elham@elham.com
              X509v3 extensions:
                  X509v3 Basic Constraints: 
                      CA:FALSE
                  Netscape Comment: 
                      OpenSSL Generated Certificate
                  X509v3 Subject Key Identifier: 
                      AD:9A:79:05:6B:6C:6F:80:6E:1C:63:AA:9B:D9:9D:3E:7D:76:9B:00
                  X509v3 Authority Key Identifier: 
                      keyid:5B:83:26:FF:14:3F:D5:A8:C6:0C:55:D9:6D:02:81:3E:95:D8:C4:C5


Certificate is to be certified until Dec 24 12:21:24 2022 GMT (365 days)
Sign the certificate? [y/n]:y

1 out of 1 certificate requests certified, commit? [y/n]y
Write out database with 1 new entries
Data Base Updated
![alt tag](https://github.com/shoaibqureshi6/Private-Key-Infrastructure-PKI/blob/main/2.3.jpeg)


# Task 3
sudo vi /etc/hosts

        % cp server.key server.pem
        % cat server.crt >> server.pem
        openssl s_server -cert server.pem -www
        
        
![alt tag](https://github.com/shoaibqureshi6/Private-Key-Infrastructure-PKI/blob/main/3.1.jpeg)
![alt tag](https://github.com/shoaibqureshi6/Private-Key-Infrastructure-PKI/blob/main/3.2.jpeg)
![alt tag](https://github.com/shoaibqureshi6/Private-Key-Infrastructure-PKI/blob/main/3.3.jpeg)
![alt tag](https://github.com/shoaibqureshi6/Private-Key-Infrastructure-PKI/blob/main/3.4.jpeg)


# Task 4

        cd /var/www
        sudo mkdir seedpki
        sudo cp "/var/www/html/index.html" "/var/www/seedpki/"


![alt tag](https://github.com/Waleed-gif/Public-Key-Infrastructure-PKI-/blob/main/task4a.PNG)

          cd /etc/apache2/
          sudo mkdir ssl

![alt tag](https://github.com/Waleed-gif/Public-Key-Infrastructure-PKI-/blob/main/task4b.PNG)

          cp server.crt crt.pem
          cp server.key key.pem
          sudo mv "/home/seed/PKI/crt.pem" "/etc/apache2/ssl"
          sudo mv "/home/seed/PKI/key.pem" "/etc/apache2/ssl"


![alt tag](https://github.com/Waleed-gif/Public-Key-Infrastructure-PKI-/blob/main/task4c.PNG)

          cd /etc/apache2/ssl


          <VirtualHost *:80>
          ServerName seedpkilab2020.com
          DocumentRoot /var/www/seedpki
          DirectoryIndex index.html
          </VirtualHost>

![alt tag](https://github.com/shoaibqureshi6/Private-Key-Infrastructure-PKI/blob/main/4.1.jpeg)


          <VirtualHost *:443>
          ServerName seedpkilab2020.com
          DocumentRoot /var/www/seedpki
          DirectoryIndex index.html
          SSLEngine On
          SSLCertificateFile /etc/apache2/ssl/cert.pem
          SSLCertificateKeyFile /etc/apache2/ssl/key.pem
          </VirtualHost>

![alt tag](https://github.com/shoaibqureshi6/Private-Key-Infrastructure-PKI/blob/main/4.2.jpeg)

          // Test the Apache configuration file for errors
          $ sudo apachectl configtest
          // Enable the SSL module
          $ sudo a2enmod ssl
          // Enable the site we have just edited
          $ sudo a2ensite default-ssl
          // Restart Apache
          $ sudo service apache2 restart

![alt tag](https://github.com/shoaibqureshi6/Private-Key-Infrastructure-PKI/blob/main/4.3.jpeg)
![alt tag](https://github.com/shoaibqureshi6/Private-Key-Infrastructure-PKI/blob/main/4.4.jpeg)
