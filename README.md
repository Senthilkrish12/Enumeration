# Enumeration Techniques
# Explore Google hacking and enumeration 
# Name : Senthil Raj G
# Register No : 212224100054
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

site: This operator allows you to search for pages that are within a specific website or domain. For example, "site:example.com" would search for pages that are on the example.com domain.
Following searches for all the sites that is in the domain yahoo.com

# Output
<img width="1918" height="1198" alt="image" src="https://github.com/user-attachments/assets/e1bcac0a-c458-45d8-b6b4-867ecdb699ab" />

filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com

# Output
<img width="1918" height="1198" alt="image" src="https://github.com/user-attachments/assets/6868e2c4-8332-4df2-aaec-8a42bb0d1964" />

intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.

# Output
<img width="1918" height="1198" alt="image" src="https://github.com/user-attachments/assets/30932525-0b7d-4aba-a62c-457ef6bc89c6" />

inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.

# Output
<img width="1918" height="1198" alt="image" src="https://github.com/user-attachments/assets/99c9fe72-c0b3-4137-9ee8-92e8a741812e" />

intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.

# Output
<img width="1600" height="1198" alt="image" src="https://github.com/user-attachments/assets/0796f1bd-4115-4ce0-83c1-d61052d752d2" />

link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.

# Output
<img width="1677" height="1198" alt="image" src="https://github.com/user-attachments/assets/b9fbcbc2-d7ac-4376-80cb-c9fe79d209fb" />

cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.

# Output 
<img width="1918" height="1198" alt="image" src="https://github.com/user-attachments/assets/af5c300a-2f97-46b0-9b4c-61e8e771a189" />

# DNS Enumeration


## DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion

## OUTPUT:
<img width="1200" height="750" alt="Screenshot From 2026-02-06 08-21-54" src="https://github.com/user-attachments/assets/78b9d71b-a8bc-478c-b682-7017a5f60e4b" />

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
# output
<img width="665" height="706" alt="Screenshot From 2026-02-06 08-28-37" src="https://github.com/user-attachments/assets/36261637-0d59-43b9-b350-e5bcb3287a79" />

## smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.


In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

select any username in the first column of the above file and check the same
# output
<img width="655" height="394" alt="Screenshot From 2026-02-06 08-28-56" src="https://github.com/user-attachments/assets/5b6577f5-bad1-43ee-8b59-3a96ada58a9c" />


# Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
## Output
<img width="495" height="86" alt="Screenshot From 2026-02-06 08-29-15" src="https://github.com/user-attachments/assets/197187d5-013f-4662-a6b6-fe3c950a6227" />

## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.
## OUTPUT:
<img width="533" height="203" alt="Screenshot From 2026-02-06 08-29-25" src="https://github.com/user-attachments/assets/6faea68c-defb-491b-9b29-ecbc662ed3e1" />

## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

