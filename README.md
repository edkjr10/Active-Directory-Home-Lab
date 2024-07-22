# Active-Directory-Home-Lab

This lab shows off the creation of a virtual network that emulates a business domain managed by Active Directory.

The virtual machines involved are a Windows 2019 Server running Active Directory, an Ubuntu Server running Splunk Enterprise, a Windows 10 client PC, and a Kali Linux attacker PC.
Both Windows machines run Splunk Forwarder to send data to the Ubuntu Server.

![AD Lab (2)](https://github.com/user-attachments/assets/58495394-f649-4f92-9727-8e41e9e05005)

<h2>Domain Details:</h2>

<img width="607" alt="Domain" src="https://github.com/user-attachments/assets/6dba54b1-8c07-43a4-a153-eca1b67c998e">

Aside from the containers added on creation of the test.domain.com domain, Organizational Units for IT and HR were added to represent the IT and HR departments of a company.
A single user was added to each of these OUs as employees: Dennis Jenkins in IT, John Hancock of HR.

<img width="452" alt="djenkins" src="https://github.com/user-attachments/assets/057d20b6-d9be-4554-8ea1-961f3c3c8fb5">   <img width="446" alt="jhancock" src="https://github.com/user-attachments/assets/2c6c3997-184c-4842-8cf4-f3c53561bc52">

Each user in the domain must have complex passwords and follow the Default Password Policy:

<img width="443" alt="password policy" src="https://github.com/user-attachments/assets/46bd7fdb-b3a0-4750-afe6-52dca8b86504">

<h2>Client Machine:</h2>

The Windows 10 Client is configured to be a part of test.domain.com, allowing users to login.

<img width="300" alt="pc domain" src="https://github.com/user-attachments/assets/0c445098-7dca-40e3-b125-b6615652f184">

Both Dennis Jenkins and John Hancock can successfully log into the PC.

<img width="214" alt="djen login" src="https://github.com/user-attachments/assets/c454c3be-f917-4241-9da5-787a2f6301f2">   <img width="216" alt="jhan login" src="https://github.com/user-attachments/assets/bd98b8aa-7ec9-4a81-9b8e-adba9ce5617b">

<img width="300" alt="Profiles" src="https://github.com/user-attachments/assets/92d9f011-3f9e-4007-8e4e-f3a0073be717">

The client machine is still able to be properly configured by logging in with the local client account.

<img width="209" alt="Client1" src="https://github.com/user-attachments/assets/e4d1c867-a7a1-4676-a68b-50b9a42c1695">

