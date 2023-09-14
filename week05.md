# Week 5 | INTERNET APPLICATIONS

## Task 1. Create Web Pages in OpenWRT
 
This is the example web page 

Note: index.html file attached.

![Examp](./images/Exampl.png)


Note: 12202930.html file and mystyle.css file are attached.


![week05](./images/week05.png)

![DateTime](./images/DateTime.png)


## Task 2. Capture HTTP Packets


I  used Get-NetNeighbor powershell command to view the ARP table for my physical interface.

My current ARP Table details :

![ARPTable1](./images/ARPTable1.png)

![ARPTb2](./images/ARPTb2.png)

![ARPTB3](./images/ARPTB3.png)

Based on the above ARP Table details, I have identified several devices that can reachable by my computer. It has mentioned the states of those devices are Permanent and Reachable.


I captured 29 packets and it's saved into 12202930.pcap file

Note: 12202930.pcap file attached.

![pack29](./images/pack29.png)

12202930.pcap file transfer to windows machine through the filezia

![savefile](./images/savefile.png)




12202930.pcap  packet capture opens through  wireshark

![mypackets](./images/mypackets.png)




## Task 3. Analyse HTTP Packet Capture

![http](./images/http.png)

### 3-a

1. First Request and Response - The user clicked http://192.168.56.2/ which caused the browser to send an HTTP request for index.html. The server does have that page.
2. Second Request and Response - The user clicked http://192.168.56.2/ which caused the browser to send an HTTP request for /12202930.html.
3. Second Request and Response - The browser sends a HTTP request asking for /mystyle.css which is linked with /12202930.html. The server does have that file.


### 3-b


### 3-c

The browser didn't send a request to the web server when the user clicked on the button to show the date and time. The reason behind that was I have implemented the 'onclick' HTML attribute. It is used to specify the JavaScript Date() function that should be executed when a user clicks on the button. This code is executed on the client side, within the user's web browser, and does not involve sending a request to the server.


### 3-d : Packet Diagram

## Task 4. View Your Cookies

Website: https://my.cqu.edu.au/login

![cookies](./images/cookies.png)

1.Session Information: Cookies often store a unique session identifier or token that helps the website recognize as a logged-in user during  visit.

2.Preferences: Cookies may store information related to preferences on the website, such as language preferences, display settings, or customized layouts. This allows the website to provide you with a more personalized experience.

3.User-Generated Data: Povided information on a website, such as filling out a form with  name, email address, or other details, cookies  store this data temporarily to facilitate the submission process.



