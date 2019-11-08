# Dockerfile

![alt tag](https://github.com/1N3/BlackWidow/blob/master/blackwidowlogo.png)

## ABOUT:
BlackWidow is a python based web application spider to gather subdomains, URL's, dynamic parameters, email addresses and phone numbers from a target website. This project also includes Inject-X fuzzer to scan dynamic URL's for common OWASP vulnerabilities.

## DEMO VIDEO:
[![BlackWidow Demo](https://i.ytimg.com/vi/mch8ht47taY/hqdefault.jpg)](https://www.youtube.com/watch?v=mch8ht47taY)

## FEATURES:
- [x] Automatically collect all URL's from a target website
- [x] Automatically collect all dynamic URL's and parameters from a target website
- [x] Automatically collect all subdomains from a target website
- [x] Automatically collect all phone numbers from a target website
- [x] Automatically collect all email addresses from a target website
- [x] Automatically collect all form URL's from a target website
- [X] Automatically scan/fuzz for common OWASP TOP vulnerabilities
- [x] Automatically saves all data into sorted text files

## LINUX INSTALL:
```
cp blackwidow /usr/bin/blackwidow 
cp injectx.py /usr/bin/injectx.py
pip install -r requirements.txt
```

## USAGE:
```
blackwidow -u https://target.com - crawl target.com with 3 levels of depth.
blackwidow -d target.com -l 5 -v y - crawl the domain: target.com with 5 levels of depth with verbose logging enabled.
blackwidow -d target.com -l 5 -c 'test=test' - crawl the domain: target.com with 5 levels of depth using the cookie 'test=test'
blackwidow -d target.com -l 5 -s y -v y - crawl the domain: target.com with 5 levels of depth and fuzz all unique parameters for OWASP vulnerabilities with verbose logging on.
injectx.py -u https://test.com/uers.php?user=1&admin=true -v y - Fuzz all GET parameters for common OWASP vulnerabilities with verbose logging enabled.
```

## SAMPLE REPORT:
![alt tag](https://github.com/1N3/BlackWidow/blob/master/blackwidow-report1.png)

## DOCKER:
```bash
git clone https://github.com/1N3/BlackWidow.git
cd BlackWidow
docker build -t blackwidow .
docker run -it blackwidow # Defaults to --help

```

## LICENSE:
This software is released under the GNU General Public License v3.0. See LICENSE.md for details.

## SOCIAL MEDIA:
- [Facebook](Nicoleus Sitorus")
- [YouTube](https://www.youtube.com/channel/UCKtXeDDrNvWdw7dJTPjQcOA "YouTube")
- [Blog](https://xerosecurity.com/wordpress/blog/ "Blog")
- [BugCrowd](https://bugcrowd.com/1N3 "BugCrowd")
- [IG: Nicoleus_sitorus")
