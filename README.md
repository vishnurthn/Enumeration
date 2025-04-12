# Enumeration
Enumeration Techniques

DEVELOPED BY : VISHNU RATHAN B

REG NO: 212224240185


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


Google hacking, also known as Google dorking, is a technique that involves using advanced operators to perform targeted searches on Google. These operators can be used to search for specific types of information, such as sensitive data 

that may have been inadvertently exposed on the web. Here are some advanced operators that can be used for Google hacking:


site: This operator allows you to search for pages that are within a specific website or domain. For example, "site:example.com" would search for pages that are on the example.com domain.

Following searches for all the sites that is in the domain yahoo.com


## Output:

![image](https://github.com/user-attachments/assets/6e730489-a824-4f9c-b2c6-e23a6ba9d6b2)


filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com


## Output:


![image](https://github.com/user-attachments/assets/e8aa8601-61c4-426f-95a5-61106be5a690)



intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.

## Output:


![image](https://github.com/user-attachments/assets/84096e5a-2b36-4226-b1d7-8a1bad6822e1)



inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.


## Output:


![image](https://github.com/user-attachments/assets/8d25b7ec-2165-4619-b9b0-5d43235fedd1)



intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.

## Output:

![image](https://github.com/user-attachments/assets/e459afb4-5bc4-4840-b312-d69ca33f4530)



link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.

## Output:

![image](https://github.com/user-attachments/assets/4a8997eb-cbb8-444f-add1-8bfa0d9c3860)

cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.


## Output:


![{13F22C65-C6FD-4F57-926E-B5E65CD56D95}](https://github.com/user-attachments/assets/cf439421-23d4-4469-b9d0-457973f62425)

 
#DNS Enumeration


##DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:


![{B44F96C2-7B55-41B5-8F43-A7CC2D0D1934}](https://github.com/user-attachments/assets/3c5cd779-c8b5-4d67-b291-6a31b3d9e515)


![{255A7CB2-8100-42A8-957B-A1236F2D8406}](https://github.com/user-attachments/assets/b80c1a35-461b-41a5-a49c-6c6ef2afe27b)






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


## Output:

![{94477A2C-AAD0-4A0B-97F5-02DCC39A0812}](https://github.com/user-attachments/assets/ce7f1e2e-f990-4802-9686-27e272f6c998)


##smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.

## Output:

![{D6897F94-EFE5-4167-AAD2-7A495EE3521D}](https://github.com/user-attachments/assets/aff9c65d-6236-467f-a6e9-3b6b9f49a944)



In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

select any username in the first column of the above file and check the same


#Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
 ##Output

  
 ![image](https://github.com/user-attachments/assets/b0724548-6257-4a56-b9da-a10f8b2523f6)
 

## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.


## OUTPUT:


![{FAE6FF65-ADB3-4C5D-B99C-AD33EA797001}](https://github.com/user-attachments/assets/92bb27f3-a30d-4f39-ae71-aab3ded96bfe)



## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

