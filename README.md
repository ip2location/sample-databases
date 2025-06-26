# IP2Location Sample Databases

IP2Location is a leading IP geolocation provider, offering solutions for IP Gelocation Lookup and Proxy Detection.

IP2Location IP Geolocation is an accurate database solution that allows you to determine the geographical location of an IP address. It maps IP addresses to a wide range of data fields such as country, region or state, district, city, latitude and longitude, ZIP/Postal code, time zone, Internet Service Provider (ISP) or company name, domain name, net speed, area code, weather station code, weather station name, mobile country code (MCC), mobile network code (MNC) and carrier brand, elevation, usage type, address type, IAB category and ASN of IP address.

IP2Proxy Proxy Detection contains proxy-related information including country, region, city, ISP, domain, usage type, ASN, last seen date, threat reported, VPN provider name and fraud score. It detects anonymous proxy, VPNs (VPN), open proxies (PUB), web proxies (WEB), Tor exit nodes (TOR), data center and hosting IPs (DCH), search engine spiders (SES), residential proxies (RES), consumer privacy networks (CPN), and enterprise private networks (EPN).

This repository contains sample datasets for IP2Location and IP2Proxy—an ideal starting point for developers to explore the data format, field structure, and integration workflows

# Databases

| Database Product | Description | Sample Database |
| --- | --- | --- |
| IP2Location IP Geolocation | There are a total of 26 package databases that help businesses identify the geographic location of their website visitors. | <https://github.com/ip2location/sample-databases/tree/main/IP2Location> |
| IP2Proxy Proxy Detection | There are a total of 12 package databases that help businesses to detect IP anonymizers. | <https://github.com/ip2location/sample-databases/tree/main/IP2Prox> |

# Repository Highlights

There are 26 database samples for IP2Location IP Geolocation and 12 database samples for IP2Proxy Proxy Detection. Please visit each folder to learn more about the databases. In the each folder, you will find:

- Sample datasets available for both IPv4 and IPv6
- Detailed field descriptions and dataset structure
- Useful guides, resources, articles, and example code snippets

# Database Overview

## IP2Location IP Geolocation Database

IP2Location delivers a precise, modular IP geolocation solution that maps any IPv4 or IPv6 address to a comprehensive set of data fields—from basic geographic information to advanced network intelligence. Organized into 26 distinct database packages, the system lets you customize integration based on the level of granularity you require. Supported formats include BIN, CSV and CIDR.

### IP2Location IP Geolocation Database Packages

| **Product Code** | **Database Name** |
| --- | --- |
| DB1 | [IP-Country](https://github.com/ip2location/sample-databases/tree/main/IP2Location/DB1) |
| DB2 | [IP-Country-ISP](https://github.com/ip2location/sample-databases/tree/main/IP2Location/DB2) |
| DB3 | [IP-Country-Region-City](https://github.com/ip2location/sample-databases/tree/main/IP2Location/DB3) |
| DB4 | [IP-Country-Region-City-ISP](https://github.com/ip2location/sample-databases/tree/main/IP2Location/DB4) |
| DB5 | [IP-Country-Region-City-Latitude-Longitude](https://github.com/ip2location/sample-databases/tree/main/IP2Location/DB5) |
| DB6 | [IP-Country-Region-City-Latitude-Longitude-ISP](https://github.com/ip2location/sample-databases/tree/main/IP2Location/DB6) |
| DB7 | [IP-Country-Region-City-ISP-Domain](https://github.com/ip2location/sample-databases/tree/main/IP2Location/DB7) |
| DB8 | [IP-Country-Region-City-Latitude-Longitude-ISP-Domain](https://github.com/ip2location/sample-databases/tree/main/IP2Location/DB8) |
| DB9 | [IP-Country-Region-City-Latitude-Longitude-ZIPCode](https://github.com/ip2location/sample-databases/tree/main/IP2Location/DB9) |
| DB10 | [IP-Country-Region-City-Latitude-Longitude-ZIPCode-ISP-Domain](https://github.com/ip2location/sample-databases/tree/main/IP2Location/DB10) |
| DB11 | [IP-Country-Region-City-Latitude-Longitude-ZIPCode-TimeZone](https://github.com/ip2location/sample-databases/tree/main/IP2Location/DB11) |
| DB12 | [IP-Country-Region-City-Latitude-Longitude-ZIPCode-TimeZone-ISP-Domain](https://github.com/ip2location/sample-databases/tree/main/IP2Location/DB12) |
| DB13 | [IP-Country-Region-City-Latitude-Longitude-TimeZone-NetSpeed](https://github.com/ip2location/sample-databases/tree/main/IP2Location/DB13) |
| DB14 | [IP-Country-Region-City-Latitude-Longitude-ZIPCode-TimeZone-ISP-Domain-NetSpeed](https://github.com/ip2location/sample-databases/tree/main/IP2Location/DB14) |
| DB15 | [IP-Country-Region-City-Latitude-Longitude-ZIPCode-TimeZone-AreaCode](https://github.com/ip2location/sample-databases/tree/main/IP2Location/DB15) |
| DB16 | [IP-Country-Region-City-Latitude-Longitude-ZIPCode-TimeZone-ISP-Domain-NetSpeed-AreaCode](https://github.com/ip2location/sample-databases/tree/main/IP2Location/DB16) |
| DB17 | [IP-Country-Region-City-Latitude-Longitude-TimeZone-NetSpeed-Weather](https://github.com/ip2location/sample-databases/tree/main/IP2Location/DB17) |
| DB18 | [IP-Country-Region-City-Latitude-Longitude-ZIPCode-TimeZone-ISP-Domain-NetSpeed-AreaCode-Weather](https://github.com/ip2location/sample-databases/tree/main/IP2Location/DB18) |
| DB19 | [IP-Country-Region-City-Latitude-Longitude-ISP-Domain-Mobile](https://github.com/ip2location/sample-databases/tree/main/IP2Location/DB19) |
| DB20 | [IP-Country-Region-City-Latitude-Longitude-ZIPCode-TimeZone-ISP-Domain-NetSpeed-AreaCode-Weather-Mobile](https://github.com/ip2location/sample-databases/tree/main/IP2Location/DB20) |
| DB21 | [IP-Country-Region-City-Latitude-Longitude-ZIPCode-TimeZone-AreaCode-Elevation](https://github.com/ip2location/sample-databases/tree/main/IP2Location/DB21) |
| DB22 | [IP-Country-Region-City-Latitude-Longitude-ZIPCode-TimeZone-ISP-Domain-NetSpeed-AreaCode-Weather-Mobile-Elevation](https://github.com/ip2location/sample-databases/tree/main/IP2Location/DB22) |
| DB23 | [IP-Country-Region-City-Latitude-Longitude-ISP-Domain-Mobile-UsageType](https://github.com/ip2location/sample-databases/tree/main/IP2Location/DB23) |
| DB24 | [IP-Country-Region-City-Latitude-Longitude-ZIPCode-TimeZone-ISP-Domain-NetSpeed-AreaCode-Weather-Mobile-Elevation-UsageType](https://github.com/ip2location/sample-databases/tree/main/IP2Location/DB24) |
| DB25 | [IP-Country-Region-City-Latitude-Longitude-ZIPCode-TimeZone-ISP-Domain-NetSpeed-AreaCode-Weather-Mobile-Elevation-UsageType-AddressType-Category](https://github.com/ip2location/sample-databases/tree/main/IP2Location/DB25) |
| DB26 | [IP-Country-Region-City-Latitude-Longitude-ZIPCode-TimeZone-ISP-Domain-NetSpeed-AreaCode-Weather-Mobile-Elevation-UsageType-AddressType-Category-District-ASN](https://github.com/ip2location/sample-databases/tree/main/IP2Location/DB26) |

### IP2Location IP Geolocation Database Packages Comparison

| DB  | Country | Region & City | Latitude & Longitude | ZIP Code | ISP | Domain | Time Zone | Net Speed | Area Code | Weather | Mobile | Elevation | Usage Type | Address Type | Category | District | ASN |
|-----|---------|----------------|-----------------------|----------|-----|--------|------------|------------|------------|---------|--------|-----------|-------------|--------------|----------|----------|-----|
| DB1 | ✔       |                |                       |          |     |        |            |            |            |         |        |           |             |              |          |          |     |
| DB2 | ✔       |                |                       |          | ✔   |        |            |            |            |         |        |           |             |              |          |          |     |
| DB3 | ✔       | ✔              |                       |          |     |        |            |            |            |         |        |           |             |              |          |          |     |
| DB4 | ✔       | ✔              | ✔                     |          | ✔   |        |            |            |            |         |        |           |             |              |          |          |     |
| DB5 | ✔       | ✔              | ✔                     |          |     |        |            |            |            |         |        |           |             |              |          |          |     |
| DB6 | ✔       | ✔              | ✔                     |          | ✔   |        |            |            |            |         |        |           |             |              |          |          |     |
| DB7 | ✔       | ✔              |                       |          | ✔   | ✔      |            |            |            |         |        |           |             |              |          |          |     |
| DB8 | ✔       | ✔              | ✔                     |          | ✔   | ✔      |            |            |            |         |        |           |             |              |          |          |     |
| DB9 | ✔       | ✔              | ✔                     | ✔        |     |        |            |            |            |         |        |           |             |              |          |          |     |
| DB10| ✔       | ✔              | ✔                     | ✔        | ✔   | ✔      |            |            |            |         |        |           |             |              |          |          |     |
| DB11| ✔       | ✔              | ✔                     | ✔        |     |        | ✔          |            |            |         |        |           |             |              |          |          |     |
| DB12| ✔       | ✔              | ✔                     | ✔        | ✔   | ✔      | ✔          |            |            |         |        |           |             |              |          |          |     |
| DB13| ✔       | ✔              | ✔                     |          |     |        | ✔          | ✔          |            |         |        |           |             |              |          |          |     |
| DB14| ✔       | ✔              | ✔                     | ✔        | ✔   | ✔      | ✔          | ✔          |            |         |        |           |             |              |          |          |     |
| DB15| ✔       | ✔              | ✔                     | ✔        |     |        | ✔          |            | ✔          |         |        |           |             |              |          |          |     |
| DB16| ✔       | ✔              | ✔                     | ✔        | ✔   | ✔      | ✔          | ✔          | ✔          |         |        |           |             |              |          |          |     |
| DB17| ✔       | ✔              | ✔                     |          |     |        | ✔          | ✔          |            | ✔       |        |           |             |              |          |          |     |
| DB18| ✔       | ✔              | ✔                     | ✔        | ✔   | ✔      | ✔          | ✔          | ✔          | ✔       |        |           |             |              |          |          |     |
| DB19| ✔       | ✔              | ✔                     |          | ✔   | ✔      |            |            |            |         | ✔      |           |             |              |          |          |     |
| DB20| ✔       | ✔              | ✔                     | ✔        | ✔   | ✔      | ✔          | ✔          | ✔          | ✔       | ✔      |           |             |              |          |          |     |
| DB21| ✔       | ✔              | ✔                     | ✔        |     |        | ✔          |            | ✔          |         |        | ✔         |             |              |          |          |     |
| DB22| ✔       | ✔              | ✔                     | ✔        | ✔   | ✔      | ✔          | ✔          | ✔          | ✔       | ✔      | ✔         |             |              |          |          |     |
| DB23| ✔       | ✔              | ✔                     |          | ✔   | ✔      |            |            |            |         | ✔      |           | ✔           |              |          |          |     |
| DB24| ✔       | ✔              | ✔                     | ✔        | ✔   | ✔      | ✔          | ✔          | ✔          | ✔       | ✔      | ✔         | ✔           |              |          |          |     |
| DB25| ✔       | ✔              | ✔                     | ✔        | ✔   | ✔      | ✔          | ✔          | ✔          | ✔       | ✔      | ✔         | ✔           | ✔            | ✔        |         |     |
| DB26| ✔       | ✔              | ✔                     | ✔        | ✔   | ✔      | ✔          | ✔          | ✔          | ✔       | ✔      | ✔         | ✔           | ✔            | ✔        | ✔        | ✔   |


## IP2Proxy Proxy Detection Database

The IP2Proxy Proxy Detection Database is a specialized dataset designed to identify IP addresses linked to anonymized or non-legitimate traffic sources. It detects a broad spectrum of proxy types, including VPNs (VPN), open proxies (PUB), web proxies (WEB), Tor exit nodes (TOR), data center and hosting IPs (DCH), search engine spiders (SES), residential proxies (RES), consumer privacy networks (CPN), and enterprise private networks (EPN).

Available in 12 structured packages with varying levels of granularity—such as autonomous system number, last seen date, threat type, provider name, and fraud score—IP2Proxy empowers developers, analysts, and security platforms to programmatically flag, filter, or block potentially high-risk IP addresses with accuracy and efficiency.

### IP2Proxy Proxy Detection Database Packages

| **Product Code** | **Database Name** |
| --- | --- |
| PX1 | [IP‑Country](https://github.com/ip2location/sample-databases//tree/main/IP2Proxy/PX1) |
| PX2 | [IP‑ProxyType‑Country](https://github.com/ip2location/sample-databases//tree/main/IP2Proxy/PX2) |
| PX3 | [IP‑ProxyType‑Country‑Region‑City](https://github.com/ip2location/sample-databases//tree/main/IP2Proxy/PX3) |
| PX4 | [IP‑ProxyType‑Country‑Region‑City‑ISP](https://github.com/ip2location/sample-databases//tree/main/IP2Proxy/PX4) |
| PX5 | [IP‑ProxyType‑Country‑Region‑City‑ISP‑Domain](https://github.com/ip2location/sample-databases//tree/main/IP2Proxy/PX5) |
| PX6 | [IP-ProxyType-Country-Region-City-ISP-Domain-UsageType](https://github.com/ip2location/sample-databases//tree/main/IP2Proxy/PX6) |
| PX7 | [IP-ProxyType-Country-Region-City-ISP-Domain-UsageType-ASN](https://github.com/ip2location/sample-databases//tree/main/IP2Proxy/PX7) |
| PX8 | [IP-ProxyType-Country-Region-City-ISP-Domain-UsageType-ASN-LastSeen](https://github.com/ip2location/sample-databases//tree/main/IP2Proxy/PX8) |
| PX9 | [IP-ProxyType-Country-Region-City-ISP-Domain-UsageType-ASN-LastSeen-Threat](https://github.com/ip2location/sample-databases//tree/main/IP2Proxy/PX9) |
| PX10 | [IP-ProxyType-Country-Region-City-ISP-Domain-UsageType-ASN-LastSeen-Threat-Residential](https://github.com/ip2location/sample-databases//tree/main/IP2Proxy/PX10) |
| PX11 | [IP-ProxyType-Country-Region-City-ISP-Domain-UsageType-ASN-LastSeen-Threat-Residential-Provider](https://github.com/ip2location/sample-databases//tree/main/IP2Proxy/PX11) |
| PX12 | [IP-ProxyType-Country-Region-City-ISP-Domain-UsageType-ASN-LastSeen-Threat-Residential-Provider-FraudScore](https://github.com/ip2location/sample-databases//tree/main/IP2Proxy/PX12) |

### IP2Proxy Proxy Detection Database Packages Comparison

| Product | Country | Proxy Type | Region & City | ISP | Domain | Usage Type | ASN | Last Seen | Threat | Residential Proxy | Provider | Fraud Score |
|---------|---------|------------|----------------|-----|--------|-------------|-----|-----------|--------|--------------------|----------|--------------|
| PX1     | ✔      |            |                |     |        |             |     |           |        |                    |          |              |
| PX2     | ✔      | 6         |                |     |        |             |     |           |        |                    |          |              |
| PX3     | ✔      | 6         | ✔             |     |        |             |     |           |        |                    |          |              |
| PX4     | ✔      | 6         | ✔             | ✔  |        |             |     |           |        |                    |          |              |
| PX5     | ✔      | 6         | ✔             | ✔  | ✔     |             |     |           |        |                    |          |              |
| PX6     | ✔      | 6         | ✔             | ✔  | ✔     | ✔          |     |           |        |                    |          |              |
| PX7     | ✔      | 6         | ✔             | ✔  | ✔     | ✔          | ✔  |           |        |                    |          |              |
| PX8     | ✔      | 6         | ✔             | ✔  | ✔     | ✔          | ✔  | ✔        |        |                    |          |              |
| PX9     | ✔      | 6         | ✔             | ✔  | ✔     | ✔          | ✔  | ✔        | ✔     |                    |          |              |
| PX10    | ✔      | 7         | ✔             | ✔  | ✔     | ✔          | ✔  | ✔        | ✔     | ✔                 |          |              |
| PX11    | ✔      | 9         | ✔             | ✔  | ✔     | ✔          | ✔  | ✔        | ✔     | ✔                 | ✔       |              |
| PX12    | ✔      | 9         | ✔             | ✔  | ✔     | ✔          | ✔  | ✔        | ✔     | ✔                 | ✔       | ✔           |

## Supported Formats

Each sample may includes:

\- CSV: Comma-delimited text file with decimal ranges for direct database import or manual inspection.

\- BIN: IP2Location binary format for use with official IP2Location or IP2Proxy libraries.

\- CIDR: Comma-delimited text file with CIDR ranges, useful for firewall rules, network scanning, log analysis, and infrastructure automation.

# Useful Guides & Resources

For more information, please refer to the IP2Location.com official documentation at <https://www.ip2location.com/documentation/main>, which provides comprehensive details and usage guidelines.

Alternatively, you may explore the articles at <https://blog.ip2location.com> for additional insights and practical examples.

# Other IP Geolocation Solutions

\- [IP2Location.io IP Geolocation API](https://www.ip2location.io)

\- [IP2Location LITE IP-ASN Database](https://lite.ip2location.com/database-asn)

\- [IP2WHOIS WHOIS Domain Lookup](https://www.ip2whois.com/)

# About IP2Location

IP2Location.com offers extensive databases for IP geolocation. It enables users to precisely identify the geographical location of IP addresses, providing details such as country, region, city, district, latitude, longitude, ZIP code, time zone, connection speed, ISP, domain name, IDD country code, area code, weather station code and name, mobile carrier, elevation, usage type, address type, advertising category, and autonomous system.

These databases are invaluable for various use cases and applications, including website traffic analysis, fraud prevention, and personalized content delivery. By leveraging IP2Location’s data, businesses and developers can enhance their services, improve user experiences, and ensure more secure online interactions. IP2Location solution is available as a database and hosted API. If you are interested in web service instead of database, please visit [IP2Location.io](https://www.ip2location.io) for the remote hosted service.

Stay connected with us on [Facebook](https://www.facebook.com/ip2location), [X](https://x.com/ip2location) and [LinkedIn](https://www.linkedin.com/company/ip2location) for more insights into IP address data and its powerful applications.
