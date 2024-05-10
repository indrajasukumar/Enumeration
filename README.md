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

site: This operator allows you to search for pages that are within a specific website or domain. For example, "site:example.com" would search for pages that are on the example.com domain.
Following searches for all the sites that is in the domain yahoo.com

![image](https://github.com/indrajasukumar/Enumeration/assets/145115195/8bb86777-22ee-4219-bfa9-e8794e011dfb)


filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com

![image](https://github.com/indrajasukumar/Enumeration/assets/145115195/d84c4273-2bd2-4375-b4d4-71afbf3b3e16)



intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.

![image](https://github.com/indrajasukumar/Enumeration/assets/145115195/b1b3525e-1d59-4520-bf0e-1cf62fec7276)


inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.

![image](https://github.com/indrajasukumar/Enumeration/assets/145115195/b42d34cc-f67d-4e53-849e-7a46422fe4bf)



intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.

![image](https://github.com/indrajasukumar/Enumeration/assets/145115195/62622124-86d1-4e81-b744-47a2e4aa7bec)


link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.

![image](https://github.com/indrajasukumar/Enumeration/assets/145115195/71f722d2-1d83-427e-8eee-bed982464328)

cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.


![image](https://github.com/indrajasukumar/Enumeration/assets/145115195/3c15fe2e-6e7b-4a37-8943-dcf98ecf03f2)

 
#DNS Enumeration


##DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion

![image](https://github.com/indrajasukumar/Enumeration/assets/145115195/0a16a854-cb01-4f51-8242-f62aea37dd33)









##  dnsenum
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

![image](https://github.com/indrajasukumar/Enumeration/assets/145115195/5a94aeda-9387-4f5e-ae40-110ffc1c655b)



## smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.

![image](https://github.com/indrajasukumar/Enumeration/assets/145115195/a1025529-f3b7-4e94-9d4b-16c6a84a0aba)



In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

select any username in the first column of the above file and check the same


![image](https://github.com/indrajasukumar/Enumeration/assets/145115195/fffa4262-6bdc-425b-a6ca-1b219aeb644c)


# Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
 ## Output
 
 ![image](https://github.com/indrajasukumar/Enumeration/assets/145115195/ca91ffb0-fc40-4ea8-8097-5a8a99362e5e)

  
  

## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.


## OUTPUT:

![image](https://github.com/indrajasukumar/Enumeration/assets/145115195/9e55003b-a7ae-44f4-a341-4615e4feb1b9)



## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

