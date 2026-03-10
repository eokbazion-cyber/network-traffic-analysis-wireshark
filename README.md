# Network Traffic Analysis with Wireshark

## Objective
Analyze live network traffic to understand DNS resolution, TCP handshake, and TLS encryption during website access.

## Tools Used
- Wireshark (macOS)
- Safari Browser

## Methodology
- Captured live traffic on Wi-Fi interface (en0)
- Visited google.com to generate network activity
- Applied display filters:
  - `dns`
  - `tcp.flags.syn == 1`
  - `tls`

## Observations

### DNS Resolution
Observed DNS queries resolving google.com to its corresponding IP address.

### TCP Handshake
Identified the TCP three-way handshake:
SYN → SYN/ACK → ACK

### TLS Encryption
Observed TLS negotiation including:
- Client Hello
- Server Hello
- Change Cipher Spec
- Encrypted Application Data

Confirmed encrypted communication over secure ports.

## Key Takeaways
- Gained understanding of how client-server communication is established.
- Observed how HTTPS encrypts traffic in transit.
- Strengthened foundational knowledge relevant to SOC monitoring and network traffic analysis.

