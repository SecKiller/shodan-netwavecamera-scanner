# shodan-netwavecamera-scanner


is a tool for exploring and obtaining information from cameras specifically Netwave IP Camera. The tool uses a search engine called shodan that makes it easy to search for cameras online.

What does the tool to? Look, a list!

Search

Brute force

SSID and WPAPSK Password Disclosure

E-mail, FTP, DNS, MSN Password Disclosure

Exploit

This is an example of shodan wave running, the password was not found through raw force so the tool tries to leak the camera's memory. If the tool finds the password it does not try to leak the memory


How to use?


To use shodanwave you need an api key which you can get for free at https://www.shodan.io/, then you need to follow the next steps.


Installation :


$ cd /opt/

$ git clone https://github.com/fbctf/shodanwave.git

$ cd shodanwave

$ pip install -r requirements.txt

Usage


Usage: python shodanwave.py -u usernames.txt -w passwords.txt  -k Shodan API key
       python shodanwave.py --help
       
       
 


Attention

Use this tool wisely and not for evil. To get the best performece of this tool you need to pay for shodan to get full API access Options --limit and --offset may need a paying API key and consume query credits from your Shodan account.

References:

Shodan API search engine for Internet-connected devices.
Requests Requests: HTTP for Humans
Netwave Exploit Netwave IP Camera - Password Disclosure
