# IP2PROXY PX3 - Proxy Detection Database

## IP-ProxyType-Country-Region-City Database

[IP2Proxy PX3 Database](https://www.ip2location.com/database/px3-ip-proxytype-country-region-city) provides proxy data like proxy type, country, region or state, and city of IP address.

This repository provides a sample version of the IP2Proxy PX3 database in CSV, BIN, and CIDR formats. The sample includes a limited number of data rows and is not updated regularly. It is intended solely for evaluation and testing purposes—not for use in production environments. 

For complete, high-accuracy data with up to daily updates, please subscribe to the commercial IP2Proxy PX3 database.

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

IP addresses are stored as 32-bit or 128-bit unsigned integers (depending on IPv4 or IPv6) and must be converted to standard IP notation for readability.

## Sample Rows in CSV Format
```csv
"37433895","37433895","PUB","RU","Russian Federation","Moskva","Moscow"
"51270344","51270467","DCH","US","United States of America","Ohio","Columbus"
"51861318","51861374","DCH","US","United States of America","Ohio","Columbus"
"56230726","56230726","PUB","US","United States of America","Virginia","Ashburn"
"58926359","58926417","DCH","US","United States of America","Ohio","Columbus"
"59681738","59681788","DCH","US","United States of America","Ohio","Columbus"
"60104056","60104056","SES","US","United States of America","Ohio","Columbus"
"67201293","67201293","DCH","US","United States of America","Texas","Dallas"
"68316705","68316705","DCH","US","United States of America","Arizona","Phoenix"
"69493632","69493759","DCH","US","United States of America","California","Tustin"
"71689985","71689986","DCH","US","United States of America","Massachusetts","Boston"
"84511931","84511985","DCH","DE","Germany","Sachsen","Falkenstein"
"86878531","86878531","PUB","ES","Spain","Andalucia","Jaen"
"90558975","90558975","PUB","RU","Russian Federation","Krasnodarskiy kray","Taman'"
"94208993","94208993","VPN","ES","Spain","Madrid, Comunidad de","Pinar de Chamartin"
```

## Downloadable File Formats

- CSV: Comma-delimited text file with decimal ranges for direct database import or manual inspection.

- BIN: IP2Location binary format for use with official IP2Location or IP2Proxy libraries.

- CIDR: Comma-delimited text file with CIDR ranges, useful for firewall rules, network scanning, log analysis, and infrastructure automation.

## Sample Databases

| Format       | IPv4 Address                                                                                                        | IPv6 Address                                                                                                        |
|--------------|--------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------|
| **CSV**      | [Download Sample](https://github.com/ip2location/sample-databases/tree/main/IP2Proxy/PX3/ip2proxy-px3-sample.ipv4.csv) | [Download Sample](https://github.com/ip2location/sample-databases/tree/main/IP2Proxy/PX3/ip2proxy-px3-sample.ipv6.csv) |
| **BIN**      | [Download Sample](https://github.com/ip2location/sample-databases/tree/main/IP2Proxy/PX3/ip2proxy-px3-sample.ipv4.bin) | [Download Sample](https://github.com/ip2location/sample-databases/tree/main/IP2Proxy/PX3/ip2proxy-px3-sample.ipv6.bin) |


# Usage

### CSV File for Database Query

For details on importing the CSV file into a database and using SQL statements for IP lookup, please visit [](https://xxxxx)<https://www.ip2location.com/documentation/ip2proxy-database-px3#codes>

### BIN File for IP Lookup

To perform IP lookups with the BIN file, you’ll need to use the IP2Proxy SDK. Refer to the [development libraries](https://www.ip2location.com/development-libraries/?tab=ip2proxy) for usage instructions and integration guides.

# License

This sample data is provided by IP2Location.com for evaluation purposes. Please refer to the [licensing page](https://www.ip2location.com/licensing) for production licensing and usage.

# Useful Guides & Resources

For more information, please refer to the IP2Location.com official documentation at <https://www.ip2location.com/documentation/ip2proxy-database-px3>, which provides comprehensive details and usage guidelines.

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
