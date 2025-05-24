# Enumeration
Enumeration Techniques
## Name: Shanmuga Raj.K
## Reg no: 212223040192
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
![1](https://github.com/user-attachments/assets/1a372bf9-3703-4405-a714-e140bda29926)
filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com
![2](https://github.com/user-attachments/assets/41a096ce-8faa-4774-8e8d-bb51594d6333)
intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.
![3](https://github.com/user-attachments/assets/de5ad93c-598c-4548-8333-9f34870356b2)
inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.
![4](https://github.com/user-attachments/assets/b78c7487-4f73-46dd-bb3a-51bb0fd8f096)
intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.
![5](https://github.com/user-attachments/assets/f23d91ab-17da-4101-b339-364aae492a58)
link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.
![6](https://github.com/user-attachments/assets/46238374-7b18-42d7-beee-268cc159c2b7)
cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.
 ![7](https://github.com/user-attachments/assets/23e45bb7-4bc9-4762-b7b3-859512ba8b6d)
#DNS Enumeration
##DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:
![8](https://github.com/user-attachments/assets/396b78de-239b-4a0c-9400-7a8cfdf90051)
![9](https://github.com/user-attachments/assets/e78e1047-bd85-4541-bd3b-9d92f749f2c4)
##dnsenum
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
![10](https://github.com/user-attachments/assets/4e8dda6a-2e46-4549-94be-b90741120cff)
##smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.
![11](https://github.com/user-attachments/assets/fb50af72-2b85-4ede-9f94-3cc536ac31c5)
In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:
![12](https://github.com/user-attachments/assets/e892cc06-eb5e-4625-b73e-e3e343d1bb9c)
select any username in the first column of the above file and check the same
![13](https://github.com/user-attachments/assets/bd1458c7-18c6-4aeb-8f83-c05f9f2d0520)
#Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
 ##Output
 ![14](https://github.com/user-attachments/assets/7744673f-bf9f-4b88-8933-a9ac21758374)
## nmap –script smtp-enum-users.nse <hostname>
The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.
## OUTPUT:
![15](https://github.com/user-attachments/assets/b6f7a3e7-f614-41e9-b874-e67afd9cf898)
## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

