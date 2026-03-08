# SOC-ANALYSIS
## Overview
This project stimulates a cyber attack scenerio and demonstrates detection and prevention using:
- Wireshark
- Pfsense
- Snort(IDS/IPS)
- Wazuh (SIEM and Monitoring)

## Objectives
- Stimulate attack (Http beaconing, DNS beaconing and bruteforce attack)
- Detect Anomally (Wireshark)
- Creating a firewall (PFSENSE)
- Block Malicious IP
- Monitor logs with Wazuh

  ## Tools Used
- Pfsense
- Wazuh
- Snort
- Kali
- Ubuntu
- Wireshark

  ## Project Architecture
  The SOC monitoring environment consist of:
   **Wireshark** - Packet capture and traffic analysis
  **pfSense** - Firewall configurationand geo-blocking
  **Snort IDS/IPS** - Intrusion detection and rule-based blocking
  **Wazuh SIEM** - Centralized logging and monitoring

                    Attacker (Kali Linux)
                            │
                            ▼
                    Network Traffic
                            │
                            ▼
                    Wireshark Analysis
                            │
                            ▼
                    pfSense Firewall + Snort IDS
                            │
                            ▼
                    Wazuh SIEM Monitoring

  ## Phase 1: Network Analysis with Wireshark
  Wireshark was used to capture and analyse network traffic in order to detect anomalies reported by theorganization.
  The analysis focused on detecting:
  - DNS beaconing
  - HTTP command and control communication
  - SSH brute force attacks

 **HTTP Beaconing Detection**
   - Suspicious HTTP request such as /http_better
   - Repeated communication withunknown IP: 192.168.0.94
   - continous GET and POST requests from the same IP
   - Lond and encoded parameters
   - Access to multiple suspicious JavaScrript payloads
     
**Screenshot**
 

  

- 
