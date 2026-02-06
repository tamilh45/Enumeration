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
Following searches for all the sites that is in the domain letterboxd.com
<img width="1919" height="1054" alt="image" src="https://github.com/user-attachments/assets/8be51816-315e-462e-b108-abbbbd841e29" />


filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain letterboxd.com
<img width="1919" height="1052" alt="image" src="https://github.com/user-attachments/assets/187fc254-68e1-46d1-80b9-f35e00032a78" />



intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.
<img width="1919" height="1051" alt="image" src="https://github.com/user-attachments/assets/2f761f9a-0470-4230-869b-3b517a4aa406" />



inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.
<img width="1919" height="1052" alt="image" src="https://github.com/user-attachments/assets/c0d7a726-7b72-40fa-a70b-a40e1d6dbd39" />

intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.
<img width="1919" height="1040" alt="Screenshot 2026-02-06 231154" src="https://github.com/user-attachments/assets/d74f9771-1e11-4b3f-b8be-e7e1dad3068d" />

link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.
<img width="1919" height="1014" alt="image" src="https://github.com/user-attachments/assets/aae05378-b9d0-4ce1-9d94-fc92c660b3ad" />

cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.
<img width="1919" height="1050" alt="image" src="https://github.com/user-attachments/assets/8bc302f4-24b4-42a6-96d8-7c42b1031e12" />

 
## DNS Enumeration


## DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:
<img width="1918" height="892" alt="Screenshot 2026-02-06 225031" src="https://github.com/user-attachments/assets/9d22e404-94ff-4166-82c2-2940f319ae4b" />







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
<img width="1050" height="906" alt="Screenshot 2026-02-06 225109" src="https://github.com/user-attachments/assets/9b2cf00a-3d37-4f23-a9aa-a514a5fd614f" />


## smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.
<img width="727" height="357" alt="Screenshot 2026-02-06 225204" src="https://github.com/user-attachments/assets/0da489af-4fc9-4982-bcf2-8bcbf3477921" />


In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:
<img width="653" height="289" alt="image" src="https://github.com/user-attachments/assets/703ae40f-421a-4c2d-8608-6529dd7c3a96" />

select any username in the first column of the above file and check the same
<img width="792" height="358" alt="image" src="https://github.com/user-attachments/assets/b3da718b-5515-4a23-84e6-78fd6208f15f" />


## Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands  

## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.


## OUTPUT:
<img width="623" height="195" alt="545538568-476029aa-c5c4-4de9-a0c2-f29ce598637a (1)" src="https://github.com/user-attachments/assets/e73cf6b6-ff1f-492d-b760-232dd9ee0da1" />


## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

