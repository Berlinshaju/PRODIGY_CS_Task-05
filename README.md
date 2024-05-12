# PRODIGY_CS_Task-05

# Network Traffic Analysis Report

__Objective:__ Analyze network traffic using tcpdump and Wireshark.

# 1. Capture Network Traffic:
```
tcpdump -i eth0 -vv dst 192.168.1.7 and port http -w http.txt
```
__tcpdump__: Command-line packet analyzer.
__-i eth0__: Specifies the network interface for capturing packets.
__-vv__: Increases verbosity for detailed output.
__dst 192.168.1.7__: Captures packets with destination IP address 192.168.1.7.
__port http__: Filters packets by HTTP port (port 80 by default).
__-w http.txt__: Writes captured packets to http.txt file.


# 2. Analyze Captured Traffic:
```
wireshark http.txt
```
__wireshark__: Graphical packet analyzer.

__http.txt__: Packet capture file to be analyzed.

# 3. View Packet Capture Details:
```
tcpdump -r http.txt
```
__tcpdump__: Command-line packet analyzer.

__-r http.txt__: Reads and displays contents of http.txt packet capture file.

# Summary:
The tcpdump command was used to capture network traffic destined for IP address __192.168.1.7__ on interface __eth0__, specifically targeting HTTP traffic.
The captured packets were written to a file named http.txt for further analysis.
Wireshark was utilized to visually analyze the captured packets, allowing for in-depth inspection of protocols, packet contents, and network behavior.
Additionally, tcpdump was used to display packet capture details directly in the terminal window.

# Conclusion:
The combination of tcpdump and Wireshark provides comprehensive tools for network traffic analysis, facilitating the identification of network issues, security threats, and protocol anomalies.


![Metasploitable2-Linux - VMware Workstation 5_12_2024 12_29_33 PM](https://github.com/Berlinshaju/PRODIGY_CS_Task-05/assets/66897078/2ca92f48-3bf4-4763-81eb-1d0ce5e95e97)


