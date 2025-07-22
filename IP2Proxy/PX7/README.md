# IP2PROXY PX7 - Proxy Detection Database

## IP-ProxyType-Country-Region-City-ISP-Domain-UsageType-ASN Database

[IP2Proxy PX7 Database](https://www.ip2location.com/database/px7-ip-proxytype-country-region-city-isp-domain-usagetype-asn) provides proxy data like proxy type, country, region or state, city, Internet Service Provider (ISP), domain, usage type, and ASN of IP address.

This repository provides a sample version of the IP2Proxy PX7 database in CSV, BIN, and CIDR formats. The sample includes a limited number of data rows and is not updated regularly. It is intended solely for evaluation and testing purposes—not for use in production environments. 

For complete, high-accuracy data with up to daily updates, please subscribe to the commercial IP2Proxy PX7 database.

## Database Fields

| **Name** | **Type** | **Description** |
| --- | --- | --- |
| ip_from | INT(10)  / Decimal(39,0) | First IP address in netblock. |
| ip_to | INT(10)  / Decimal(39,0) | Last IP address in netblock. |
| proxy_type | VARCHAR(3) | Type of proxy. |
| country_code | CHAR(2) | Two-character country code based on ISO 3166. |
| country_name | VARCHAR(64) | Country name based on ISO 3166. |
| region_name | VARCHAR(128) | Region or state name. |
| city_name | VARCHAR(128) | City name. |
| isp | VARCHAR(256) | Internet Service Provider or company's name. |
| domain | VARCHAR(128) | Internet domain name associated with IP address range. |
| usage_type | VARCHAR(11) | Usage type classification of ISP or company:<br> (COM) Commercial<br> (ORG) Organization<br> (GOV) Government<br> (MIL) Military<br> (EDU) University/College/School<br> (LIB) Library<br> (CDN) Content Delivery Network<br> (ISP) Fixed Line ISP<br> (MOB) Mobile ISP<br> (DCH) Data Center/Web Hosting/Transit<br> (SES) Search Engine Spider<br> (RSV) Reserved |
| asn | VARCHAR(6) | Autonomous system number (ASN). |
| as | VARCHAR(256) | Autonomous system (AS) name. |

IP addresses are stored as 32-bit or 128-bit unsigned integers (depending on IPv4 or IPv6) and must be converted to standard IP notation for readability.

## Sample Rows in CSV Format
```csv
"37375232","37375487","VPN","MX","Mexico","Ciudad de Mexico","Mexico City","Profisol Telecom S.R.L.","profisol.ro","DCH","207990","HostRoyale Technologies Pvt Ltd"
"51107360","51108001","DCH","GB","United Kingdom of Great Britain and Northern Ireland","England","London","Amazon Data Services UK","amazon.com","DCH","16509","Amazon.com Inc."
"51749853","51749865","DCH","US","United States of America","Ohio","Columbus","Amazon Technologies Inc.","amazon.com","DCH","16509","Amazon.com Inc."
"55970289","55970424","DCH","US","United States of America","Virginia","Ashburn","Amazon Data Services NoVa","amazon.com","DCH","14618","Amazon.com Inc."
"58417791","58418977","DCH","DE","Germany","Hessen","Frankfurt am Main","A100 ROW GmbH","amazon.com","DCH","16509","Amazon.com Inc."
"59464156","59464156","SES","US","United States of America","Ohio","Columbus","Amazon Technologies Inc.","amazon.com","SES","16509","Amazon.com Inc."
"59881250","59881250","SES","US","United States of America","Ohio","Columbus","Amazon Technologies Inc.","amazon.com","SES","16509","Amazon.com Inc."
"65765890","65766340","DCH","US","United States of America","Virginia","Ashburn","Amazon Data Services NoVa","amazon.com","DCH","14618","Amazon.com Inc."
"68039093","68039094","DCH","US","United States of America","Oklahoma","Tulsa","Level 3 Communications Inc.","level3.com","DCH","3356","Level 3 Parent LLC"
"68816351","68816376","DCH","US","United States of America","Utah","Salt Lake City","Level 3 Communications Inc.","level3.com","DCH","3356","Level 3 Parent LLC"
"71575125","71575125","DCH","BG","Bulgaria","Sofia (stolitsa)","Sofia","Level 3 Communications Ltd","level3.com","DCH","3356","Level 3 Parent LLC"
"80943049","80944479","DCH","FR","France","Ile-de-France","Paris","Microsoft Corporation","microsoft.com","DCH","8075","Microsoft Corporation"
"86206379","86206379","VPN","SK","Slovakia","Bratislavsky kraj","Bratislava","Internet-Hosting Ltd","ihc.ru","DCH","61424","eServer s.r.o."
"88841424","88841424","PUB","DE","Germany","Bayern","Nuremberg","Hetzner Online GmbH","hetzner.de","DCH","24940","Hetzner Online GmbH"
"92652037","92652038","VPN","SE","Sweden","Stockholms lan","Stockholm","Internet Vikings International AB","internetvikings.com","DCH","51747","Internet Vikings International AB"
"94448862","94448895","DCH","US","United States of America","Virginia","Ashburn","Hetzner Online GmbH","hetzner.de","DCH","213230","Hetzner Online GmbH"
```

## Downloadable File Formats

- CSV: Comma-delimited text file with decimal ranges for direct database import or manual inspection.

- BIN: IP2Location binary format for use with official IP2Location or IP2Proxy libraries.

- CIDR: Comma-delimited text file with CIDR ranges, useful for firewall rules, network scanning, log analysis, and infrastructure automation.

## Sample Databases

| Format       | IPv4 Address
| IPv6 Address                                                                                                          |
|--------------|----------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------|
| **CSV**      | [Download Sample](https://github.com/ip2location/sample-databases/tree/main/IP2Proxy/PX7/ip2proxy-px7-sample.ipv4.csv) | [Download Sample](https://github.com/ip2location/sample-databases/tree/main/IP2Proxy/PX7/ip2proxy-px7-sample.ipv6.csv) |
| **BIN**      | [Download Sample](https://github.com/ip2location/sample-databases/tree/main/IP2Proxy/PX7/ip2proxy-px7-sample.ipv4.bin) | [Download Sample](https://github.com/ip2location/sample-databases/tree/main/IP2Proxy/PX7/ip2proxy-px7-sample.ipv6.bin) |
| **CIDR**     | [Download Sample](https://github.com/ip2location/sample-databases/tree/main/IP2Proxy/PX7/ip2proxy-px7-sample.ipv4.cidr.csv) | [Download Sample](https://github.com/ip2location/sample-databases/tree/main/IP2Proxy/PX7/ip2proxy-px7-sample.ipv6.cidr.csv) |



# Usage

### CSV File for Database Query

For details on importing the CSV file into a database and using SQL statements for IP lookup, please visit [](https://xxxxx)<https://www.ip2location.com/documentation/ip2proxy-database-px7#codes>

### BIN File for IP Lookup

To perform IP lookups with the BIN file, you’ll need to use the IP2Proxy SDK. Refer to the [development libraries](https://www.ip2location.com/development-libraries/?tab=ip2proxy) for usage instructions and integration guides.

# License

This sample data is provided by IP2Location.com for evaluation purposes. Please refer to the [licensing page](https://www.ip2location.com/licensing) for production licensing and usage.

# Useful Guides & Resources

For more information, please refer to the IP2Location.com official documentation at <https://www.ip2location.com/documentation/ip2proxy-database-px7>, which provides comprehensive details and usage guidelines.

Alternatively, you may explore the articles at <https://blog.ip2location.com> for additional insights and practical examples.

# Other IP Geolocation Solutions

- [IP2Location.io IP Geolocation API](https://www.ip2location.io)

- [IP2Location IP Geolocation Database](https://www.ip2location.com/database/ip2location)

- [IP2Location LITE IP-ASN Database](https://lite.ip2location.com/database-asn)

- [IP2WHOIS WHOIS Domain Lookup](https://www.ip2whois.com/)

# About IP2Location

IP2Location.com offers extensive databases for IP geolocation. It enables users to precisely identify the geographical location of IP addresses, providing details such as country, region, city, district, latitude, longitude, ZIP code, time zone, connection speed, ISP, domain name, IDD country code, area code, weather station code and name, mobile carrier, elevation, usage type, address type, advertising category, and autonomous system.

These databases are invaluable for various use cases and applications, including website traffic analysis, fraud prevention, and personalized content delivery. By leveraging IP2Location’s data, businesses and developers can enhance their services, improve user experiences, and ensure more secure online interactions. IP2Location solution is available as a database and hosted API. If you are interested in web service instead of database, please visit [IP2Location.io](https://www.ip2location.io) for the remote hosted service.

Stay connected with us on [Facebook](https://www.facebook.com/ip2location), [X](https://x.com/ip2location) and [LinkedIn](https://www.linkedin.com/company/ip2location) for more insights into IP address data and its powerful applications.
