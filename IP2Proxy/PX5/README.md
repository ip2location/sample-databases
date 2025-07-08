# IP2PROXY PX5 - Proxy Detection Database

## IP-ProxyType-Country-Region-City-ISP-Domain Database

[IP2Proxy PX5 Database](https://www.ip2location.com/database/px5-ip-proxytype-country-region-city-isp-domain) provides proxy data like proxy type, country, region or state, city, Internet Service Provider (ISP) and domain of IP address.

This repository provides a sample version of the IP2Proxy PX5 database in CSV, BIN, and CIDR formats. The sample includes a limited number of data rows and is not updated regularly. It is intended solely for evaluation and testing purposes—not for use in production environments. 

For complete, high-accuracy data with up to daily updates, please subscribe to the commercial IP2Proxy PX5 database.

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

IP addresses are stored as 32-bit or 128-bit unsigned integers (depending on IPv4 or IPv6) and must be converted to standard IP notation for readability.

## Sample Rows in CSV Format
```csv
"37376007","37376007","PUB","DE","Germany","Brandenburg","Karlsruhe","Contabo GmbH","contabo.com"
"51108075","51108118","DCH","GB","United Kingdom of Great Britain and Northern Ireland","England","London","Amazon Data Services UK","amazon.com"
"51749876","51749897","DCH","US","United States of America","Ohio","Columbus","Amazon Technologies Inc.","amazon.com"
"55970864","55971321","DCH","US","United States of America","Virginia","Ashburn","Amazon Data Services NoVa","amazon.com"
"58419445","58420734","DCH","DE","Germany","Hessen","Frankfurt am Main","A100 ROW GmbH","amazon.com"
"59464192","59464192","SES","US","United States of America","Ohio","Columbus","Amazon Technologies Inc.","amazon.com"
"59881329","59881329","SES","US","United States of America","Ohio","Columbus","Amazon Technologies Inc.","amazon.com"
"65767239","65767363","DCH","US","United States of America","Virginia","Ashburn","Amazon Data Services NoVa","amazon.com"
"68039361","68039362","DCH","US","United States of America","Oklahoma","Tulsa","Level 3 Communications Inc.","level3.com"
"68816896","68817429","DCH","US","United States of America","New Jersey","Newark","Level 3 Communications Inc.","level3.com"
"71575133","71575134","DCH","NL","Netherlands (Kingdom of the)","Noord-Holland","Amsterdam","Level 3 Communications Inc.","level3.com"
"80952425","80958653","DCH","FR","France","Ile-de-France","Paris","Microsoft Corporation","microsoft.com"
"86206955","86206975","DCH","KZ","Kazakhstan","Almaty oblysy","Dostyk","Cloud Services Kazakhstan LLP","yandex.com"
"88842157","88842157","PUB","DE","Germany","Bayern","Nuremberg","Hetzner Online GmbH","hetzner.de"
"92652200","92652200","PUB","SE","Sweden","Stockholms lan","Stockholm","Internet Vikings International AB","internetvikings.com"
"94449369","94449407","DCH","US","United States of America","Virginia","Ashburn","Hetzner Online GmbH","hetzner.de"
"96263010","96263010","PUB","SE","Sweden","-","-","Petersburg Internet Network Ltd.","pinspb.ru"
```

## Downloadable File Formats

- CSV: Comma-delimited text file with decimal ranges for direct database import or manual inspection.

- BIN: IP2Location binary format for use with official IP2Location or IP2Proxy libraries.

- CIDR: Comma-delimited text file with CIDR ranges, useful for firewall rules, network scanning, log analysis, and infrastructure automation.

## Sample Databases

| Format       | IPv4 Address                                                                                                        | IPv6 Address                                                                                                        |
|--------------|--------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------|
| **CSV**      | [Download Sample](https://github.com/ip2location/sample-databases/tree/main/IP2Proxy/PX5/ip2proxy-px5-sample.ipv4.csv) | [Download Sample](https://github.com/ip2location/sample-databases/tree/main/IP2Proxy/PX5/ip2proxy-px5-sample.ipv6.csv) |
| **BIN**      | [Download Sample](https://github.com/ip2location/sample-databases/tree/main/IP2Proxy/PX5/ip2proxy-px5-sample.ipv4.bin) | [Download Sample](https://github.com/ip2location/sample-databases/tree/main/IP2Proxy/PX5/ip2proxy-px5-sample.ipv6.bin) |


# Usage

### CSV File for Database Query

For details on importing the CSV file into a database and using SQL statements for IP lookup, please visit [](https://xxxxx)<https://www.ip2location.com/documentation/ip2proxy-database-px5#codes>

### BIN File for IP Lookup

To perform IP lookups with the BIN file, you’ll need to use the IP2Proxy SDK. Refer to the [development libraries](https://www.ip2location.com/development-libraries/?tab=ip2proxy) for usage instructions and integration guides.

# License

This sample data is provided by IP2Location.com for evaluation purposes. Please refer to the [licensing page](https://www.ip2location.com/licensing) for production licensing and usage.

# Useful Guides & Resources

For more information, please refer to the IP2Location.com official documentation at <https://www.ip2location.com/documentation/ip2proxy-database-px5>, which provides comprehensive details and usage guidelines.

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
