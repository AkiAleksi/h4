# h4

14.11.2023 klo 17:00

# x


A01:2021 – Broken Access Control 

-94% of applications were tested for some form of broken access control with the average incidence rate of 3.81%, and has the most occurrences in the contributed dataset with over 318k. 

-Notable Common Weakness Enumerations (CWEs) included are CWE-200: Exposure of Sensitive Information to an Unauthorized Actor, CWE-201: Insertion of Sensitive Information Into Sent Data, and CWE-352: Cross-Site Request Forgery.

-Access control enforces policy such that users cannot act outside of their intended permissions. Failures typically lead to unauthorized information disclosure, modification, or destruction of all data or performing a business function outside the user's limits.

-Access control is only effective in trusted server-side code or server-less API, where the attacker cannot modify the access control check or metadata.



* A10:2021 – Server-Side Request Forgery (SSRF)


-SSRF flaws occur whenever a web application is fetching a remote resource without validating the user-supplied URL. It allows an attacker to coerce the application to send a crafted request to an unexpected destination, even when protected by a firewall, VPN, or another type of network access control list (ACL). 
Access control vulnerabilities and privilege escalation 

-Access control is the application of constraints on who or what is authorized to perform actions or access resources. In the context of web applications, access control is dependent on authentication and session management: authentication, session management, access control.

-Broken access controls are common and often present a critical security vulnerability. 


* Server-side template injection


-Server-side template injection is when an attacker is able to use native template syntax to inject a malicious payload into a template, which is then executed server-side.

-Server-side template injection vulnerabilities can expose websites to a variety of attacks depending on the template engine in question and how exactly the application uses it. 

-Server-side template injection vulnerabilities arise when user input is concatenated into templates rather than being passed in as data.

* Server-side request forgery (SSRF)


-Server-side request forgery is a web security vulnerability that allows an attacker to cause the server-side application to make requests to an unintended location.

-A successful SSRF attack can often result in unauthorized actions or access to data within the organization. This can be in the vulnerable application, or on other back-end systems that the application can communicate with. In some situations, the SSRF vulnerability might allow an attacker to perform arbitrary command execution.

* Cross-site scripting


-Cross-site scripting (also known as XSS) is a web security vulnerability that allows an attacker to compromise the interactions that users have with a vulnerable application. It allows an attacker to circumvent the same origin policy, which is designed to segregate different websites from each other. Cross-site scripting vulnerabilities normally allow an attacker to masquerade as a victim user, to carry out any actions that the user is able to perform, and to access any of the user's data.

-Cross-site scripting works by manipulating a vulnerable web site so that it returns malicious JavaScript to users. When the malicious code executes inside a victim's browser, the attacker can fully compromise their interaction with the application.

17.11.2023 klo 19:58

a.)


Latasin oswap zapin.

<img width="611" alt="Screenshot 2023-11-17 at 20 01 55" src="https://github.com/AkiAleksi/h4/assets/112399816/699ca0c3-d41e-4e72-bef8-6a47082b7d76">

Ajoin java -jar <kohde> komennon. Se käynnistää zapin.

<img width="634" alt="Screenshot 2023-11-17 at 20 00 21" src="https://github.com/AkiAleksi/h4/assets/112399816/8aa49a76-1d9d-41e0-8b06-943bd2daab84">


Zap käynnissä

<img width="651" alt="Screenshot 2023-11-16 at 14 05 02" src="https://github.com/AkiAleksi/h4/assets/112399816/3c56d989-1215-4f49-b9a5-f1848741cc61">

localhost:8080 
Zap näkyy
Latasin sertifikaatin.






<img width="659" alt="Screenshot 2023-11-17 at 20 18 27" src="https://github.com/AkiAleksi/h4/assets/112399816/3df089aa-412b-487e-bc7f-1e8e6f454728">


importtasin sertifikaatin.



<img width="645" alt="Screenshot 2023-11-17 at 20 20 40" src="https://github.com/AkiAleksi/h4/assets/112399816/49d96942-2597-4162-a6fe-db40f6d3b41e">


Latasin Foxyproxyn


<img width="516" alt="Screenshot 2023-11-17 at 20 27 22" src="https://github.com/AkiAleksi/h4/assets/112399816/3a70d03b-31e7-4891-a4ef-6677ac83d17f">

Käynnistin sen


<img width="659" alt="Screenshot 2023-11-17 at 20 29 00" src="https://github.com/AkiAleksi/h4/assets/112399816/bc89e4f3-1386-4158-85b0-95dbc0266a5f">


Hain googlea 


<img width="654" alt="Screenshot 2023-11-17 at 20 31 31" src="https://github.com/AkiAleksi/h4/assets/112399816/d8a19575-52f0-4067-8866-ce36f0c29a5c">



Näkyy google haku näkyy Zap

<img width="554" alt="Screenshot 2023-11-17 at 20 11 23" src="https://github.com/AkiAleksi/h4/assets/112399816/d1084316-a849-453c-be11-5ebdab5ca161">




