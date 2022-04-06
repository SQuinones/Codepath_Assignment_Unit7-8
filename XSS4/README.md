

Steps:

1)Create a comment on a post using the following malicious inject XSS

<img width="1083" alt="Screen Shot 2022-04-06 at 5 36 52 PM" src="https://user-images.githubusercontent.com/78192383/162075671-60ebf6d5-0882-439a-85a2-0f108bb8f3ea.png">


2) Wait for approval from the admin.

3) If the admin approved malicious file will be download

Tested in version: WordPress <= 4.2.8

Fixed in version: 4.5.1

CVE-2016-4566

References:

https://gist.github.com/cure53/09a81530a44f6b8173f545accc9ed07e

https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-4566

https://wpvulndb.com/vulnerabilities/8489

GIF Walkthrough:

![XSS4](https://user-images.githubusercontent.com/78192383/162075448-9b892590-bccf-46a2-b8c3-3f8260fd5a67.gif)
