Authenticated Stored Cross-Site Scripting (XSS)

Cross-Site Scripting (XSS) allows a remote attacker to deface a random post on the site and store malicious Javascript code in it. This code would be executed when a visitors view the post and when anyone edits the post from the WordPress dashboard. As a result, an administrator tries to fix the defaced post, the would unknowingly trigger the malicious script, which could then be used to put a backdoor on the site and create new admin users.

Steps:

1)Write in the comment box the following inject XSS:

<INPUT TYPE="BUTTON" ONCLICK="alert('XSS')"/>

2)Then after click in the button you will see the alert 

Tested in version: WordPress 4.0-4.7.2

Fixed in version: 4.2.13

CVE-2017-6817

References:

https://wpscan.com/vulnerability/3ee54fc3-f4b4-4c35-8285-9d6719acecf0

https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2017-6817

https://wordpress.org/news/2017/03/wordpress-4-7-3-security-and-maintenance-release/

https://github.com/WordPress/WordPress/commit/419c8d97ce8df7d5004ee0b566bc5e095f0a6ca8

https://blog.sucuri.net/2017/03/stored-xss-in-wordpress-core.html

GIF Walkthrough:

![XSS3](https://user-images.githubusercontent.com/78192383/162075094-52b1b07f-4596-4bdb-becf-24e13e7dcc67.gif)


