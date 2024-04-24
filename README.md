# Types of DNS Records

- ### A RECORD
  Maps a domain name to an **IPv4 address**
  
    | Domain Name   | TTL  | Value      |
    |---------------|------|------------|
    | example.com   | 3600 | 192.0.2.1  |


- ### AAAA Record (IPv6 Address) 
  Maps a domain name to an **IPv6 address**

    | Domain Name   | TTL  | Value                                       |
    |---------------|------|---------------------------------------------|
    | example.com.  | 3600 | 2001:0db8:85a3:0000:0000:8a2e:0370:7334    |


- ### CNAME Record (Canonical Name)
  Maps an alias (subdomain) to the canonical (main) domain name or to any other domain.

    | Domain Name      | TTL  | Value       |
    |------------------|------|-------------|
    | www.example.com. | 3600 | example.com|
    | www.example.net. | 3600 | otherdomain.com|


- ### MX Record (Mail Exchange)
  Specifies mail servers responsible for accepting email on behalf of the domain

    | Domain Name   | TTL  | Priority | Mail Server          |
    |---------------|------|----------|----------------------|
    | example.com.  | 3600 | 10       | mail.example.com.    |


- ### TXT Record (Text)
  Holds arbitrary text data and is often used for verifying domain ownership or providing information

    | Domain Name   | TTL  | Value                |
    |---------------|------|----------------------|
    | example.com.  | 3600 | "v=spf1 mx a ~all"  |


- ### PTR Record (Pointer)
  Used in reverse DNS lookups to map an IP address to a domain name.

    | Domain Name          | TTL  | Value       |
    |----------------------|------|-------------|
    | 1.2.3.4.in-addr.arpa.| 3600 | example.com.|


- ### NS Record (Name Server) 
  Specifies authoritative name servers for the domain

    | Domain Name   | TTL  | Value             |
    |---------------|------|-------------------|
    | example.com.  | 3600 | ns1.example.com. |

