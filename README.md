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

### OUTPUT:
![267852983-a588360a-5d51-4d26-8322-2f6ebe032e87](https://github.com/Sudharsanram/Enumeration/assets/119393980/b45d11d4-e464-4102-a807-3bed5ef64bce)


filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com

### OUTPUT:

![267853046-f3e518cd-6e9e-4a68-8d7c-8814a8755cfb](https://github.com/Sudharsanram/Enumeration/assets/119393980/fd91be7f-f94d-434a-8a49-01b0d46d55ca)


intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.

### OUTPUT:

![267853099-dc9f230f-dda7-4b8f-a781-9fd26086ec1f](https://github.com/Sudharsanram/Enumeration/assets/119393980/14a42e7b-a0dc-42af-88de-400e268dca45)

inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.

### OUTPUT:

![267853406-97ced70a-7a07-4633-a8c1-d2f6b675c4a6](https://github.com/Sudharsanram/Enumeration/assets/119393980/bc37795f-0975-4b29-a1dd-f4302b116474)


intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.

### OUTPUT:

![267853437-277b9853-d670-482f-919a-7e3742e044ca](https://github.com/Sudharsanram/Enumeration/assets/119393980/05161b04-30ec-4f75-a6ac-2ebc2e1068ef)


link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.

### OUTPUT:
![267853772-2ca05ba5-465e-4d79-bf68-8bd726ea6482](https://github.com/Sudharsanram/Enumeration/assets/119393980/3b95cf5a-b918-4946-937a-3c760d857beb)



cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.

### OUTPUT:
 
 ![267853818-1e930c95-fe58-473b-a483-71d5d7527307](https://github.com/Sudharsanram/Enumeration/assets/119393980/2e49f8f8-88ca-43bc-a4b6-39a17d5d1a57)

#DNS Enumeration


##DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:

![267853921-bff6b1fa-db5a-4634-9e87-09d9ebd0da4f](https://github.com/Sudharsanram/Enumeration/assets/119393980/5640f904-3892-4d53-a667-3ba376b5f9d1)
![267853929-340db1a8-7257-4426-9b9e-6cdb8d653240](https://github.com/Sudharsanram/Enumeration/assets/119393980/545f433d-ffc2-4de6-9569-459b3069d1cf)

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

### OUTPUT:
![267854029-68bd4daa-782d-43ff-bf7d-ab03a8a0ab7b](https://github.com/Sudharsanram/Enumeration/assets/119393980/8307245a-86ac-4f80-bc3d-bec43eadefd4)


##smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.

![267854080-d8162783-ec5d-4ad9-b1c9-14e3e26dce67](https://github.com/Sudharsanram/Enumeration/assets/119393980/52a47529-c60d-40e1-a97e-02acc5d16cd1)


In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

select any username in the first column of the above file and check the same

![267854120-b7b2b3d4-681d-457e-987f-fa9982d42525](https://github.com/Sudharsanram/Enumeration/assets/119393980/59e027ae-e7d3-49bc-9066-012bd4f76af9)


#Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
 ##Output
  
  ![267854200-ff539a92-be6e-40a3-8c46-d9b223a62e21](https://github.com/Sudharsanram/Enumeration/assets/119393980/d33f7aaa-b486-43f3-8e62-064d046dda40)

  

## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.


## OUTPUT:

![267854311-16652a98-4067-4b41-ae7f-2606f57b747a](https://github.com/Sudharsanram/Enumeration/assets/119393980/27fd7be4-b1c1-4ebf-bdcb-ee0f36d3e893)


## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

