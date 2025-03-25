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

![WhatsApp Image 2025-03-15 at 13 21 25_8d234d67](https://github.com/user-attachments/assets/fb753012-3893-4518-84f7-ac9b03d02b76)


filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com

![WhatsApp Image 2025-03-15 at 13 23 04_216ee4d2](https://github.com/user-attachments/assets/e94efa37-f8bd-45bb-b6fb-8be2651def94)



intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.

![WhatsApp Image 2025-03-15 at 13 25 45_2173d021](https://github.com/user-attachments/assets/1a7e0e9d-34ae-4209-9988-d181d7db7928)

inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.

![WhatsApp Image 2025-03-25 at 10 59 03_58737e15](https://github.com/user-attachments/assets/b4056ccb-5f55-4435-b6dc-bb4ae6d36ac0)

intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.

![WhatsApp Image 2025-03-15 at 13 29 40_fa7e63b7](https://github.com/user-attachments/assets/85d43d48-a305-48be-8b58-f54e1cddfa01)

link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.

![WhatsApp Image 2025-03-25 at 11 00 55_fec08cc0](https://github.com/user-attachments/assets/bb2f2160-0bf3-41e5-95ee-b589bd7bf56c)

cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.

![WhatsApp Image 2025-03-25 at 11 01 55_29b7b94b](https://github.com/user-attachments/assets/ca8e1f92-0e43-426c-9b49-22f884e6dc1e)

 
#DNS Enumeration


##DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:

![WhatsApp Image 2025-03-25 at 11 03 16_52d35edf](https://github.com/user-attachments/assets/25b60eca-85de-4cfe-b5f9-a1beea8ff4a1)

![WhatsApp Image 2025-03-25 at 11 05 22_271d4982](https://github.com/user-attachments/assets/ff1663b2-bdfd-4518-b124-3619a8d4601b)





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

![WhatsApp Image 2025-03-25 at 11 06 21_a9b3fb9a](https://github.com/user-attachments/assets/bee857ae-6348-4e84-95c6-9cb5148e7dd8)

##smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.

![WhatsApp Image 2025-03-25 at 11 07 17_a2476b13](https://github.com/user-attachments/assets/bcf99851-993b-42c4-a15b-44f24f793dc0)

In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

select any username in the first column of the above file and check the same

![WhatsApp Image 2025-03-25 at 11 08 08_7a308b2e](https://github.com/user-attachments/assets/337a38f7-477b-4b72-865b-9d853fed636a)

#Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
 ##Output
  
  ![WhatsApp Image 2025-03-22 at 13 15 23_90f79aca](https://github.com/user-attachments/assets/de098176-f186-4dce-b00f-eb1f858def24)


## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.


## OUTPUT:

![WhatsApp Image 2025-03-22 at 13 15 23_90f79aca](https://github.com/user-attachments/assets/3576910a-18d1-4da8-af2a-2172753a4c33)

## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

