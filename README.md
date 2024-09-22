# CrossSiteScripting-XSS-with-zap
## Objective
The objective of this project is to demonstrate the exploitation of Cross-Site Scripting (XSS) vulnerabilities within a website's input fields or URL parameters. The project aims to show how malicious scripts can be injected into web pages, enabling attackers to compromise user data, manipulate website content, or execute unauthorized actions on behalf of users. Through this project, key security concepts related to web application vulnerabilities are explored, along with mitigation strategies to prevent XSS attacks, such as input validation, encoding, and content security policies.

### Skills Learned
- Understanding of Cross-Site Scripting (XSS):In-depth knowledge of different types of XSS (Reflected, Stored, DOM-based).Awareness of how XSS vulnerabilities occur in web applications.
- Web Application Security:Identifying and exploiting security flaws in web applications.Understanding of security best practices, such as Content Security Policy (CSP), to prevent XSS.
- Injection Techniques:Crafting and injecting malicious scripts into vulnerable web applications.Understanding of how to execute scripts via URL parameters, form fields, or user inputs.
- Penetration Testing:Hands-on experience in ethical hacking techniques related to XSS.Use of tools such as Burp Suite, OWASP ZAP, or custom scripts to detect and exploit XSS vulnerabilities.

### Tools Used
- OWASP ZAP (Zed Attack Proxy) is an open-source web application security scanner used for finding vulnerabilities in web applications, such as XSS, SQL injection, and other common security flaws.
- Kali Linux is a Debian-based operating system designed specifically for penetration testing, digital forensics, and security research, offering a wide range of pre-installed security tools.

## Steps
- Open Kali and search for zaproxy and open it
- Now search for Bwapp.login.php (It is a vulnerable website for practice)
- ![Screenshot 2024-09-22 145951](https://github.com/user-attachments/assets/7fe6eae0-e2f1-4277-949f-33e0e6838b7c)
- As we are going with login page it is better to use a manual scan (passive scan)
- give the URL and Enable HUD(Heads up Display)
-  ![Screenshot 2024-09-22 150026](https://github.com/user-attachments/assets/0a08e89e-ac50-48e2-904f-9417dd1c28d1)
- tap on launch browser
- ![Screenshot 2024-09-22 150049](https://github.com/user-attachments/assets/e788830a-959e-474b-89ce-dcbbbd7ff22e)
- give user name as bee and password bug
- ![Screenshot 2024-09-22 150344](https://github.com/user-attachments/assets/c708140a-51af-439b-9f12-7a6a574f54d8)
- tap login
- ![Screenshot 2024-09-22 151410](https://github.com/user-attachments/assets/607b08cf-9edd-4d6f-82fc-e548cb9a09d6)
- Select portal to SQL injection (get/search)
![Screenshot 2024-09-22 151446](https://github.com/user-attachments/assets/e9d57062-3c58-4adb-8242-ba0a7a0c2ec4)
- Search for any movie and check for results. It shows no movies were found
- ![Screenshot 2024-09-22 151647](https://github.com/user-attachments/assets/5b6af590-7cf4-47fb-a970-c6905207851a)
- open zap and check the Request and Response of the search url
-  ![Screenshot 2024-09-22 151817](https://github.com/user-attachments/assets/557edd52-b89f-4079-9aff-e191de727e1a)
![Screenshot 2024-09-22 151837](https://github.com/user-attachments/assets/055abe35-2783-4ee4-8bfa-3241cd81145b)
- Now right click on url and start a active scan
- ![Screenshot 2024-09-22 151904](https://github.com/user-attachments/assets/e6cd5ab3-a251-464c-b86b-0da327eaaab9)
- attack is in process
- ![Screenshot 2024-09-22 153704](https://github.com/user-attachments/assets/18a20bcb-5d58-4831-bdaa-cfde76d63498)
- after the attack is done go to alerts and check for cross site scripting. It is present right click for details
- ![Screenshot 2024-09-22 160030](https://github.com/user-attachments/assets/bcdcb069-65a0-4776-8935-b89b93dcde90)
- copy attack details and place in "Search for Movies"
- ![Screenshot 2024-09-22 155719](https://github.com/user-attachments/assets/cefa62ec-e1fc-437a-bcf4-b73821d9d5bd)
- click search and then Boom!!
- ![Screenshot 2024-09-22 155655](https://github.com/user-attachments/assets/c4f25ff4-1098-4d66-ae2a-72d1066ffda9)

- 






















 
