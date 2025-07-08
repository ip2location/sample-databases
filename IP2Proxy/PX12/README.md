# IP2PROXY PX12 - Proxy Detection Database

## IP-ProxyType-Country-Region-City-ISP-Domain-UsageType-ASN-LastSeen-Threat-Residential-Provider-FraudScore Database

[IP2Proxy PX12 Database](https://www.ip2location.com/database/px12-ip-proxytype-country-region-city-isp-domain-usagetype-asn-lastseen-threat-residential-provider-fraudscore) provides proxy data like proxy type, country, region or state, city, Internet Service Provider (ISP), domain, usage type, ASN, last seen, threat, residential, provider and fraud score of IP address.

This repository provides a sample version of the IP2Proxy PX12 database in CSV, BIN, and CIDR formats. The sample includes a limited number of data rows and is not updated regularly. It is intended solely for evaluation and testing purposes—not for use in production environments. 

For complete, high-accuracy data with up to daily updates, please subscribe to the commercial IP2Proxy PX12 database.

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
| provider | VARCHAR(256) | Name of [VPN provider](https://www.ip2location.com/vpn-provider-coverage) if available. |
| fraud_score | INT(10) | Potential risk score (0 - 99) associated with IP address. A higher IP2Proxy Fraud Score indicates a greater likelihood of fraudulent activity and a lower reputation. |

IP addresses are stored as 32-bit or 128-bit unsigned integers (depending on IPv4 or IPv6) and must be converted to standard IP notation for readability.

## Sample Rows in CSV Format
```csv
"27956963","27956963","RES","TW","Taiwan (Province of China)","Yunlin","Douliu","Chunghwa Telecom Co. Ltd.","cht.com.tw","ISP/MOB","3462","Asia Pacific Network Information Centre","19","-","-","42"
"37504603","37504603","RES","RU","Russian Federation","Omskaya oblast'","Omsk","OJSC Sibirtelecom","sibirtelecom.ru","ISP","12389","PJSC Rostelecom","29","-","-","32"
"47893732","47893732","RES","GB","United Kingdom of Great Britain and Northern Ireland","England","London","SKY UK Limited","sky.com","ISP/MOB","5607","SKY UK Limited","19","-","-","42"
"51850166","51850418","DCH","US","United States of America","Ohio","Columbus","Amazon Technologies Inc.","amazon.com","DCH","16509","Amazon.com Inc.","1","-","-","3"
"58531587","58531587","PUB","DE","Germany","Hessen","Frankfurt am Main","A100 ROW GmbH","amazon.com","DCH","16509","Amazon.com Inc.","30","-","-","80"
"59883433","59883433","SES","US","United States of America","Ohio","Columbus","Amazon Technologies Inc.","amazon.com","SES","16509","Amazon.com Inc.","1","-","-","1"
"68033847","68033848","DCH","US","United States of America","Tennessee","Nashville","Level 3 Communications Inc.","level3.com","DCH","3356","Level 3 Parent LLC","1","-","-","3"
"71573047","71573047","DCH","IT","Italy","Lombardia","Milan","Level 3 Communications Ltd","level3.com","DCH","3356","Level 3 Parent LLC","1","-","-","3"
"84802181","84802181","RES","RO","Romania","Vrancea","Focsani","RCS & RDS S.A.","rcs-rds.ro","ISP/MOB","8708","Digi Romania S.A.","1","-","-","60"
"86813962","86813963","RES","RU","Russian Federation","Kemerovskaya oblast'","Novokuznetsk","Norilsk-Telecom JSC","norcom.ru","ISP","40995","Sibirskie Seti Ltd.","16","-","-","45"
"89168363","89168363","RES","GB","United Kingdom of Great Britain and Northern Ireland","England","Leicester","British Telecommunications Plc","bt.com","ISP/MOB","2856","British Telecommunications Plc","23","-","-","38"
"93505012","93505012","RES","DE","Germany","Nordrhein-Westfalen","Hassels","Vodafone West GmbH","unitymedia.de","ISP","3209","Vodafone GmbH","25","-","Webshare","36"
"95691264","95691268","DCH","NL","Netherlands (Kingdom of the)","Limburg","Maastricht","Scheggia Services","cyberassets.ae","DCH","215026","Alessandro Accorsi Trading As Len Service Srl","1","-","-","3"
"98858900","98858900","PUB","RU","Russian Federation","Moskva","Moscow","NCN BBCUST","rt.ru","DCH","42610","PJSC Rostelecom","30","-","-","80"
"143918272","143918272","DCH","CN","China","Zhejiang","Hangzhou","Alibaba Cloud (Singapore) Private Limited","alicloud.com","DCH","37963","Hangzhou Alibaba Advertising Co. Ltd.","17","SCANNER","-","62"
```

## Downloadable File Formats

- CSV: Comma-delimited text file with decimal ranges for direct database import or manual inspection.

- BIN: IP2Location binary format for use with official IP2Location or IP2Proxy libraries.

- CIDR: Comma-delimited text file with CIDR ranges, useful for firewall rules, network scanning, log analysis, and infrastructure automation.

## Sample Databases

| Format       | IPv4 Address                                                                                                        | IPv6 Address                                                                                                        |
|--------------|--------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------|
| **CSV**      | [Download Sample](https://github.com/ip2location/sample-databases/tree/main/IP2Proxy/PX12/ip2proxy-px12-sample.ipv4.csv) | [Download Sample](https://github.com/ip2location/sample-databases/tree/main/IP2Proxy/PX12/ip2proxy-px12-sample.ipv6.csv) |
| **BIN**      | [Download Sample](https://github.com/ip2location/sample-databases/tree/main/IP2Proxy/PX12/ip2proxy-px12-sample.ipv4.bin) | [Download Sample](https://github.com/ip2location/sample-databases/tree/main/IP2Proxy/PX12/ip2proxy-px12-sample.ipv6.bin) |


# Usage

### CSV File for Database Query

For details on importing the CSV file into a database and using SQL statements for IP lookup, please visit [](https://xxxxx)<https://www.ip2location.com/documentation/ip2proxy-database-px12#codes>

### BIN File for IP Lookup

To perform IP lookups with the BIN file, you’ll need to use the IP2Proxy SDK. Refer to the [development libraries](https://www.ip2location.com/development-libraries/?tab=ip2proxy) for usage instructions and integration guides.

# License

This sample data is provided by IP2Location.com for evaluation purposes. Please refer to the [licensing page](https://www.ip2location.com/licensing) for production licensing and usage.

# Useful Guides & Resources

For more information, please refer to the IP2Location.com official documentation at <https://www.ip2location.com/documentation/ip2proxy-database-px12>, which provides comprehensive details and usage guidelines.

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
