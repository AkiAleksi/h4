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

Menin web security academyyn. Hakupyyntö ilmestyi Zapin käyttöliittymään.


<img width="766" alt="Screenshot 2023-11-18 at 15 26 11" src="https://github.com/AkiAleksi/h4/assets/112399816/363a5d62-c78c-40b2-9cd8-33bd695c2dd0">





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

<img width="568" alt="Screenshot 2023-11-18 at 14 03 38" src="https://github.com/AkiAleksi/h4/assets/112399816/a6187480-a036-4aac-931b-3d53491b715d">

<img width="618" alt="Screenshot 2023-11-18 at 14 04 13" src="https://github.com/AkiAleksi/h4/assets/112399816/260d825b-89f8-49e6-9a44-70fc5133ec53">






e.)

https://0a32007304ea7b9781cb52c4001c00b9.web-security-academy.net/image?filename=/etc/passwd


<img width="639" alt="Screenshot 2023-11-18 at 14 12 33" src="https://github.com/AkiAleksi/h4/assets/112399816/943f765c-7d87-44ab-8102-0bede4e3bf6e">


f.)

g.)

h.)

Menin tuotesivulle. Klikkasin check stock painiketta. 
Kyseinen pyyntö ilmestyi zappiin.

<img width="585" alt="Screenshot 2023-11-18 at 15 48 57" src="https://github.com/AkiAleksi/h4/assets/112399816/8c9d5a3e-e370-4c06-978e-b7af79da1716">

Pyynnössä näkyy stockApi. Klikkasin Request editoria kyseisen
pyynnön suhteen. Lähetin väärennetyn pyynnön stockApi=http://localhost/admin

<img width="456" alt="Screenshot 2023-11-18 at 15 50 17" src="https://github.com/AkiAleksi/h4/assets/112399816/f88279db-3952-4722-92eb-0f9fc7a7b155">

HTML:ssä näkyy kohta, jossa poistetaan carlos.


<img width="437" alt="Screenshot 2023-11-18 at 15 51 53" src="https://github.com/AkiAleksi/h4/assets/112399816/5db9246e-c6f0-4ecb-a82f-daffd83a17d2">





Annetaan väärennetty pyyntö stockApi=http://localhost/admin/delete?username=carlos
Lab solved!!

<img width="434" alt="Screenshot 2023-11-18 at 15 58 52" src="https://github.com/AkiAleksi/h4/assets/112399816/20d62486-6948-45c1-b157-7ddcea22861d">

i.)


<img width="444" alt="Screenshot 2023-11-18 at 16 41 29" src="https://github.com/AkiAleksi/h4/assets/112399816/41d80b11-814f-4013-9117-3907d64e65c9">





<img width="366" alt="Screenshot 2023-11-18 at 16 45 07" src="https://github.com/AkiAleksi/h4/assets/112399816/fc489d79-d77f-4b98-beb4-1ebee4ca0632">




<img width="424" alt="Screenshot 2023-11-18 at 16 44 21" src="https://github.com/AkiAleksi/h4/assets/112399816/63c26178-1b14-402a-a629-92017ada87fd">






<img width="440" alt="Screenshot 2023-11-18 at 16 44 35" src="https://github.com/AkiAleksi/h4/assets/112399816/b33b3bff-96db-4baa-97a8-dbc5f21c79ae">


