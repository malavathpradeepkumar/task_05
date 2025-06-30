I have included my packet capture file for this project, which you can download from the following link:

https://drive.google.com/file/d/1K6kVna3OrC47tAHDL5PlHtE9nvh_hiza/view?usp=sharing

This .pcap file contains the network traffic I captured during the practical part of my project, including DNS, HTTP, ICMP, and other packets. It can be opened using Wireshark to see the captured packets, filter them by protocol, and verify the analysis described in my report.

For my project, I performed a packet capture and analysis using Wireshark on Kali Linux. First, I updated my system and installed Wireshark by running the commands 
sudo apt update and sudo apt install wireshark -y. To allow my user to capture packets without root, I added my user to the wireshark group using sudo usermod -aG 
wireshark $USER and then confirmed the installation with wireshark --version. After installation, I launched Wireshark by typing wireshark in the terminal. In the 
Wireshark interface, I selected my active network interface, which was either wlan0 or eth0, and started capturing live network traffic. While the capture was running, 
I generated traffic by opening a web browser and visiting sites like kali.org and debian.org, and I also used the command ping -c 4 google.com to create ICMP packets. 
After about a minute, I stopped the capture by clicking the red stop button and saved the captured packets as capture1.pcap. Then, I explored the capture by applying 
protocol filters in Wireshark, such as dns, http, icmp, and tcp, to view packets related to specific network protocols. I also exported filtered packets to separate 
pcap files like dns_traffic.pcap for better analysis and documentation. To create my report, I reviewed the total number of packets captured, counted how many belonged 
to each protocol, and captured screenshots of the main Wireshark window and the protocol hierarchy statistics. Through this process, I learned how to capture real network 
traffic, analyze it by protocol, and document my 
findings effectively using Wireshark.
