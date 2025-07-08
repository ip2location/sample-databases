# IP2PROXY PX9 - Proxy Detection Database

## IP-ProxyType-Country-Region-City-ISP-Domain-UsageType-ASN-LastSeen-Threat Database

[IP2Proxy PX9 Database](https://www.ip2location.com/database/px9-ip-proxytype-country-region-city-isp-domain-usagetype-asn-lastseen) provides proxy data like proxy type, country, region or state, city, Internet Service Provider (ISP), domain, usage type, ASN, last seen and threat of IP address.

This repository provides a sample version of the IP2Proxy PX9 database in CSV, BIN, and CIDR formats. The sample includes a limited number of data rows and is not updated regularly. It is intended solely for evaluation and testing purposes—not for use in production environments. 

For complete, high-accuracy data with up to daily updates, please subscribe to the commercial IP2Proxy PX9 database.

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
| last_seen | INT(10) | Proxy last seen in days. |
| threat | VARCHAR(128) | Security threat reported:<br> (SPAM) Email and forum spammers<br> (SCANNER) Network security scanners<br> (BOTNET) Malware infected devices |

IP addresses are stored as 32-bit or 128-bit unsigned integers (depending on IPv4 or IPv6) and must be converted to standard IP notation for readability.

## Sample Rows in CSV Format
```csv
"50910463","50910467","DCH","GB","United Kingdom of Great Britain and Northern Ireland","England","London","Amazon Data Services UK","amazon.com","DCH","16509","Amazon.com Inc.","1","-"
"55696820","55696916","DCH","US","United States of America","Virginia","Ashburn","Amazon Data Services NoVa","amazon.com","DCH","14618","Amazon.com Inc.","1","-"
"59346830","59346857","DCH","US","United States of America","Ohio","Columbus","Amazon Technologies Inc.","amazon.com","DCH","16509","Amazon.com Inc.","1","-"
"63574166","63574167","DCH","US","United States of America","Washington","Seattle","Amazon Technologies Inc.","amazon.com","DCH","16509","Amazon.com Inc.","1","-"
"68703662","68703668","DCH","US","United States of America","Louisiana","Monroe","Level 3 Communications Inc.","level3.com","DCH","3356","Level 3 Parent LLC","1","-"
"72257474","72257474","VPN","US","United States of America","Maryland","Baltimore","Level 3 Communications Inc.","level3.com","DCH","3356","Level 3 Parent LLC","26","-"
"86844587","86844587","VPN","US","United States of America","Texas","Victoria","Internet Utilities Europe and Asia Limited","cyberassets.ae","DCH","61317","Hivelocity LLC","1","-"
"93725249","93725279","DCH","GB","United Kingdom of Great Britain and Northern Ireland","England","London","London Grid for Learning Trust","lgfl.org.uk","DCH","60187","London Grid for Learning Trust","1","-"
"98833946","98833946","PUB","RU","Russian Federation","Moskva","Moscow","NCN BBCUST","rt.ru","DCH","42610","PJSC Rostelecom","30","-"
"147971648","147971778","DCH","JP","Japan","Tokyo","Tokyo","Alibaba Cloud (Singapore) Private Limited","alicloud.com","DCH","45102","Alibaba (US) Technology Co. Ltd.","1","-"
"215520560","215520567","DCH","US","United States of America","California","Sacramento","U.S. TelePacific Corp.","tpx.com","DCH","7018","AT&T Enterprises LLC","1","-"
"226353837","226353837","PUB","KR","Korea (the Republic of)","Seoul-teukbyeolsi","Seoul","Amazon Technologies Inc.","amazon.com","DCH","16509","Amazon.com Inc.","30","-"
"233512806","233512806","PUB","IN","India","Maharashtra","Mumbai","Amazon Data Services India","amazon.com","DCH","16509","Amazon.com Inc.","30","-"
"267110992","267110992","DCH","SG","Singapore","Singapore","Singapore","OVH Singapore Pte. Ltd","ovh.com","DCH","16276","OVH SAS","1","-"
"309818973","309818973","SES","US","United States of America","Ohio","Columbus","Amazon Technologies Inc.","amazon.com","SES","16509","Amazon.com Inc.","1","-"

```

## Downloadable File Formats

- CSV: Comma-delimited text file with decimal ranges for direct database import or manual inspection.

- BIN: IP2Location binary format for use with official IP2Location or IP2Proxy libraries.

- CIDR: Comma-delimited text file with CIDR ranges, useful for firewall rules, network scanning, log analysis, and infrastructure automation.

## Sample Databases

| Format       | IPv4 Address                                                                                                        | IPv6 Address                                                                                                        |
|--------------|--------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------|
| **CSV**      | [Download Sample](https://github.com/ip2location/sample-databases/tree/main/IP2Proxy/PX9/ip2proxy-px9-sample.ipv4.csv) | [Download Sample](https://github.com/ip2location/sample-databases/tree/main/IP2Proxy/PX9/ip2proxy-px9-sample.ipv6.csv) |
| **BIN**      | [Download Sample](https://github.com/ip2location/sample-databases/tree/main/IP2Proxy/PX9/ip2proxy-px9-sample.ipv4.bin) | [Download Sample](https://github.com/ip2location/sample-databases/tree/main/IP2Proxy/PX9/ip2proxy-px9-sample.ipv6.bin) |


# Usage

### CSV File for Database Query

For details on importing the CSV file into a database and using SQL statements for IP lookup, please visit [](https://xxxxx)<https://www.ip2location.com/documentation/ip2proxy-database-px9#codes>

### BIN File for IP Lookup

To perform IP lookups with the BIN file, you’ll need to use the IP2Proxy SDK. Refer to the [development libraries](https://www.ip2location.com/development-libraries/?tab=ip2proxy) for usage instructions and integration guides.

# License

This sample data is provided by IP2Location.com for evaluation purposes. Please refer to the [licensing page](https://www.ip2location.com/licensing) for production licensing and usage.

# Useful Guides & Resources

For more information, please refer to the IP2Location.com official documentation at <https://www.ip2location.com/documentation/ip2proxy-database-px9>, which provides comprehensive details and usage guidelines.

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
