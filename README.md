# Mirai Malware

## Overview
Mirai is a type of malware that targets Internet of Things (IoT) devices—such as routers, IP cameras, and DVRs—to create a large botnet capable of launching powerful distributed denial-of-service (DDoS) attacks.

## History
- **First Discovered:** August 2016  
- **Authors:** Originally developed by a group of hackers using the handles “Anna-senpai,” “t0xic,” and “vamp,” later open-sourced on Hack Forums.  
- **Notable Attacks:**  
  - **KrebsOnSecurity DDoS (September 2016):** Peaked at ~620 Gbps.  
  - **Dyn DNS Attack (October 2016):** Disrupted major websites (e.g., Twitter, Netflix, Reddit).

## Infection Mechanism
1. **Scanning:** Mirai continuously scans the public internet for devices listening on Telnet ports (23/2323).
2. **Brute-Force Login:** It attempts to log in using a built-in list of common default credentials.
3. **Payload Deployment:** Once a device is compromised, Mirai deploys its payload, adding the device to its botnet.
4. **Command & Control (C&C):** Infected devices connect back to C&C servers to receive instructions (e.g., target IPs for DDoS).

## Botnet Capabilities
- **DDoS Attacks:** UDP floods, TCP SYN floods, HTTP GET floods, GRE packets.
- **Scale:** At its height, Mirai controlled hundreds of thousands of devices.
- **Modularity:** Open-source release allowed rapid creation of Mirai variants (e.g., “Okiru,” “Satori”).

## Impact
- **Internet Disruption:** Major outages of high-profile services.
- **Economic Cost:** Millions of dollars in mitigation and recovery.
- **Security Awareness:** Highlighted the risks of insecure IoT devices and the need for strong credential practices.

## Mitigation & Prevention
- **Change Default Credentials:** Use unique, strong usernames and passwords.
- **Firmware Updates:** Apply patches to IoT devices regularly.
- **Network Segmentation:** Isolate IoT devices on separate VLANs.
- **Rate Limiting & Filtering:** Deploy upstream DDoS protection and ingress/egress filters.

## Evolution & Legacy
Because the Mirai source code was publicly released, it spawned numerous variants, each adapting to new device types and vulnerabilities. Security vendors and device manufacturers have since prioritized better out-of-the-box security for IoT, but the threat remains a cautionary example of how simple, automated attacks can leverage massive numbers of devices.

---

*Mirai’s rise underscored the critical importance of securing IoT ecosystems and has informed both industry standards and best practices in network defense.*  
