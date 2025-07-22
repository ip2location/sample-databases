# IP2PROXY PX8 - Proxy Detection Database

## IP-ProxyType-Country-Region-City-ISP-Domain-UsageType-ASN-LastSeen Database

[IP2Proxy PX8 Database](https://www.ip2location.com/database/px8-ip-proxytype-country-region-city-isp-domain-usagetype-asn-lastseen) provides proxy data like proxy type, country, region or state, city, Internet Service Provider (ISP), domain, usage type, ASN, and last seen of IP address.

This repository provides a sample version of the IP2Proxy PX8 database in CSV, BIN, and CIDR formats. The sample includes a limited number of data rows and is not updated regularly. It is intended solely for evaluation and testing purposes—not for use in production environments. 

For complete, high-accuracy data with up to daily updates, please subscribe to the commercial IP2Proxy PX8 database.

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

IP addresses are stored as 32-bit or 128-bit unsigned integers (depending on IPv4 or IPv6) and must be converted to standard IP notation for readability.

## Sample Rows in CSV Format
```csv
"37309880","37309880","PUB","US","United States of America","California","Los Angeles","ClearDocks LLC","hostroyale.com","DCH","203020","HostRoyale Technologies Pvt Ltd","30"
"50935829","50935829","PUB","GB","United Kingdom of Great Britain and Northern Ireland","England","London","Amazon Data Services UK","amazon.com","DCH","16509","Amazon.com Inc.","30"
"51606993","51607266","DCH","US","United States of America","Ohio","Columbus","Amazon Technologies Inc.","amazon.com","DCH","16509","Amazon.com Inc.","1"
"55735917","55736134","DCH","US","United States of America","Virginia","Ashburn","Amazon Data Services NoVa","amazon.com","DCH","14618","Amazon.com Inc.","1"
"57643341","57643962","DCH","IN","India","Maharashtra","Mumbai","Amazon Data Services India","amazon.com","DCH","16509","Amazon.com Inc.","1"
"59354676","59354676","SES","US","United States of America","Ohio","Columbus","Amazon Technologies Inc.","amazon.com","SES","16509","Amazon.com Inc.","1"
"59835997","59836000","DCH","US","United States of America","Ohio","Columbus","Amazon Technologies Inc.","amazon.com","DCH","16509","Amazon.com Inc.","1"
"64215395","64215395","PUB","US","United States of America","Virginia","Ashburn","Amazon Data Services NoVa","amazon.com","DCH","14618","Amazon.com Inc.","30"
"67372767","67372768","DCH","US","United States of America","Missouri","Kansas City","Level 3 Communications Inc.","level3.com","DCH","3356","Level 3 Parent LLC","1"
"68721713","68721713","DCH","US","United States of America","New York","New York City","Level 3 Communications Inc.","level3.com","DCH","3356","Level 3 Parent LLC","1"
"69946411","69947364","DCH","US","United States of America","Missouri","Kansas City","Level 3 Communications Inc.","level3.com","DCH","3356","Level 3 Parent LLC","1"
"72322761","72322815","DCH","US","United States of America","California","Tustin","Level 3 Communications Inc.","level3.com","DCH","3356","Level 3 Parent LLC","1"
"84539546","84539546","DCH","DE","Germany","Sachsen","Falkenstein","Snow-Forecast.Com Ltd","your-server.de","DCH","24940","Hetzner Online GmbH","1"
"86867456","86867583","DCH","EE","Estonia","Ida-Virumaa","Johvi","P.A.G.M. Ou","fastvps.ee","DCH","198068","P.A.G.M. Ou","1"
"90504643","90504643","PUB","IL","Israel","HaMerkaz","Kafr Qasim","O.M.C. Computers & Communications Ltd","omc.co.il","DCH","44709","O.M.C. Computers & Communications Ltd","30"
"93900144","93900151","DCH","GB","United Kingdom of Great Britain and Northern Ireland","England","Milton Keynes","Dedicated Server Hosting","redstation.net.uk","DCH","20860","iomart Cloud Services Limited","1"
```

## Downloadable File Formats

- CSV: Comma-delimited text file with decimal ranges for direct database import or manual inspection.

- BIN: IP2Location binary format for use with official IP2Location or IP2Proxy libraries.

- CIDR: Comma-delimited text file with CIDR ranges, useful for firewall rules, network scanning, log analysis, and infrastructure automation.

## Sample Databases

| Format       | IPv4 Address                                                                                                          | IPv6 Address                                                                                                          |
|--------------|----------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------|
| **CSV**      | [Download Sample](https://github.com/ip2location/sample-databases/tree/main/IP2Proxy/PX8/ip2proxy-px8-sample.ipv4.csv) | [Download Sample](https://github.com/ip2location/sample-databases/tree/main/IP2Proxy/PX8/ip2proxy-px8-sample.ipv6.csv) |
| **BIN**      | [Download Sample](https://github.com/ip2location/sample-databases/tree/main/IP2Proxy/PX8/ip2proxy-px8-sample.ipv4.bin) | [Download Sample](https://github.com/ip2location/sample-databases/tree/main/IP2Proxy/PX8/ip2proxy-px8-sample.ipv6.bin) |
| **CIDR**     | [Download Sample](https://github.com/ip2location/sample-databases/tree/main/IP2Proxy/PX8/ip2proxy-px8-sample.ipv4.cidr.csv) | [Download Sample](https://github.com/ip2location/sample-databases/tree/main/IP2Proxy/PX8/ip2proxy-px8-sample.ipv6.cidr.csv) |


# Usage

### CSV File for Database Query

For details on importing the CSV file into a database and using SQL statements for IP lookup, please visit [](https://xxxxx)<https://www.ip2location.com/documentation/ip2proxy-database-px8#codes>

### BIN File for IP Lookup

To perform IP lookups with the BIN file, you’ll need to use the IP2Proxy SDK. Refer to the [development libraries](https://www.ip2location.com/development-libraries/?tab=ip2proxy) for usage instructions and integration guides.

# License

This sample data is provided by IP2Location.com for evaluation purposes. Please refer to the [licensing page](https://www.ip2location.com/licensing) for production licensing and usage.

# Useful Guides & Resources

For more information, please refer to the IP2Location.com official documentation at <https://www.ip2location.com/documentation/ip2proxy-database-px8>, which provides comprehensive details and usage guidelines.

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
