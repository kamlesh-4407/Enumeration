# Enumeration
Enumeration Techniques

# Explore Google hacking and enumeration 

# AIM:

To use Google for gathering information and perform enumeration of targets

## STEPS:

### Step 1:

Install kali linux either in partition or virtual box or in live mode

### Step 2:

Investigate on the various Google hacking keywords and enumeration tools as follows:

### Step 3:
Open terminal and try execute some kali linux commands

## Pen Test Tools Categories:  

Following Categories of pen test tools are identified:
Information Gathering.

Google Hacking:

Google hacking, also known as Google dorking, is a technique that involves using advanced operators to perform targeted searches on Google. These operators can be used to search for specific types of information, such as sensitive data that may have been inadvertently exposed on the web. Here are some advanced operators that can be used for Google hacking:

### site:
This operator allows you to search for pages that are within a specific website or domain. For example, "site:example.com" would search for pages that are on the example.com domain.
Following searches for all the sites that is in the domain yahoo.com

<img width="1898" height="1139" alt="image" src="https://github.com/user-attachments/assets/b565c957-7078-4a58-95aa-ff40f39f3890" />

### filetype: 
This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com

<img width="1862" height="954" alt="image" src="https://github.com/user-attachments/assets/c15ee05a-2f3b-4a2b-9336-6eba2bbe081c" />

### intext: 
This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.

<img width="1903" height="1006" alt="image" src="https://github.com/user-attachments/assets/258582c4-941a-425d-a547-6c56369ec150" />

### inurl: 
This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.

<img width="1919" height="1016" alt="image" src="https://github.com/user-attachments/assets/db92ce3d-4a36-475e-95fc-74370160b09b" />

### intitle:
This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.

<img width="1910" height="1115" alt="image" src="https://github.com/user-attachments/assets/9736f968-2c95-4899-b079-6c2e93ed71ef" />

### link:
This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.

<img width="1918" height="995" alt="image" src="https://github.com/user-attachments/assets/7e7013bc-d7ea-4ea2-9fad-df59414ec555" />
cache: 
This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.

 
# DNS Enumeration

## DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## Output:
<img width="1382" height="777" alt="image" src="https://github.com/user-attachments/assets/916550ba-bb2e-4c20-a457-45e4b99904b6" />

## dnsenum
Dnsenum is a multithreaded perl script to enumerate DNS information of a domain and to discover non-contiguous ip blocks. The main purpose of Dnsenum is to gather as much information as possible about a domain. The program currently performs the following operations:

Get the host’s addresses (A record).
Get the namservers (threaded).
Get the MX record (threaded).
Perform axfr queries on nameservers and get BIND versions(threaded).
Get extra names and subdomains via google scraping (google query = “allinurl: -www site:domain”).
Brute force subdomains from file, can also perform recursion on subdomain that have NS records (all threaded).
Calculate C class domain network ranges and perform whois queries on them (threaded).
Perform reverse lookups on netranges (C class or/and whois netranges) (threaded).
Write to domain_ips.txt file ip-blocks.
This program is useful for pentesters, ethical hackers and forensics experts. It also can be used for security tests.
## Output:
<img width="924" height="907" alt="image" src="https://github.com/user-attachments/assets/5b77880c-7927-4304-8862-e9931e6c76eb" />

<img width="1089" height="923" alt="image" src="https://github.com/user-attachments/assets/6941759c-0563-421c-ae1d-0c268ef1c735" />

## smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.
In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:
select any username in the first column of the above file and check the same
## Output:
<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/43f61f90-6f13-44a9-8687-a185c2c48847" />

# Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
 ## Output:
 
  
## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.
## OUTPUT:

<img width="695" height="249" alt="image" src="https://github.com/user-attachments/assets/3a44a8e2-9cec-4fbc-89b8-80430849bc72" />

## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

