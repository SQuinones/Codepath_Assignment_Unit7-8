Cross-Site Scripting (XSS)

Summary: Cross-Site Scripting (XSS) attacks are a type of injection, in which malicious scripts are injected. If untrusted data contains a client side script, the browser will execute the script while it is interpreting the page. An unauthenticated attacker can inject JavaScript in WordPress comments. The script is triggered when the comment is viewed.

If the comment text is long enough, it will be truncated when inserted in the database. The MySQL TEXT type size limit is 64 kilobytes, so we need to make the a long comment

STEPS:

    Create a comment on a post
    The admnin needs to approve the commnet. So we need to make a nice trust comment
    After the approval we insert the injection XSS in the comments

XSS to insert:

<img width="1089" alt="Screen Shot 2022-04-06 at 5 26 05 PM" src="https://user-images.githubusercontent.com/78192383/162073988-b9bdf953-19a6-4d4a-a73b-b2f061b0dcfd.png">


Screen Shot 2022-04-06 at 3 43 49 PM

Tested in version: WordPress <= 4.2

Fixed in version: 4.2.1

CVE-2015-3440

References:

https://wpscan.com/vulnerability/8051e64b-f73e-45ce-a853-02b8e425155b

https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-3440

https://www.exploit-db.com/exploits/36844/

https://klikki.fi/adv/wordpress2.html

https://packetstormsecurity.com/files/131644/

GIF Walkthrough:

![XSS1](https://user-images.githubusercontent.com/78192383/162074033-32dc3aa6-7e3f-4d21-9374-1b2430dd714d.gif)



