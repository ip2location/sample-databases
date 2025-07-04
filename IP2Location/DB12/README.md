# IP2Location DB12 – IP Geolocation Database

## IP-Country-Region-City-Latitude-Longitude-ZIPCode-TimeZone-ISP-Domain Database Sample

[IP2Location DB12 database](https://www.ip2location.com/database/db12-ip-country-region-city-latitude-longitude-zipcode-timezone-isp-domain) provides an IP geolocation solution to determine the country, region or state, city, latitude, longitude, ZIP/postal code, time zone, ISP, and domain of an IP address. 

This repository offers a sample version of the IP2Location DB12 database in CSV, BIN, and CIDR formats. The sample includes a limited number of data rows and is intended solely for evaluation and testing—not for production use. For full, high‑accuracy data with daily updates, please subscribe to the commercial IP2Location DB12 database. 

## Database Fields

| **Name**        | **Type**                    | **Description**                                                                 |
|-----------------|-----------------------------|---------------------------------------------------------------------------------|
| ip_from         | INT(10) / Decimal(39,0)     | First IP address in the netblock.                                              |
| ip_to           | INT(10) / Decimal(39,0)     | Last IP address in the netblock.                                               |
| country_code    | CHAR(2)                     | Two-character country code (ISO 3166).                                         |
| country_name    | VARCHAR(64)                 | Country name.                                                                  |
| region_name     | VARCHAR(128)                | Region or state name.                                                          |
| city_name       | VARCHAR(128)                | City name.                                                                     |
| latitude        | DOUBLE                      | City latitude. Defaults to capital if city is unknown.                          |
| longitude       | DOUBLE                      | City longitude. Defaults to capital if city is unknown.                         |
| zip_code         | VARCHAR(30)                 | ZIP or postal code.                                                            |
| time_zone        | VARCHAR(32)                 | UTC time zone (with DST supported).                              |
| isp             | VARCHAR(256)                | Internet Service Provider or company name.                                     |
| domain          | VARCHAR(128)                | Internet domain name associated with IP address range.							|

IP addresses are stored as 32-bit or 128-bit unsigned integers (depending on IPv4 or IPv6) and must be converted to dotted‑decimal or standard notation for readability.

## Sample Rows in CSV Format
```csv
"67260168","67260175","US","United States of America","Ohio","Cincinnati","39.162000","-84.456890","45950","-04:00","Intelletrace Panattoni","intelletrace.com"
"67260176","67260415","US","United States of America","Ohio","Cincinnati","39.162000","-84.456890","45950","-04:00","Level 3 Communications Inc.","level3.com"
"67260416","67260927","US","United States of America","Massachusetts","Boston","42.358478","-71.060075","02117","-04:00","Level 3 Communications Inc.","level3.com"
"67260928","67261439","US","United States of America","Louisiana","Monroe","32.524505","-92.128516","71203","-05:00","Level 3 Communications Inc.","level3.com"
"67261440","67261697","US","United States of America","Washington","Seattle","47.604309","-122.329845","98164","-07:00","Level 3 Communications Inc.","level3.com"
"67261698","67261698","US","United States of America","Massachusetts","Burlington","42.504820","-71.195610","01803","-04:00","Level 3 Communications Inc.","level3.com"
"67261699","67262203","US","United States of America","Washington","Seattle","47.604309","-122.329845","98164","-07:00","Level 3 Communications Inc.","level3.com"
"67262204","67262207","US","United States of America","Washington","Seattle","47.604309","-122.329845","98164","-07:00","Survitec Canada","level3.net"
"67262208","67262463","US","United States of America","Washington","Seattle","47.604309","-122.329845","98164","-07:00","Level 3 Communications Inc.","level3.com"
"67262464","67262975","US","United States of America","Oklahoma","Tulsa","36.153980","-95.992780","74172","-05:00","Level 3 Communications Inc.","level3.com"
"67262976","67264063","US","United States of America","Louisiana","Monroe","32.524505","-92.128516","71203","-05:00","Level 3 Communications Inc.","level3.com"
"67264064","67264071","US","United States of America","South Dakota","Rapid City","44.080550","-103.231053","57709","-06:00","Respec Inc","respec.com"
"67264072","67264511","US","United States of America","Louisiana","Monroe","32.524505","-92.128516","71203","-05:00","Level 3 Communications Inc.","level3.com"
"67264512","67265023","US","United States of America","Tennessee","Nashville","36.166290","-86.784440","37219","-05:00","Level 3 Communications Inc.","level3.com"
"67265024","67265535","US","United States of America","Louisiana","Monroe","32.524505","-92.128516","71203","-05:00","Level 3 Communications Inc.","level3.com"
"67265536","67265791","US","United States of America","New Jersey","Newark","40.732277","-74.173575","07102","-04:00","Level 3 Communications Inc.","level3.com"
```

## Downloadable File Formats

- CSV: Comma-delimited text file with decimal ranges for direct database import or manual inspection.

- BIN: IP2Location binary format for use with official IP2Location or IP2Proxy libraries.

- CIDR: Comma-delimited text file with CIDR ranges, useful for firewall rules, network scanning, log analysis, and infrastructure automation.

## Sample Databases

| Format       | IPv4 Address                                                                                                         | IPv6 Address                                                                                                         |
|--------------|---------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------|
| **CSV** | [Download Sample](https://github.com/ip2location/sample-databases/tree/main/IP2Location/DB12/ip2location-DB12-sample.ipv4.csv) | [Download Sample](https://github.com/ip2location/sample-databases/tree/main/IP2Location/DB12/ip2location-DB12-sample.ipv6.csv) |
| **BIN** | [Download Sample](https://github.com/ip2location/sample-databases/tree/main/IP2Location/DB12/ip2location-DB12-sample.ipv4.bin) | [Download Sample](https://github.com/ip2location/sample-databases/tree/main/IP2Location/DB12/ip2location-DB12-sample.ipv6.bin) |

# Usage

### CSV File for Database Query

For details on importing the CSV file into a database and using SQL statements for IP lookup, please visit <https://www.ip2location.com/documentation/ip2location-database-DB12#codes>

### BIN File for IP Lookup

To perform IP lookups with the BIN file, you’ll need to use the IP2Location SDK. Refer to the [development libraries](https://www.ip2location.com/development-libraries/) for usage instructions and integration guides.

# License

This sample data is provided by IP2Location.com for evaluation purposes. Please refer to the [licensing page](https://www.ip2location.com/licensing) for production licensing and usage.

# Useful Guides & Resources

For more information, please refer to the IP2Location.com official documentation at <https://www.ip2location.com/documentation/ip2location-database-DB12>, which provides comprehensive details and usage guidelines.

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