# IP2Proxy Sample Databases

IP2Proxy helps identify IP addresses linked to anonymous proxy services such as VPN servers, open proxies, web proxies, Tor exits, search engine robots, data center ranges, residential proxies, consumer privacy networks, enterprise private networks and more.

It reveals valuable attributes including: Residential Proxy, Proxy Type, Fraud Score, Last Seen, Threat Type
Available in 12 different packages for different levels of detail. The commercial database is being updated daily to maintain accuracy and reliability.

Use cases include:

- Security & Fraud Prevention
  - Prevent account abuse
  - Detect suspicious logins
  - Reduce bot traffic
- Compliance & Licensing
  - Enforce geo-restrictions
  - Regulatory compliance
- Platform Integrity
  - Protect online communities
  - Prevent scraping and abuse
- Analytics Accuracy
  - Improve data quality
- Infrastructure Management
  - Firewall integration 

# Database Overview

## IPProxy Proxy Detection Database

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

\- [IP2Location IP Geolocation Database](https://www.ip2location.com/database/ip2location)

\- [IP2Location LITE IP-ASN Database](https://lite.ip2location.com/database-asn)

\- [IP2WHOIS WHOIS Domain Lookup](https://www.ip2whois.com/)

# About IP2Location

IP2Location.com offers extensive databases for IP geolocation. It enables users to precisely identify the geographical location of IP addresses, providing details such as country, region, city, district, latitude, longitude, ZIP code, time zone, connection speed, ISP, domain name, IDD country code, area code, weather station code and name, mobile carrier, elevation, usage type, address type, advertising category, and autonomous system.

These databases are invaluable for various use cases and applications, including website traffic analysis, fraud prevention, and personalized content delivery. By leveraging IP2Location’s data, businesses and developers can enhance their services, improve user experiences, and ensure more secure online interactions. IP2Location solution is available as a database and hosted API. If you are interested in web service instead of database, please visit [IP2Location.io](https://www.ip2location.io) for the remote hosted service.

Stay connected with us on [Facebook](https://www.facebook.com/ip2location), [X](https://x.com/ip2location) and [LinkedIn](https://www.linkedin.com/company/ip2location) for more insights into IP address data and its powerful applications.
