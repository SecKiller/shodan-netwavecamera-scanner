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

Installation

$ cd /opt/
$ git clone https://github.com/fbctf/shodanwave.git
$ cd shodanwave
$ pip install -r requirements.txt
Usage


Usage: python shodanwave.py -u usernames.txt -w passwords.txt  -k Shodan API key
       python shodanwave.py --help
       
       
   _____/ /_  ____  ____/ /___ _____
  / ___/ __ \/ __ \/ __  / __ `/ __ \
 (__  ) / / / /_/ / /_/ / /_/ / / / /
/____/_/ /_/\____/\__,_/\__,_/_/ /_/

               __
   ____  ___  / /__      ______ __   _____
  / __ \/ _ \/ __/ | /| / / __ `/ | / / _ \
 / / / /  __/ /_ | |/ |/ / /_/ /| |/ /  __/
/_/ /_/\___/\__/ |__/|__/\__,_/ |___/\___/

                                             ____
   ______________ _____  ____  ___  _____   / __ )__  __
  / ___/ ___/ __ `/ __ \/ __ \/ _ \/ ___/  / __  / / / /
 (__  ) /__/ /_/ / / / / / / /  __/ /     / /_/ / /_/ /
/____/\___/\__,_/_/ /_/_/ /_/\___/_/     /_____/\__, /
                                               /____/
   _____           __ __ _ ____
  / ___/___  _____/ //_/(_) / /__  _____
  \__ \/ _ \/ ___/ ,<  / / / / _ \/ ___/
 ___/ /  __/ /__/ /| |/ / / /  __/ /
/____/\___/\___/_/ |_/_/_/_/\___/_/


This tool is successfully connected to shodan service
Information the use of this tool is illegal, not bad.

usage: shodanwave.py [-h] [-s SEARCH] [-u USERNAME] [-w PASSWORD] [-k ADDRESS]
                     [-t OUTPUT] [-l LIMIT] [-o OFFSET]

optional arguments:
  -h, --help            show this help message and exit
  -s SEARCH, --search SEARCH
                        Default Netwave IP Camera
  -u USERNAME, --username USERNAME
                        Select your usernames wordlist
  -w PASSWORD, --wordlist PASSWORD
                        Select your passwords wordlist
  -k ADDRESS, --shodan ADDRESS
                        Shodan API key
  -t OUTPUT, --output OUTPUT
                        Log File
  -l LIMIT, --limit LIMIT
                        Limit the number of registers responsed by Shodan
  -o OFFSET, --offset OFFSET
                        Shodan skips this number of registers from response


Attention

Use this tool wisely and not for evil. To get the best performece of this tool you need to pay for shodan to get full API access Options --limit and --offset may need a paying API key and consume query credits from your Shodan account.

References:

Shodan API search engine for Internet-connected devices.
Requests Requests: HTTP for Humans
Netwave Exploit Netwave IP Camera - Password Disclosure
