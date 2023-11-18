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

b.)

Latasin Foxyproxyn


<img width="516" alt="Screenshot 2023-11-17 at 20 27 22" src="https://github.com/AkiAleksi/h4/assets/112399816/3a70d03b-31e7-4891-a4ef-6677ac83d17f">

Lisäsin proxyn





<img width="944" alt="Screenshot 2023-11-17 at 21 37 24" src="https://github.com/AkiAleksi/h4/assets/112399816/ffb5f90b-ee19-4b29-ac62-520a89774137">





Käynnistin sen


<img width="659" alt="Screenshot 2023-11-17 at 20 29 00" src="https://github.com/AkiAleksi/h4/assets/112399816/bc89e4f3-1386-4158-85b0-95dbc0266a5f">

Asetin proxyn


<img width="929" alt="Screenshot 2023-11-17 at 20 59 15" src="https://github.com/AkiAleksi/h4/assets/112399816/b369bb16-bff1-48a2-a776-eb7be3d2ed9f">

FoxyProxy toimii



<img width="382" alt="Screenshot 2023-11-18 at 12 05 06" src="https://github.com/AkiAleksi/h4/assets/112399816/fbc32ca9-f616-4e5a-ac64-de4f5a122c2d">




17.11.2023 klo 21:38

c.)

Live chat. chattasin sen jälkeen view transcript. 
Huomasin, että numeroitu txt file 2.txt

<img width="646" alt="chat" src="https://github.com/AkiAleksi/h4/assets/112399816/36b7d754-b407-47a3-9c05-bc945b1c4feb">

Katsoin kaappauksen zapista. Muokkasin pyyntöä.
Ensin laitoin 0.txt. En saanut mitään.
Sen jälkeen kokeilin 1.txt sain salasanan


<img width="908" alt="intercept" src="https://github.com/AkiAleksi/h4/assets/112399816/7e812faf-decd-48e2-b1f0-0ee7cbfc4f4f">

Kokeilin salasanaa ja se oli oikein.

<img width="678" alt="solved" src="https://github.com/AkiAleksi/h4/assets/112399816/15a93f0b-be10-4b6a-b2c6-2c838292240c">

Lab solved!!!

d.)

kaappaus

<img width="825" alt="rename" src="https://github.com/AkiAleksi/h4/assets/112399816/76ec9cb5-7c10-4b53-ae9e-6831586b2996">

/../../../../etc/passwd

<img width="266" alt="Screenshot 2023-11-18 at 12 34 38" src="https://github.com/AkiAleksi/h4/assets/112399816/e51534de-bea6-43a6-803a-8053ebf5ce37">

Lab solved


<img width="380" alt="Screenshot 2023-11-18 at 12 36 00" src="https://github.com/AkiAleksi/h4/assets/112399816/14b989d1-4c00-4189-982e-281fc791317b">

e.)

<img width="164" alt="uusxd" src="https://github.com/AkiAleksi/h4/assets/112399816/e32f1393-f0e3-4503-b058-c36d8f3b26cc">



<img width="275" alt="Screenshot 2023-11-18 at 13 36 55" src="https://github.com/AkiAleksi/h4/assets/112399816/3aed873e-9213-40e3-976a-b1f6586e08ca">

f.)


