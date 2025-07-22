# IP2PROXY PX2 - Proxy Detection Database

## IP-ProxyType-Country Database Sample

[IP2Proxy PX2 Database](https://www.ip2location.com/database/px2-ip-proxytype-country) provides proxy data like proxy type and country of IP address.

This repository provides a sample version of the IP2Proxy PX2 database in CSV, BIN, and CIDR formats. The sample includes a limited number of data rows and is not updated regularly. It is intended solely for evaluation and testing purposes—not for use in production environments. 

For complete, high-accuracy data with up to daily updates, please subscribe to the commercial IP2Proxy PX2 database.

## Database Fields

| **Name** | **Type** | **Description** |
| --- | --- | --- |
| ip_from | INT(10)  / Decimal(39,0) | First IP address in netblock. |
| ip_to | INT(10)  / Decimal(39,0) | Last IP address in netblock. |
| proxy_type | VARCHAR(3) | Type of proxy. |
| country_code | CHAR(2) | Two-character country code based on ISO 3166. |
| country_name | VARCHAR(64) | Country name based on ISO 3166. |

IP addresses are stored as 32-bit or 128-bit unsigned integers (depending on IPv4 or IPv6) and must be converted to standard IP notation for readability.

## Sample Rows in CSV Format
```csv
"41310832","41310835","DCH","IT","Italy"
"51762951","51762951","PUB","US","United States of America"
"56183162","56183162","PUB","US","United States of America"
"59382778","59382778","PUB","US","United States of America"
"61193734","61193778","DCH","US","United States of America"
"66871059","66871059","PUB","IE","Ireland"
"80280404","80280407","PUB","AU","Australia"
"86218864","86218864","VPN","RU","Russian Federation"
"89008934","89008934","PUB","US","United States of America"
"93673782","93673782","PUB","BA","Bosnia and Herzegovina"
"95791353","95791355","DCH","TR","Turkiye"
"100455471","100455471","DCH","PL","Poland"
"147945326","147945326","PUB","DE","Germany"
"155261666","155262265","DCH","US","United States of America"
"208242096","208242103","DCH","US","United States of America"
"216327264","216327271","DCH","US","United States of America"
"223049754","223049767","DCH","HK","Hong Kong"
"232018274","232018280","DCH","SG","Singapore"
```

## Downloadable File Formats

- CSV: Comma-delimited text file with decimal ranges for direct database import or manual inspection.

- BIN: IP2Location binary format for use with official IP2Location or IP2Proxy libraries.

- CIDR: Comma-delimited text file with CIDR ranges, useful for firewall rules, network scanning, log analysis, and infrastructure automation.

## Sample Databases

| Format       | IPv4 Address                                                                                                          | IPv6 Address                                                                                                          |
|--------------|----------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------|
| **CSV**      | [Download Sample](https://github.com/ip2location/sample-databases/tree/main/IP2Proxy/PX2/ip2proxy-px2-sample.ipv4.csv) | [Download Sample](https://github.com/ip2location/sample-databases/tree/main/IP2Proxy/PX2/ip2proxy-px2-sample.ipv6.csv) |
| **BIN**      | [Download Sample](https://github.com/ip2location/sample-databases/tree/main/IP2Proxy/PX2/ip2proxy-px2-sample.ipv4.bin) | [Download Sample](https://github.com/ip2location/sample-databases/tree/main/IP2Proxy/PX2/ip2proxy-px2-sample.ipv6.bin) |
| **CIDR**     | [Download Sample](https://github.com/ip2location/sample-databases/tree/main/IP2Proxy/PX2/ip2proxy-px2-sample.ipv4.cidr.csv) | [Download Sample](https://github.com/ip2location/sample-databases/tree/main/IP2Proxy/PX2/ip2proxy-px2-sample.ipv6.cidr.csv) |


# Usage

### CSV File for Database Query

For details on importing the CSV file into a database and using SQL statements for IP lookup, please visit [](https://xxxxx)<https://www.ip2location.com/documentation/ip2proxy-database-px2#codes>

### BIN File for IP Lookup

To perform IP lookups with the BIN file, you’ll need to use the IP2Proxy SDK. Refer to the [development libraries](https://www.ip2location.com/development-libraries/?tab=ip2proxy) for usage instructions and integration guides.

# License

This sample data is provided by IP2Location.com for evaluation purposes. Please refer to the [licensing page](https://www.ip2location.com/licensing) for production licensing and usage.

# Useful Guides & Resources

For more information, please refer to the IP2Location.com official documentation at <https://www.ip2location.com/documentation/ip2proxy-database-px2>, which provides comprehensive details and usage guidelines.

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
