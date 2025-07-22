# IP2Location DB6 - IP Geolocation Database

## IP-Country-Region-City-Latitude-Longitude-ISP Database Sample

[IP2Location DB6 database](https://www.ip2location.com/database/db6-ip-country-region-city-latitude-longitude-isp) provides an IP geolocation solution to determine the country, region (state), city, latitude, longitude, and ISP of an IP address.

This repository provides a sample version of the IP2Location DB6 database in CSV, BIN, and CIDR formats. The sample includes a limited number of data rows and is not updated regularly. It is intended solely for evaluation and testing purposes—not for use in production environments.

For complete, high‑accuracy data with daily updates, please subscribe to the commercial IP2Location DB6 database.

## Database Fields

| **Name**      | **Type**                    | **Description**                             |
|---------------|-----------------------------|---------------------------------------------|
| ip_from       | INT(10) / Decimal(39,0)     | First IP address in netblock.               |
| ip_to         | INT(10) / Decimal(39,0)     | Last IP address in netblock.                |
| country_code  | CHAR(2)                     | Two-character country code based on ISO 3166. |
| country_name  | VARCHAR(64)                 | Country name based on ISO 3166.             |
| region_name   | VARCHAR(128)                | Region or state name.                       |
| city_name     | VARCHAR(128)                | City name.                                  |
| latitude      | DOUBLE                      | City latitude. Defaults to capital if unknown. |
| longitude     | DOUBLE                      | City longitude. Defaults to capital if unknown. |
| isp           | VARCHAR(256)                | Internet Service Provider or company name.  |

IP addresses are stored as 32-bit or 128-bit unsigned integers (depending on IPv4 or IPv6) and must be converted to standard IP notation for readability.

## Sample Rows in CSV Format
```csv
"16777216","16777471","CN","China","Beijing","Beijing","39.9042","116.4074","China Telecom"
"16777472","16777727","AU","Australia","Queensland","South Brisbane","-27.4766","153.0166","Telstra"
"16777728","16778239","CN","China","Beijing","Beijing","39.9042","116.4074","China Unicom"
"16778240","16779263","AU","Australia","Queensland","South Brisbane","-27.4766","153.0166","Telstra"
"16779264","16781311","CN","China","Beijing","Beijing","39.9042","116.4074","China Unicom"
"16781312","16785407","JP","Japan","Tokyo","Tokyo","35.6895","139.6917","SoftBank"
"16785408","16793599","CN","China","Guangdong","Guangzhou","23.1291","113.2644","China Telecom"
"16793600","16809983","CN","China","Beijing","Beijing","39.9042","116.4074","China Unicom"
"16809984","16842751","JP","Japan","Tokyo","Tokyo","35.6895","139.6917","NTT Communications"
```

## Downloadable File Formats

- CSV: Comma-delimited text file with decimal ranges for direct database import or manual inspection.

- BIN: IP2Location binary format for use with official IP2Location or IP2Proxy libraries.

- CIDR: Comma-delimited text file with CIDR ranges, useful for firewall rules, network scanning, log analysis, and infrastructure automation.

## Sample Databases

| Format       | IPv4 Address                                                                                                         | IPv6 Address                                                                                                         |
|--------------|---------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------|
| **CSV**      | [Download Sample](https://github.com/ip2location/sample-databases/tree/main/IP2Location/DB6/ip2location-db6-sample.ipv4.csv) | [Download Sample](https://github.com/ip2location/sample-databases/tree/main/IP2Location/DB6/ip2location-db6-sample.ipv6.csv) |
| **BIN**      | [Download Sample](https://github.com/ip2location/sample-databases/tree/main/IP2Location/DB6/ip2location-db6-sample.ipv4.bin) | [Download Sample](https://github.com/ip2location/sample-databases/tree/main/IP2Location/DB6/ip2location-db6-sample.ipv6.bin) |
| **CIDR**     | [Download Sample](https://github.com/ip2location/sample-databases/tree/main/IP2Location/DB6/ip2location-db6-sample.ipv4.cidr.csv) | [Download Sample](https://github.com/ip2location/sample-databases/tree/main/IP2Location/DB6/ip2location-db6-sample.ipv6.cidr.csv) |


# Usage

### CSV File for Database Query

For details on importing the CSV file into a database and using SQL statements for IP lookup, please visit <https://www.ip2location.com/documentation/ip2location-database-db6#codes>

### BIN File for IP Lookup

To perform IP lookups with the BIN file, you’ll need to use the IP2Location SDK. Refer to the [development libraries](https://www.ip2location.com/development-libraries/) for usage instructions and integration guides.

# License

This sample data is provided by IP2Location.com for evaluation purposes. Please refer to the [licensing page](https://www.ip2location.com/licensing) for production licensing and usage.

# Useful Guides & Resources

For more information, please refer to the IP2Location.com official documentation at <https://www.ip2location.com/documentation/ip2location-database-db6>, which provides comprehensive details and usage guidelines.

Alternatively, you may explore the articles at <https://blog.ip2location.com> for additional insights and practical examples.

# Other IP Geolocation Solutions

- [IP2Location.io IP Geolocation API](https://www.ip2location.io)

- [IP2Proxy Proxy Detection Database](https://www.ip2location.com/database/ip2proxy)

- [IP2Location LITE IP-ASN Database](https://lite.ip2location.com/database-asn)

- [IP2WHOIS WHOIS Domain Lookup](https://www.ip2whois.com/)

# About IP2Location

IP2Location.com offers extensive databases for IP geolocation. It enables users to precisely identify the geographical location of IP addresses, providing details such as country, region, city, district, latitude, longitude, ZIP code, time zone, connection speed, ISP, domain name, IDD country code, area code, weather station code and name, mobile carrier, elevation, usage type, address type, advertising category, and autonomous system.

These databases are invaluable for various use cases and applications, including website traffic analysis, fraud prevention, and personalized content delivery. By leveraging IP2Location’s data, businesses and developers can enhance their services, improve user experiences, and ensure more secure online interactions. IP2Location solution is available as a database and hosted API. If you are interested in web service instead of database, please visit [IP2Location.io](https://www.ip2location.io) for the remote hosted service.

Stay connected with us on [Facebook](https://www.facebook.com/ip2location), [X](https://x.com/ip2location), and [LinkedIn](https://www.linkedin.com/company/ip2location) for more insights into IP address data and its powerful applications.
