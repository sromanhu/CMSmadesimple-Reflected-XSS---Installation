# Cmsmadesimple CMS Stored XSS v2.2.18

## Author: (Sergio)

**Description:** Multiple Cross-Site Scripting (XSS) vulnerabilities in installation of  cmsmadesimple v.2.2.18 allows a local attacker to execute arbitrary web scripts via a crafted payload injected into the Database Name, DataBase User or Database Port.
**Attack Vectors:** A vulnerability in the installation sanitation in the Database name, user name and port allows JavaScript code to be injected.

---

### POC:


During the installation process we enter the XSS payload in any of the 3 fields and when we click on next, we will obtain the XSS pop-up

### XSS Payload:

```"' on focus="alert(1)" autofocus="
```


In the following image you can see the embedded code that executes the payload in the instalaltion process.





</br>

### Additional Information:
http://cszcms.com
https://owasp.org/Top10/es/A03_2021-Injection/
https://owasp.org/www-community/attacks/xss/
