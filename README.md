# Week 7- WordPress Pentesting

Time Spent: 11 Hours

>Objective: Find, analyze, recreate, and document **five vulerabilities** affecting an old version of WordPress

## Pentesting Report

1. XML-RPC API Multi-Call 
  - [ ] Summary: Used WPScan to find users and also to execute an XML-RPC multi-call brute force attack for the passwords of the users found.
    - Vulnerability types: Weak Passwords and a XML-RPC vulnerability where for each HTTP request, there could over 1000+ attempts. 
    - Tested in version: WordPress 4.2
    - Fixed in version: 4.7.5
  - [ ] GIF Walkthrough: https://github.com/jarosales1029/Week-7-WordPress/blob/master/Week%207%20-%20XML-RPC.gif
  - [ ] Steps to recreate: Open terminal and type in the command: 'wpscan --url http://wpdistilery.vm --enumerate u' to find users. Then type in the command 'wpscan --url http://wpdistillery.vm --passwords /usr/share/wordlists/rockyou.txt --usernames admin' where after '--passwords' you will list your path to your wordlist and where after '--usernames' you will list the names you find after enumarting for them.
  - [ ] Affected source code:
    - https://null-byte.wonderhowto.com/how-to/gain-control-wordpress-by-exploiting-xml-rpc-0174864/
2. Large File Upload Error Cross-Site Scripting (XSS)
  - [ ] Summary: Able to XSS an alert with a big enough file to potentially excute a code off of just the file name.  
    - Vulnerability types: XSS
    - Tested in version: 4.2
    - Fixed in version: 4.2.15
  - [ ] GIF Walkthrough: https://github.com/jarosales1029/Week-7-WordPress/blob/master/Week%207%20-%20Large%20File%20Upload%20Error%20XSS.gif
  - [ ] Steps to recreate: Download an image file larger than 20mb and renamed file to Silver Surfing Cosmos<img src=x onerror=alert(1337)>.jpg.  Attempted to drag image file to upload in WordPress and received XSS alert.
  - [ ] Affected source code:
    - [Large File Upload Error Cross-Site Scripting (XSS)](https://hackerone.com/reports/203515).
3. Authenticated Stored Cross-Site Scripting (XSS)
  - [ ] Summary: Can post a comment that has an XSS vulernability to execute JavaScript by simply viewing the comment and having the correct permissions.
    - Vulnerability types: XSS
    - Tested in version: 4.2
    - Fixed in version: 4.2.4
  - [ ] GIF Walkthrough: https://github.com/jarosales1029/Week-7-WordPress/blob/master/Week%207%20-%20Authenticated%20Stored%20XSS.gif
  - [ ] Steps to recreate: Would post a comment with the code found at https://klikki.fi/adv/wordpress2.html. The next user to view the code will have an XSS alert pop up with potential JavaScript code.
  - [ ] Affected source code:
    - [https://klikki.fi/adv/wordpress2.html]

## Assets

List any additional assets, such as scripts or files

## Resources

- [WordPress Source Browser](https://core.trac.wordpress.org/browser/)
- [WordPress Developer Reference](https://developer.wordpress.org/reference/)
- [https://github.com/1N3/](https://github.com/1N3/Wordpress-XMLRPC-Brute-Force-Exploit)
- [+Bilal Rizwan](https://medium.com/@the.bilal.rizwan/wordpress-xmlrpc-php-common-vulnerabilites-how-to-exploit-them-d8d3c8600b32)
-

GIFs created with [LiceCap](http://www.cockos.com/licecap/).

## Notes

Describe any challenges encountered while doing the work

## License

    Copyright [yyyy] [name of copyright owner]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
