# Security attack
## Recall
Recall that there are different cloud layer in CC.
  
    1) SaaS
    2) PaaS
    3) IaaS
    
## Objective
In this artcile, I will simply discuss the security attack in each cloud layer.

Let's get started.

## Security attack on SaaS cloud layer
It involves:

1) Dos attack and its extension.

For more details, see my notes.

2) Authecation attack.
    
        The core concepts of this attack involves the approaches to target the mechanism which is used by the user to authencate the system.
        
        The approaches includes 
        
        2.1) All ways to guess the user's account and password of administrator such as brute-force etc. 
        2.2) Social engineering. Use social engineering to lower the users worriness, easily provides the account and password to the attacker.

        Once attacker get the user's account and password. Attacker can grant the administrator privilege in system, performing some scaring operation in terminal 
        (such as installing malware packages etc).
        
        For example, in Linux system, to enter the root account, just type these command in terminal.
        
        sudo -i
        
        Then the system will require your password.
        
        What happen if your password is stolen? 
        
        you should know.
        
3) SQL-injection attack

For more details, see my notes.

## Security attack on PaaS cloud layer
It involves

1) Phisihing attack
    
        Phishing refers direct the user into a fake website (and of course, mislead the user the website is safe), misleading the user input sensitive information in the fake website.
        
        Here, some readers may think it is easy to recognize a website is fake or not. Just very careful to the url.
        
        NOPE!!! 
        
        It is NOT easy.
        
        However, there are some features of a fake website. We can according to them to filter some phishing websites.
        
        Before continue reading, I recommend you to spend some time on thinking that if you are an attack how to make a fake website and seems to be an unfake website 
        
        for the user.
        
        Here, I list some features of a phishing website and prevent phishing attack as possible.
        
        1.1) First, the url of a phishing website looks like the url of  atcual website but NOT same.
        
        Take google webbrowser as example.
        
        In google webbrowser, the actual url is "https://www.google.com.tw/"
        
        Someone may register an url "https://www.goog1e.com.tw"
        
        NOTE that there are slightly difference between them. Tha latter url contains "goog1e" instead of "google". 
         
        To prevent to visit phishing websites, check the url carefully before visiting.
        
        1.2) Second, a phishing website will require some unnecessary information.
        
        For example, when you want to reset the password of the Google Email, it will require your email account or your telephone etc.
        
        It will NOT require information about your ID card and your bank account and password.
        
        Thus, once they are required when you reset the password of the Google Email, you have to caution. You visit a phishing website.
        
        Caution to required information.
        
        1.3) Finnally, in a phishing website, some anormal things may occur.
        
        Such as, when you reset password in Google Email, whatever the account you entered, it always say it is wrong or correct.
        
        If the above situation occur, it must be a phishing website. (... and you're too late to caution. ...)
        
        
2) port scanning attack.        

To fully understand about port scanning attack, I recommend you to comprehend these temrs <b>port</b> and <b> scanning attack</b>

Scanning attack refers attacks from scanning on cloud.

Look at the following figure.

![image](https://user-images.githubusercontent.com/75050655/227419603-2427f44b-4b68-434c-84ba-01de7b0d8554.png)


### Ref
https://www.geeksforgeeks.org/what-are-scanning-attacks/


Before introducing the term, let's quick review some basic knowledge about sending a packet in TCP.

![image](https://user-images.githubusercontent.com/75050655/227423222-1bbcd7e4-d3c2-4a7b-8145-2c2dd79ac001.png)

Look at the above figure.

To send a package from client to server in TCP. It uses the three-hand way.

    1) The client must send SYN request to the server.
    2) The server will response the SYN also request ACK to client.
    3) The client will response ACK to server.

### Ref
https://en.wikipedia.org/wiki/Transmission_Control_Protocol

### Intro
The port scanning attack refers the attack involved port scanning.

The attacker may scanning some ports and request to target to connect with the target, then sneak to perform some operations 

such as download and install malware etc.

![image](https://user-images.githubusercontent.com/75050655/227420234-511b157f-d889-4986-b1c8-7009ce7721d0.png)

### Prevention

To prevent port scanning attack, as a user, we can built secured firewalls and apply strong security mechanism.


![image](https://user-images.githubusercontent.com/75050655/227430105-668b1d20-8ea5-4d13-90fe-17913c188dbb.png)

### Ref
https://www.geeksforgeeks.org/port-scanning-attack/

3) Man-in-middle attack

### Intro
In this attack, the attacker may intercept the message while transferring.

### Prevention
To prevent this, just use a safely algorithm to encrypt the message into ciphertext before transferring.

By doing this, if the attacker intercepts successfully, then one will get its ciphertext. To get plaintext, one must decrypt it.

NOTE that:
  
    1) safely algorithm refers the algorithm which, for any ciphertexts, it can NOT must decrypt in available time (such as in NP time).
    


### My Notes

For more details about encryption and decryption, see my notes or study information security (中文譯:資訊安全) or cryptography (中文譯:密碼學).

https://github.com/40843245/Information_Security/blob/main/Basic%20knowledgement/process%20of%20encryption%20and%20decryption.md

4) Metadata spoofing attack

### Intro

Metadata refers <b>data about data</b>

Typically, metadata store sensitivie data.

The major step of this attack is 

    1) spoofing the metadata
    2) read the metadata and gain important sensitive data.
        
![image](https://user-images.githubusercontent.com/75050655/227442667-da1eedc7-6260-495f-9344-e41381838155.png


        
        

    

