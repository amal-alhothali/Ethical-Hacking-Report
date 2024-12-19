# Ethical-Hacking-Report

<h2>Challenge 1: As a web penetration tester, the client asked you to find a vulnerability in the web
application. The machine has a suspicious user, under the home directory of that user there is a file
called flag.txt, get the file and display it's contents.  
Link: http://labmachine.ddnsking.com:8080/</h2>


-when I click the link this message appear:
![Screenshot (717)](https://github.com/user-attachments/assets/9d10d343-979e-476f-911d-0104afb8fe11)

-Then view page sourse and find a link then try to use it as a hint to reach to flag: 
![Screenshot (718)](https://github.com/user-attachments/assets/2d159108-6096-444e-9795-236d4a967944)

-when you open this link this page appear:
![Screenshot (721)](https://github.com/user-attachments/assets/e7751de0-103a-4408-a7b0-e34f1b969dd3)

-try to attempt to exploit the LFI vulnerability by manipulate input parameter to a web application in
a way reach the information of user accounts on the server:

![Screenshot (720)](https://github.com/user-attachments/assets/f9121de7-92ff-4f79-a64c-b79f9f0ce95b)

-Then I found the suspicious user to added it to the parameter and reached the flag:
![Screenshot (723)](https://github.com/user-attachments/assets/1d30d695-8554-48fe-8492-443fc48b3c14)


<h2>Challenge 2: A vulnerable service on the file-sharing server is running on a specific port; locate the
port and try to exploit the vulnerability.
Challenge IP: 64.225.93.192</h2>


-I used nmap tool to find out which service is running on a specific port of a server with this IP:
![Screenshot (724)](https://github.com/user-attachments/assets/991c49e2-e1e5-469e-abb5-99f4b1fbe505)

-Then use msfconsole to run Metasploit to run the module:
![Screenshot (725)](https://github.com/user-attachments/assets/c7a11434-d884-496c-b894-e99168fb03aa)

-Then configure it with the required options:
![Screenshot (726)](https://github.com/user-attachments/assets/39d42575-0e7d-49de-b89e-c7354d282f45)

-Then defined the rhosts by set after that run the exploit to exploit the vulnerability:
![Screenshot (727)](https://github.com/user-attachments/assets/21209341-f2ce-4852-b002-6dc56a99cf7a)

-I have opened a shell session and identified the location of the Bash shell:
![Screenshot (728)](https://github.com/user-attachments/assets/4ed26b5b-839e-408b-b388-ad7a45d9c024)

-Then finally I reached to the flag:
![Screenshot (729)](https://github.com/user-attachments/assets/b012fb7f-542e-4ed1-81c0-a1baaf47938a)


<h2>Challenge 3: The web developers made a simple web server, but they made a fatal mistake that
enables an attacker to exploit, find the vulnerability before a bad actor does!
Challenge link: http://labmachine.ddnsking.com/
</h2>


-I use wappalyzer extension to get some information about the server that is used to make this
website:
![Screenshot (730)](https://github.com/user-attachments/assets/0d70f3a1-a2da-4f15-a12e-df8f6f01164c)


-Then I used searchsploit to search for the server that has the vulnerability to examine and download
the exploit:
![Screenshot (731)](https://github.com/user-attachments/assets/0db6c326-65c9-483e-901a-ee093d000e32)
![Screenshot (732)](https://github.com/user-attachments/assets/3c7bea66-9701-4088-8438-929fed41e6dc)

-Used cat to examine the contents of the exploit module after it has been copied locally and used
chmod +x to make the exploit module executable, and then run the script directly:
![Screenshot (7344)](https://github.com/user-attachments/assets/a668a86e-9ce6-4e11-8ccd-ba4e6bfff60b)


-Then I found the flag:
![Screenshot (735)](https://github.com/user-attachments/assets/54379af0-c5cf-4eae-bb3e-3f700d892be7)



