# SWYNEX Network Security Analysis

A hands-on network traffic analysis project completed as part of the SWYNEX internship tasks. This project uses Wireshark and TShark in a controlled Kali Linux lab to inspect network protocols, understand communication patterns, and document potential security concerns.

## Objectives

- Analyse network traffic using Wireshark.
- Identify ICMP, DNS, TCP, HTTP, and TLS protocols.
- Inspect TCP connection establishment and HTTP request-response behaviour.
- Review HTTP response headers and potential security considerations.
- Document findings, evidence, and defensive recommendations.

## Tools and Technologies

- **Operating System:** Kali Linux
- **Packet Analysis:** Wireshark, TShark
- **Traffic Generation:** ping, nslookup, curl
- **Lab Environment:** VMware Workstation
- **Test Application:** OWASP Juice Shop (local lab)

## Project Structure

```text
SWYNEX-Network-Security-Analysis/
├── README.md
├── network-security-analysis.md
├── evidence/
│   ├── 01-icmp-loopback.png
│   ├── 02-dns-query-response.png
│   ├── 03-https-tls-analysis.png
│   ├── 04-http-request-response.png
│   ├── 05-http-response-headers.png
│   └── 06-tcp-syn-analysis.png
└── captures/
    ├── https-tls-baseline.pcapng
    ├── dns-traffic.pcapng
    └── local-http-analysis.pcapng
```

## Analysis Performed

| Area | Analysis |
|---|---|
| ICMP | Observed loopback echo requests and replies |
| DNS | Inspected DNS queries and responses |
| HTTPS/TLS | Examined TCP port 443 traffic and TLS handshake packets |
| HTTP | Inspected a local HTTP HEAD request and server response |
| HTTP headers | Reviewed response headers and their security implications |
| TCP | Examined a SYN packet used to initiate a TCP connection |

## Key Learnings

- Understanding packet capture and display filters.
- Identifying source and destination IP addresses, ports, and protocols.
- Interpreting DNS queries, TCP connection attempts, and TLS traffic.
- Inspecting HTTP response status codes and security headers.
- Distinguishing normal network behaviour from potential security concerns.
- Preserving packet captures and screenshots as technical evidence.

## Security Considerations

The analysis highlighted the importance of encrypted communication, appropriate CORS configuration, secure HTTP response headers, and contextual network monitoring.

The observations are educational and defensive. No confirmed exploitable vulnerability or malicious activity was established solely from these captures.

## Evidence and Report

- **Detailed report:** [`network-security-analysis.md`](network-security-analysis.md)
- **Screenshots:** [`evidence/`](evidence/)
- **Packet captures:** [`captures/`](captures/)

The PCAPNG files can be opened in Wireshark for further inspection.

## Scope and Disclaimer

All analysis was conducted in a controlled personal lab using locally generated or otherwise authorized traffic. This project is intended for educational and defensive cybersecurity purposes only.

## Acknowledgement

Completed as part of the **SWYNEX Technologies internship task series**.

#CyberSecurity #NetworkSecurity #Wireshark #KaliLinux #PacketAnalysis #SWYNEX #Internship