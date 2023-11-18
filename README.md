# h4

14.11.2023 klo 17:00

# x


A01:2021 – Broken Access Control 

-94%:sta sovelluksista testattiin jollain tavalla rikkoutuneen pääsynhallinnan varalta keskimääräisen ilmenevyysasteen ollessa 3.81%, ja se esiintyi eniten osallistuneessa datasetissä yli 318 000 kertaa. 

-Huomionarvoisia yleisiä heikkouksien luettelointeja (CWE) ovat CWE-200: Herkkien tietojen paljastuminen valtuuttamattomalle toimijalle, CWE-201: Herkän tiedon lisääminen lähetettyihin tietoihin ja CWE-352: Ristiinsivustoista pyyntöjen väärentämistä.

-Pääsynhallinta toteuttaa käytäntöjä niin, että käyttäjät eivät voi toimia oman tarkoitetun käyttöoikeutensa ulkopuolella. Epäonnistumiset johtavat yleensä valtuuttamattomaan tietojen paljastumiseen, muokkaamiseen tai tuhoamiseen, tai käyttäjän rajojen ulkopuolisen liiketoimintatoiminnon suorittamiseen.

-Pääsynhallinta on tehokasta vain luotetussa palvelinpuolen koodissa tai palvelimetöntä API:ta käytettäessä, missä hyökkääjä ei voi muokata pääsynhallinnan tarkistusta tai metadataa.



* A10:2021 – Server-Side Request Forgery (SSRF)


-SSRF-haavoittuvuudet ilmenevät aina, kun verkkosovellus noutaa etäresurssia ilman käyttäjän toimittaman URL-osoitteen validoimista. Se mahdollistaa hyökkääjän pakottaa sovelluksen lähettämään muokatun pyynnön odottamattomaan kohteeseen, vaikka se olisi suojattu palomuurilla, VPN:llä tai toisentyyppisellä verkon pääsynhallintalistalla (ACL). Pääsynhallintahaavoittuvuudet ja oikeuksien laajennukset



* Server-side template injection


-Palvelinpuolen mallinjäykkäys tapahtuu, kun hyökkääjä pystyy käyttämään alkuperäistä mallisyntaksia upottaakseen haitallisen kuormituksen malliin, joka suoritetaan sitten palvelinpuolella

-Palvelinpuolen mallinjäykkyyshaavoittuvuudet voivat altistaa verkkosivustot monenlaisille hyökkäyksille riippuen kyseessä olevasta mallimoottorista ja siitä, miten sovellus tarkalleen ottaen sitä käyttää.

-Palvelinpuolen mallinjäykkyyshaavoittuvuudet syntyvät, kun käyttäjän antama syöte yhdistetään malleihin sen sijaan, että se siirrettäisiin dataksi.

* Server-side request forgery (SSRF)


-Palvelinpuolen pyynnön väärentäminen on verkkoturvahaavoittuvuus, joka mahdollistaa hyökkääjän aiheuttaa palvelinpuolen sovelluksen tekemään pyyntöjä ei-tarkoitetulle sijainnille.

-Onnistunut SSRF-hyökkäys voi usein johtaa valtuuttamattomiin toimiin tai pääsyyn tietoihin organisaatiossa. Tämä voi tapahtua joko haavoittuvassa sovelluksessa tai muissa taustajärjestelmissä, joiden kanssa sovellus voi viestiä. Joissakin tilanteissa SSRF-haavoittuvuus saattaa mahdollistaa hyökkääjän suorittaa mielivaltaisia komentoja.

* Cross-site scripting


-Cross-site scripting (tunnetaan myös nimellä XSS) on verkkoturvahaavoittuvuus, joka mahdollistaa hyökkääjän vaarantaa vuorovaikutukset, joita käyttäjillä on haavoittuvan sovelluksen kanssa. Se sallii hyökkääjän kiertää samaa alkuperäisperiaatetta, joka on suunniteltu erottamaan eri verkkosivustot toisistaan. Cross-site scripting -haavoittuvuudet mahdollistavat yleensä hyökkääjän teeskennellä uhriksi joutunutta käyttäjää, suorittamaan mitä tahansa toimintoja, joita käyttäjä voi tehdä, ja saamaan pääsyn kaikkiin käyttäjän tietoihin.

-Cross-site scripting toimii manipuloimalla haavoittuvaa verkkosivustoa niin, että se palauttaa käyttäjille haitallista JavaScript-koodia. Kun haitallinen koodi suoritetaan uhrihenkilön selaimessa, hyökkääjä voi täysin vaarantaa heidän vuorovaikutuksensa sovelluksen kanssa.

17.11.2023 klo 19:58

a.)


Latasin oswap zapin. Valitsin tuon toisiksi alimmaisen.

<img width="611" alt="Screenshot 2023-11-17 at 20 01 55" src="https://github.com/AkiAleksi/h4/assets/112399816/699ca0c3-d41e-4e72-bef8-6a47082b7d76">

navigoin cd /usr/share/zaproxy/
Sen jälkeen ajoin java -jar <kohde> komennon. Se käynnistää zapin.

<img width="634" alt="Screenshot 2023-11-17 at 20 00 21" src="https://github.com/AkiAleksi/h4/assets/112399816/8aa49a76-1d9d-41e0-8b06-943bd2daab84">


Zap käynnissä

<img width="651" alt="Screenshot 2023-11-16 at 14 05 02" src="https://github.com/AkiAleksi/h4/assets/112399816/3c56d989-1215-4f49-b9a5-f1848741cc61">


Zap näkyy

Loin CA-sertifikaatin. Zapissa sertifikaatti luodaan menemällä Options -> Server Certificates -> Save. Sitten paikan valinta.
Sitten laitoin hakukenttään localhost:8080. Zapin sivut aukesi. Latasin sertifikaatin zapin sivuilta.






<img width="659" alt="Screenshot 2023-11-17 at 20 18 27" src="https://github.com/AkiAleksi/h4/assets/112399816/3df089aa-412b-487e-bc7f-1e8e6f454728">


importtasin sertifikaatin.



<img width="645" alt="Screenshot 2023-11-17 at 20 20 40" src="https://github.com/AkiAleksi/h4/assets/112399816/49d96942-2597-4162-a6fe-db40f6d3b41e">


Latasin Foxyproxyn, jo tässä kohtaa kun ei toiminut localhostissa ilman sitä.


<img width="516" alt="Screenshot 2023-11-17 at 20 27 22" src="https://github.com/AkiAleksi/h4/assets/112399816/3a70d03b-31e7-4891-a4ef-6677ac83d17f">

Käynnistin sen


<img width="659" alt="Screenshot 2023-11-17 at 20 29 00" src="https://github.com/AkiAleksi/h4/assets/112399816/bc89e4f3-1386-4158-85b0-95dbc0266a5f">

Menin web security academyyn. Hakupyyntö ilmestyi Zapin käyttöliittymään.


<img width="766" alt="Screenshot 2023-11-18 at 15 26 11" src="https://github.com/AkiAleksi/h4/assets/112399816/363a5d62-c78c-40b2-9cd8-33bd695c2dd0">





b.)

Latasin Foxyproxyn. Menin add extensions. Hain Foxyproxya. Sen jälkeen lisäsin sen.



<img width="516" alt="Screenshot 2023-11-17 at 20 27 22" src="https://github.com/AkiAleksi/h4/assets/112399816/3a70d03b-31e7-4891-a4ef-6677ac83d17f">

Lisäsin foxyproxy profiilit.





<img width="944" alt="Screenshot 2023-11-17 at 21 37 24" src="https://github.com/AkiAleksi/h4/assets/112399816/ffb5f90b-ee19-4b29-ac62-520a89774137">





Käynnistin profiilin.


<img width="659" alt="Screenshot 2023-11-17 at 20 29 00" src="https://github.com/AkiAleksi/h4/assets/112399816/bc89e4f3-1386-4158-85b0-95dbc0266a5f">

Asetin proxyn


<img width="929" alt="Screenshot 2023-11-17 at 20 59 15" src="https://github.com/AkiAleksi/h4/assets/112399816/b369bb16-bff1-48a2-a776-eb7be3d2ed9f">

FoxyProxy toimii



<img width="382" alt="Screenshot 2023-11-18 at 12 05 06" src="https://github.com/AkiAleksi/h4/assets/112399816/fbc32ca9-f616-4e5a-ac64-de4f5a122c2d">




17.11.2023 klo 21:38

c.)

Menin live chattiin ja chattasin. Sen jälkeen view transcript. 
Huomasin, että numeroitu txt file 2.txt

<img width="646" alt="chat" src="https://github.com/AkiAleksi/h4/assets/112399816/36b7d754-b407-47a3-9c05-bc945b1c4feb">

Katsoin kaappauksen zapista. Muokkasin pyyntöä.
Ensin laitoin 0.txt. En saanut mitään.
Sen jälkeen kokeilin 1.txt sain salasanan


<img width="908" alt="intercept" src="https://github.com/AkiAleksi/h4/assets/112399816/7e812faf-decd-48e2-b1f0-0ee7cbfc4f4f">

Kokeilin kirjautua tunnuksella ja salasanalla. Pääsin kirjautumaan sisään. 
Salasana oli oikein. 

<img width="678" alt="solved" src="https://github.com/AkiAleksi/h4/assets/112399816/15a93f0b-be10-4b6a-b2c6-2c838292240c">

Lab solved!!!

d.)

Laitoin kuvat mukaan History-osaan: Tools > Options > Display > Process images in HTTP requests/responses
Kaappasin zapilla pyynnön, jolla haetaan kuva.


<img width="522" alt="Screenshot 2023-11-18 at 22 20 34" src="https://github.com/AkiAleksi/h4/assets/112399816/d0b097b6-80c6-4575-a936-9d2937e309fb">



Pyynnön kohta filename on hyökättävissä tämän hyökkäyksen avulla.
Muutin siihen ../../../../etc/passwd



<img width="436" alt="Screenshot 2023-11-18 at 22 21 09" src="https://github.com/AkiAleksi/h4/assets/112399816/ba451d3b-7059-4a5c-8f2d-fa472b9f988a">



Path traversal hyökkäys onnistui!



<img width="461" alt="Screenshot 2023-11-18 at 22 21 33" src="https://github.com/AkiAleksi/h4/assets/112399816/efebeac8-94f8-433a-98dd-11378d38ff66">




Lab ratkaistu

<img width="618" alt="Screenshot 2023-11-18 at 14 04 13" src="https://github.com/AkiAleksi/h4/assets/112399816/260d825b-89f8-49e6-9a44-70fc5133ec53">






e.)



Kaappasin taas pyynnön ja muokkasin sitä.
GET https://0a4f00a803cca70c836b50ec00ac0006.web-security-academy.net/image?filename=/etc/passwd

<img width="440" alt="Screenshot 2023-11-18 at 22 28 05" src="https://github.com/AkiAleksi/h4/assets/112399816/00b70ec4-7837-41fc-ac7d-a1709a0ef823">


Hyökkäys onnistui


<img width="232" alt="Screenshot 2023-11-18 at 22 30 13" src="https://github.com/AkiAleksi/h4/assets/112399816/f8a10e25-2c87-4951-806e-8756ddaa4a70">


Lab ratkaistu!


<img width="639" alt="Screenshot 2023-11-18 at 14 12 33" src="https://github.com/AkiAleksi/h4/assets/112399816/943f765c-7d87-44ab-8102-0bede4e3bf6e">


f.)



Kaappasin pyynnön. 

<img width="466" alt="Screenshot 2023-11-18 at 22 33 37" src="https://github.com/AkiAleksi/h4/assets/112399816/d1bdc96d-62ec-49d3-b7ce-36c6bd498f78">





Muokkasin pyyntöä ....//....//....//etc/passwd


<img width="242" alt="Screenshot 2023-11-18 at 22 34 01" src="https://github.com/AkiAleksi/h4/assets/112399816/92c97fa4-ad22-4ff7-a799-80a7645d3895">




Hyökkäys onnistui!



<img width="456" alt="Screenshot 2023-11-18 at 22 34 15" src="https://github.com/AkiAleksi/h4/assets/112399816/a4b37ac1-4eb3-4010-9992-436684385752">




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


Search box syöttää siihen kirjoitetun koodin.
Testataan <h1>xd</h1>


<img width="444" alt="Screenshot 2023-11-18 at 16 41 29" src="https://github.com/AkiAleksi/h4/assets/112399816/41d80b11-814f-4013-9117-3907d64e65c9">





Syötetään <script>alert()</script>






<img width="366" alt="Screenshot 2023-11-18 at 16 45 07" src="https://github.com/AkiAleksi/h4/assets/112399816/fc489d79-d77f-4b98-beb4-1ebee4ca0632">







alert box tulee esiin.






<img width="424" alt="Screenshot 2023-11-18 at 16 44 21" src="https://github.com/AkiAleksi/h4/assets/112399816/63c26178-1b14-402a-a629-92017ada87fd">





Lab ratkaistu






<img width="440" alt="Screenshot 2023-11-18 at 16 44 35" src="https://github.com/AkiAleksi/h4/assets/112399816/b33b3bff-96db-4baa-97a8-dbc5f21c79ae">

j.)

Syötin kommentin ja kaappasin sen zapilla.


<img width="436" alt="Screenshot 2023-11-18 at 17 29 08" src="https://github.com/AkiAleksi/h4/assets/112399816/b0c558ea-687e-46f0-9293-116071ec38af">


Muutin sitä


<img width="168" alt="Screenshot 2023-11-18 at 17 33 12" src="https://github.com/AkiAleksi/h4/assets/112399816/4fac5812-f13e-49bd-b69d-d1d76a220a22">



Lab ratkaistu!


<img width="157" alt="Screenshot 2023-11-18 at 17 34 48" src="https://github.com/AkiAleksi/h4/assets/112399816/d9bd8517-5808-4047-8433-64a33a462582">


k.)

https://owasp.org/www-project-webgoat/


<img width="864" alt="Screenshot 2023-11-18 at 17 48 07" src="https://github.com/AkiAleksi/h4/assets/112399816/0a76c286-32fe-4e2b-828f-8fb7a336b8a5">


<img width="457" alt="Screenshot 2023-11-18 at 17 47 00" src="https://github.com/AkiAleksi/h4/assets/112399816/f80013fa-6172-4b4c-9a4c-2fbe4f1d3794">

m.)



Hijack a session (1)

Tässä näkyy cookie.
En kyllä oikein keksinyt mitä sille pitäisi tehdä.


<img width="432" alt="Screenshot 2023-11-18 at 19 37 34" src="https://github.com/AkiAleksi/h4/assets/112399816/a15882b2-cbb4-4c8a-9898-ee67062607a0">



Insecure Direct Object References (4)
Missing Function Level Access Control (3)
Spoofing an Authentication Cookie (1)

n) (A7) Identity & Auth Failure (WebGoat 2023.4)
Authentication Bypasses (1)
Insecure Login (1)

o) (A10) Server-side Request Forgery (WebGoat 2023.4)
Server-Side Request Forgery (2)

p) Client side (WebGoat 2023.4)
Bypass front-end restrictions (2)
