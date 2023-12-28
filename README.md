<h1>Wireless Forensics Investigation Project</h1>

<h2>Description</h2>
<br>The scope of this project consists of the process and tools that have been well-tested and documented on the internet, no new or untested tools or processes were used in this report.<br />


<h2>Languages and Utilities Used</h2>

- <b>Cisco CMD</b> 
- <b>Command Prompt</b>

<h2>Environments Used </h2>

- <b>Cisco Packet Tracer</b>
- <b>Wireshark</b>

<h2>Project Body</h2>

<p align="center">
Figure 1 Wireless Network Architecture: <br/>
<img src="https://i.imgur.com/TQhOKYh.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br>
  <p>  In Figure 1 we are shown a network that is using WPA2-PSK in its wireless access points to connect to end devices. There are a number of risks that can be found when using this type of security, that being said this report will focus on the use of Key Reinstallation Attacks (KRACK). This type of attack targets the four-way handshake process that establishes encryption keys between a client device and an access point. The four-way handshake is an integral part of the WPA2 authentication, it is meant to protect against replay attacks. KRACK is used to exploit weaknesses in this process, the attacker will then be able to manipulate and replay certain steps of the handshake to force devices to reinstall a key that has already been used. With the attacker able to intercept and replay specific frames exchanged during the handshake they will be able to potentially decrypt packets, inject malicious content, or forge packets within the Wi-Fi network.
</p>
<p>  The need for a search warrant regarding the on-site examination of devices and any wireless-related equipment is of utmost importance. A search warrant is a legal authorization issued by a court that allows law enforcement or authorized individuals to conduct searches of specified locations or seize specific items. A search warrant is needed to protect individuals' 4th Amendment Rights against unreasonable searches and seizures. If evidence is collected without a search warrant its credibility in a court of law is slim to none unless there are other circumstances. In regards to the on-site examination of devices a search warrant can be very specific as to what investigators can look into, such as a computer investigators may only have access to certain drives and not the entire computer.
</p>
<p>It is important to stay within the scope of the warrant because collecting data that was not permitted by the courts could result in all of the data collected losing its credibility. Wireless-related equipment search warrants would simply include the devices that were used in the implementation of the wireless data. That would include but not be limited to routers, switches, access points, computers, mobile devices, or any equipment related to the wireless network setup. This would allow investigators to collect digital evidence, logs, configurations, and data pertinent to the investigation while respecting privacy rights and legal constraints.
</p>
<p>The process of identifying the wireless devices connected to the network would first be done by getting access to the network. The next step would be to examine all of the assigned IP addresses on the network these can be found in the DHCP logs. The next step would be to Log into the administrative interface of each WAP(Wireless Access Point) in the network. Within the WAP's administrative interface, check for information related to connected devices this information lists devices associated with each access point, providing their MAC and IP addresses. Wireshark can then be used to capture packets on the network to provide a view of devices communicating on the network. The implementation of Wireless Intrusion Detection Systems across the network helps in monitoring and identifying unauthorized devices on the network. Finally, the use of active network monitoring tools can be used to scan and detect devices connecting to the network in real-time. This will allow for monitoring of the network to help in identifying any new or unrecognized devices that join the network.
</p>
<p>The process of documenting the scene includes assessing and documenting the physical environment where evidence is located. The investigator will then need to take comprehensive photographs or videos of the scene from multiple angles. The next step in the process would be to create a sketch or diagram illustrating the layout of the area. The final step in the process will be to prepare written notes describing the scene, this will include documenting the date, time, location, and individuals present as well as including details about observed conditions or anything out of the ordinary.
</p>
<p>The chain of custody is important to maintain the integrity of the evidence collected, the document will need to include the initial seizure or collection of evidence, including information like item description, location, time, and individual handling the evidence. The document should be in secure packaging which is tamper-evident containers or bags. Each transfer or handling of the evidence should be recorded with the details of who handled it, the purpose, date, time, and any relevant actions taken. The evidence should be stored in a secure location with restricted access, ensuring it's protected from tampering, loss, or damage. Properly documenting the scene and maintaining a Chain of Custody ensures the credibility and admissibility of evidence in legal proceedings. 
</p>
<p>There are different types of tools that are used for detecting wireless connections the use including Wireshark. It is a form of a packet sniffer detection tool that allows deep packet inspection, capturing and analyzing wireless traffic to identify devices, protocols, and data exchanges within a network. There are wireless network scanners such as NetSpot which Provides visual Wi-Fi mapping, signal analysis, and troubleshooting tools to identify wireless networks and their strengths. There are also processes that allow wireless intrusion detection including Snort which offers intrusion detection capabilities.
</p>
<p>Tools that can be used to determine the wireless field's strength vary with the different devices that they can be used on. On most mobile devices there are apps that can be used that provide real-time measurements of signal strength and signal quality. There are professional software such as NetSpot Pro which is a software designed for Wi-Fi analysis that provides heatmaps of signal coverage and strength within a specified area. Finally, there are built ways to test the wireless field strength of a network in operating systems, in windows using the command ‘netsh wlan show interfaces’ in the command prompt will display the strength as shown in Figure 2.
</p>
<p align="center">
Figure 2 Netsh: <br/>
<img src="https://i.imgur.com/L7AuKFL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<p>In terms of creating a static map of wireless zones and hotspots, it involves collecting and analyzing data from wireless connections to identify areas with varying signal strengths and coverage. The process of signal strength measuring can help to find this information, the program previously discussed NetSpot can also be used as a coverage mapping tool. The logging of the recorded signal strength measurements at various points, and noting the strength, and location coordinates all better provide an understanding of the area in the network. After collecting the heatmap of a network the data is used to create a heatmap or color-coded map representing signal strength variations across the surveyed area. Mapping the zones will consist of creating distinct boundaries or outlines to represent different zones within the map. 
</p>
<p>Network monitoring tools, sniffing tools, and other methods used to capture wireless traffic are essential in analyzing network behavior, identifying security threats, and troubleshooting issues. The tool Wireshark can be used to capture and analyze packets on a network, offering in-depth inspection of traffic, including wireless transmissions. Wireshark has the ability to capture packets across various protocols, allowing for detailed analysis. The tool Aircrack-ng can be used as a sniffer as it is primarily used for penetration testing and analyzing wireless security, it includes packet sniffing tools for capturing and analyzing Wi-Fi traffic. The Aircrack-ng tool also has the ability to perform WEP/WPA/WPA2 attacks and analyze wireless traffic for security vulnerabilities.
</p>
<p>There are a number of different wireless evidence types, packet captures are one of them which is capturing wireless network traffic containing packets, which can be analyzed for forensic investigation. Network logs are records of network activity, including connection logs, access point logs, and router logs, providing information on network interactions. Device configurations and logs from wireless devices like routers, switches, access points, or wireless-enabled devices can be valuable evidence in an investigation. Aircrack-ng is a wireless forensic software tool used for capturing and analyzing packets, cracking Wi-Fi encryption, and performing penetration tests on wireless networks. The packet analysis tool Wireshark is also a wireless forensic tool as it provides wireless network traffic for forensic analysis.
</p>
<p>There are also other tools that are used to examine wireless evidence such as Forensic Imaging Devices. This tool is designed for forensically sound imaging of wireless devices, capturing data without altering the original evidence. Another example of a tool to examine wireless evidence is a mobile forensic tool called Cellebrite UFED (Universal Forensic Extraction Device). Cellebrite UFED is a  comprehensive mobile forensic tool supporting extraction from a wide range of mobile devices, including smartphones, feature phones, and tablets. It allows logical and physical extraction of data, bypassing locks, decoding various file systems, and analyzing mobile device contents.
</p>
<h3>Works Cited</h3>
<p>Aircrack-ng.org, https://www.aircrack-ng.org/. Accessed 25 November 2023.
“Cellebrite UFED | Access and Collect Mobile Device Data.” Cellebrite, https://cellebrite.com/en/ufed/. Accessed 25 November 2023.
</p>
<p>Ghimiray, Deepan, and Step Guide. “Wi-Fi Security: WEP vs WPA or WPA2.” Avast, 7 January 2022, https://www.avast.com/c-wep-vs-wpa-or-wpa2. Accessed 25 November 2023.
</p>
<p>Hathaway, Annie. “Using Log Data as Forensic Evidence.” Rapid7, 12 August 2016, https://www.rapid7.com/blog/post/2016/08/12/using-log-data-as-forensic-evidence/. Accessed 25 November 2023.
</p>
<p>“Plan, survey, visualize & improve WiFi network with NetSpot.” NetSpot, https://www.netspotapp.com/features.html. Accessed 25 November 2023.
</p>
<p>“Wireshark · Documentation.” Wireshark, https://www.wireshark.org/docs/. Accessed 25 November 2023.
</p>
  <br />  
<br />
