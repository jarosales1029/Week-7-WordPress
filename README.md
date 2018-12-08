## Week-7-WordPress
Week 7 - WordPress Pentesting

Time Spent: 11 Hours

>Objective: Find, analyze, recreate, and document **five vulerabilities** affecting an old version of WordPress

## Pentesting Report

1. XML-RPC API Multi-Call 
  - [ ] Summary: 
    - Vulnerability types:
    - Tested in version: WordPress 4.2
    - Fixed in version: 4.7.5
  - [ ] GIF Walkthrough: https://github.com/jarosales1029/Week-7-WordPress/blob/master/Week%207%20-%20XML-RPC.gif
  - [ ] Steps to recreate: Open terminal and type in the command: 'wpscan --url http://wpdistilery.vm --enumerate u' to find users.  Then type in the command 'wpscan --url http://wpdistillery.vm --passwords /usr/share/wordlists/rockyou.txt --usernames admin' where after --passwords you will list your path to your wordlist and where after --usernames you will list the names you find after enumarting for them.
  - [ ] Affected source code:
    - https://null-byte.wonderhowto.com/how-to/gain-control-wordpress-by-exploiting-xml-rpc-0174864/
1. (Required) Vulnerability Name or ID
  - [ ] Summary: 
    - Vulnerability types:
    - Tested in version:
    - Fixed in version: 
  - [ ] GIF Walkthrough: 
  - [ ] Steps to recreate: 
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)
1. (Required) Vulnerability Name or ID
  - [ ] Summary: 
    - Vulnerability types:
    - Tested in version:
    - Fixed in version: 
  - [ ] GIF Walkthrough: 
  - [ ] Steps to recreate: 
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)
1. (Optional) Vulnerability Name or ID
  - [ ] Summary: 
    - Vulnerability types:
    - Tested in version:
    - Fixed in version: 
  - [ ] GIF Walkthrough: 
  - [ ] Steps to recreate: 
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)
1. (Optional) Vulnerability Name or ID
  - [ ] Summary: 
    - Vulnerability types:
    - Tested in version:
    - Fixed in version: 
  - [ ] GIF Walkthrough: 
  - [ ] Steps to recreate: 
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php) 

## Assets

List any additional assets, such as scripts or files

## Resources

- [WordPress Source Browser](https://core.trac.wordpress.org/browser/)
- [WordPress Developer Reference](https://developer.wordpress.org/reference/)
- [https://github.com/1N3/](https://github.com/1N3/Wordpress-XMLRPC-Brute-Force-Exploit)
- [https://github.com/AresS31/](https://github.com/AresS31/xmlrpc-bruteforcer)
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
