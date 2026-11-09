# 🔐 Wireshark SOC Analysis Labs

**Networkwalks Cybersecurity Internship – Batch B084**

## 📌 Project Overview

This repository documents my hands-on experience completing six Wireshark SOC analysis labs as part of the Networkwalks Cybersecurity Internship.

The project focuses on analysing network traffic, investigating suspicious activities, identifying potential security threats, and understanding how network protocols can be used during cybersecurity investigations.

Through these practical exercises, I gained experience using Wireshark to examine packet captures and investigate different types of network-based attacks.

## 🎯 Project Objectives

The main objectives of these practical labs were to:

- Understand network packet analysis and traffic inspection using Wireshark.
- Identify suspicious IP addresses, source ports, destination ports, and potential network attackers.
- Analyse TCP conversations and reconstruct communication using the Follow TCP Stream feature.
- Investigate HTTP requests, responses, and plain-text information transmitted across networks.
- Understand the security risks associated with transmitting login credentials over unencrypted connections.
- Examine FTP authentication traffic and identify failed and successful login attempts.
- Detect and investigate brute-force attacks through network traffic analysis.
- Analyse VoIP communication using SIP and RTP protocols.
- Understand voice codecs and how voice traffic can be examined during an investigation.
- Identify network security weaknesses and recommend appropriate countermeasures, including HTTPS and SRTP encryption.
- Develop practical skills in network traffic analysis, threat identification, and security investigation.


## 🛠️ Tools and Technologies Used

### 1. Tools
- **Wireshark:** Used to capture, inspect, filter, and analyse network traffic during the practical investigations.
- **PCAP Files:** Packet capture files used as the source of network traffic for the six lab exercises.

### 2. Network Protocols Analysed
- **TCP:** Examined network communication sessions and followed TCP streams to reconstruct conversations.
- **HTTP:** Investigated web traffic and examined information transmitted in plain text.
- **FTP:** Analysed file transfer traffic and authentication attempts.
- **SIP:** Examined VoIP call signalling and call setup.
- **RTP:** Investigated the transmission of voice data during VoIP communication.

### 3. Security Concepts Explored
- **HTTPS:** Studied as a secure alternative to unencrypted HTTP communication.
- **SRTP:** Explored as a security solution for encrypting VoIP audio traffic.
- **Network Traffic Analysis:** Applied packet inspection and protocol analysis to identify suspicious activities and potential security threats.

## 🔍 Practical Labs and Activities

I worked through six hands-on Wireshark labs, each focusing on a different aspect of network traffic analysis.

During the exercises, I examined captured network traffic, followed TCP streams, investigated different protocols, and looked for signs of suspicious activity.

Below are the six labs I completed and a brief description of what I did in each one.


## 🧪 Detailed Lab Activities

### Lab 1: Identify the Attacker's IP

**Screenshot Evidence:** [View Lab 1 Screenshots](screenshots/Wireshark-SOC-Labs/Lab-1-Identify-the-Attackers-IP/)

I started by examining a packet capture containing suspicious network activity. I checked the total number of packets, identified SYN packets and examined the source and destination IP addresses to determine which system was initiating the connections.

I then investigated TCP conversations, checked the ports being accessed and examined TCP flags to distinguish open ports from closed ones. From the analysis, I identified the attacker, the target system and the port-scanning activity taking place.

**Key finding:** Identified the attacker as `192.168.10.66`, the target as `192.168.10.20`, and recognised the activity as a port scan.

### Lab 2: Follow TCP Stream 1

**Screenshot Evidence:** [View Lab 2 Screenshots](screenshots/Wireshark-SOC-Labs/Lab-2-Follow-TCP-Stream-1/)

In this exercise, I investigated a captured TCP conversation using Wireshark's Follow TCP Stream feature. I examined the communication between the client and server to reconstruct the exchanged messages.

By following the stream, I was able to identify the client IP address, TCP stream number and communication details. I also examined the conversation to uncover information shared between the users, including a staff member's name and other internal details.

**Key finding:** Learned how to reconstruct TCP conversations and extract useful information from network communication.

### Lab 3: Follow TCP Stream, Part 2

**Screenshot Evidence:** [View Lab 3 Screenshots](screenshots/Wireshark-SOC-Labs/Lab-3-Follow-TCP-Stream-Part-2/)

This lab involved a deeper investigation of TCP communication. I used Follow TCP Stream to examine captured traffic and uncover information that was not immediately visible in the packet list.

I investigated a hidden webpage, examined an HTML comment, identified the relevant TCP stream and inspected HTTP responses. I also checked the traffic direction and HTTP status code to understand how the server responded to the client's request.

**Key finding:** Successfully identified a hidden staff webpage, examined its HTTP response and located a downloaded report within the captured traffic.

### Lab 4: HTTP Plain Text Credentials

**Screenshot Evidence:** [View Lab 4 Screenshots](screenshots/Wireshark-SOC-Labs/Lab-4-HTTP-Plain-Text-Credentials/)

For this lab, I examined HTTP traffic to investigate how login information can be exposed during network communication. I identified the HTTP protocol, located POST requests and examined the login page and authentication attempts.

I also inspected the packet details to understand how form data was transmitted. This helped me see why sending login credentials over an unencrypted HTTP connection creates a security risk.

**Key finding:** Identified exposed login information in HTTP traffic and understood why HTTPS should be used to protect sensitive credentials.

### Lab 5: Catch the Brute Force Attacker

**Screenshot Evidence:** [View Lab 5 Screenshots](screenshots/Wireshark-SOC-Labs/Lab-5-Catch-the-Brute-Force-Attacker/)

In this exercise, I investigated FTP traffic to identify a suspected brute-force attack. I examined the communication between the attacker and target system, identified the username being targeted and checked the FTP response codes.

I distinguished failed login attempts from successful authentication and counted the repeated failures. This helped me understand how brute-force activity can be detected by analysing authentication patterns in network traffic.

**Key finding:** Identified 24 failed login attempts, recognised FTP response codes `530` and `230`, and confirmed the activity as a brute-force attack.

### Lab 6: Catch the Call Scammer (VoIP Call Replay)

**Screenshot Evidence:** [View Lab 6 Screenshots](screenshots/Wireshark-SOC-Labs/Lab-6-Catch-the-Call-Scammer/)

In the final lab, I investigated captured VoIP traffic to understand how an insecure phone conversation could expose sensitive information. I examined SIP packets to understand the call setup process and RTP packets to investigate the voice communication.

I also identified the caller's extension, examined the caller information and checked the audio codec used during the call. By investigating the call and listening to the recorded audio, I was able to determine who answered it. The exercise also demonstrated the risks of transmitting sensitive information over unencrypted voice communication.

**Key finding:** Identified SIP and RTP traffic, recognised the PCMU audio codec and learned why Secure Real-time Transport Protocol (SRTP) is important for protecting VoIP calls.




## 🎓 Skills and Knowledge Gained

Completing these labs helped me develop practical skills in:

- Network packet inspection and traffic analysis using Wireshark.
- Identifying suspicious IP addresses, ports and network activities.
- Reconstructing TCP conversations using Follow TCP Stream.
- Investigating HTTP requests and exposed credentials.
- Recognising FTP brute-force attacks through authentication patterns.
- Analysing VoIP communication using SIP and RTP.
- Understanding network security risks and appropriate security measures.

These exercises improved my understanding of how network traffic can be investigated to detect and analyse potential security threats.



## 🏆 Project Results and Completion

**Completion Evidence:** [View All Six Lab Results](screenshots/Wireshark-SOC-Labs/Lab-Completion-Results/)

I successfully completed all six Wireshark SOC analysis labs, covering a total of 60 practical tasks.

**Final Results:**
- Labs Completed: 6/6
- Tasks Completed: 60/60
- Total Score: 600/600
- Overall Performance: 100%

Completing these exercises gave me valuable hands-on experience in network traffic analysis, attack investigation and identifying security weaknesses using Wireshark.


## 📝 Conclusion

Completing these six Wireshark labs was a valuable learning experience. I had the opportunity to work with real packet analysis scenarios, investigate different types of network activity and understand how security threats can be identified through network traffic.

This project has strengthened my practical understanding of network analysis and motivated me to continue developing my skills in cybersecurity and security operations.
