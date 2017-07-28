# shodan-netwavecamera-scanner


Shodan netwave scanner is a tool for exploring and obtaining information from cameras specifically Netwave IP Camera. The tool uses a search engine called shodan that makes it easy to search for cameras online.

What does the tool to? Look, a list!

 * Search 
 * Brute force
 * SSID and WPAPSK Password Disclosure
 * E-mail, FTP, DNS, MSN Password Disclosure 
 * Exploit
 

### How to use?
To use shodan netwave scanner you need an api key which you can get for free at https://www.shodan.io/, then you need to follow the next steps.

### Installation

```
$ cd /opt/
$ git clone https://github.com/SecKiller/shodan-netwavecamera-scanner.git
$ cd shodan-netwavecamera-scanner
$ pip install -r requirements.txt
```
### Usage
```
Usage: python SecKiller-shodan-netwave-scanner.py -u usernames.txt -w passwords.txt  -k Shodan API key
       python SecKiller-shodan-netwave-scanner.py --help 
	   
         __              __                                   
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

usage: SecKiller-shodan-netwave-scanner.py [-h] [-s SEARCH] [-u USERNAME] [-w PASSWORD] [-k ADDRESS]

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
  -l LIMIT, --limit LIMIT
                        Limit the number of registers responsed by Shodan
  -o OFFSET, --offset OFFSET
                        Shodan skips this number of registers from response
  -t OUTPUT, --output OUTPUT
                        Save the results


```
### Attention
Use this tool wisely and not for evil. To get the best performece of this tool you need to pay for shodan to get full API access
Options --limit and --offset may need a paying API key and consume query credits from your Shodan account.

### References:

 * [Shodan API](https://www.shodan.io/)  search engine for Internet-connected devices.
 * [Requests](http://docs.python-requests.org/en/master/) Requests: HTTP for Humans
 * [Netwave Exploit](https://www.exploit-db.com/exploits/41236/) Netwave IP Camera - Password Disclosure


Greeting to EternalSec Team :)
