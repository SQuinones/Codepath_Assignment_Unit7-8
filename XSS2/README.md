
Cross-Site Scripting (XSS)

Cross-Site Scripting, or XSS, issues occur when an application uses untrusted data in a web browser without sufficient validation or escaping.

Steps:

1)login as an admin

2)inject the this XSS in the comments box:

<img width="1116" alt="Screen Shot 2022-04-06 at 5 28 45 PM" src="https://user-images.githubusercontent.com/78192383/162074451-8af4103e-4be0-4603-b54b-3ae780e17459.png">


Tested in version: WordPress <= 4.2.3

Fixed in version: 4.2.4

CVE-2015-5734

References:

https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-5734

GIF Walkthrough:

![XSS](https://user-images.githubusercontent.com/78192383/162074566-f3039283-f5b8-4f50-9cb7-030e4dfc9035.gif)
