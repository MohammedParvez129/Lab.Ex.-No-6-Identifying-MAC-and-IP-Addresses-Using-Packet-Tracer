# Ex. No: 6 Identifying MAC and IP Addresses Using Packet Tracer
# Date: 13-09-2025
________________________________________
# Objective
To use Cisco Packet Tracer simulation mode to capture and analyze MAC and IP address information for both local and remote network communication.
________________________________________
# Apparatus/Tools Required
•	Cisco Packet Tracer<br>
•	Pre-configured network topology (as provided in the activity file)<br>
•	PCs, switches, router, hub, and wireless access point (as per given setup)<br>
________________________________________
# Network Topology Diagram
# Description:
•	The topology contains a local network (172.16.31.0/24) connected to a remote network (10.10.10.0/24) via a router.<br>
•	Devices include PCs, switches, hub, and wireless AP.<br>
(Insert screenshot of your Packet Tracer setup here)<br>
________________________________________
# IP Addressing Table
(Example – actual values from simulation)<br>
Device	IPv4 Address	Subnet Mask	MAC Address<br>
PC-A	172.16.31.5	255.255.255.0	00D0:D311:C788<br>
PC-B	172.16.31.2	255.255.255.0	000C:85CC:1DA7<br>
Router (G0/0)	172.16.31.1	255.255.255.0	00D0:BA8E:741A<br>
PC-Remote	10.10.10.2	255.255.255.0	00D0:588C:2401<br>
________________________________________
# Procedure
# Part 1: Local Network Communication
1.	Click PC-A (172.16.31.5) and open the Command Prompt.<br>
2.	Enter ping 172.16.31.2.<br>
3.	Switch to Simulation Mode and repeat the ping.<br>
4.	When the PDU appears, click it and record: Destination MAC, Source MAC, Source IP, Destination IP, and the device name.<br>
5.	Use Capture/Forward to follow the PDU through the network until it reaches PC-B.<br>
6.	Record the information in a table.<br>
7.	Repeat the above process for:<br>
o	Ping from 172.16.31.3 to 172.16.31.2<br>
o	Ping from 172.16.31.5 to 172.16.31.4<br>
Part 2: Remote Network Communication<br>
1.	From PC-A (172.16.31.5), enter ping 10.10.10.2.<br>
2.	Switch to Simulation Mode and repeat the ping.<br>
3.	When the PDU appears, note the Destination MAC, Source MAC, Source IP, and Destination IP.<br>
4.	Follow the PDU step-by-step until it reaches the remote PC.<br>
5.	Observe how MAC addresses change at the router while IP addresses remain constant end-to-end.<br>
________________________________________
# Example Data Recording Table
At Device	Dest. MAC	Src MAC	Src IPv4	Dest IPv4<br>
172.16.31.5	000C:85CC:1DA7	00D0:D311:C788	172.16.31.5	172.16.31.2<br>
Switch1	000C:85CC:1DA7	00D0:D311:C788	N/A	N/A<br>
172.16.31.2	00D0:D311:C788	000C:85CC:1DA7	172.16.31.2	172.16.31.5<br>
________________________________________
# Output (Screenshots)
•	PDU details for local communication<br>
<img width="1920" height="1080" alt="Screenshot 2025-09-13 141808" src="https://github.com/user-attachments/assets/e2d95ecd-345a-43c4-9041-3afa991d7343" />
<img width="1920" height="1080" alt="Screenshot 2025-09-13 141712" src="https://github.com/user-attachments/assets/4208635d-8b3b-4800-bea7-cb6b9e1068de" />
<img width="1920" height="1080" alt="Screenshot 2025-09-13 141620" src="https://github.com/user-attachments/assets/b07c6fe5-81c6-4cb6-90e1-b90ba4515f35" />
<img width="1920" height="1080" alt="Screenshot 2025-09-13 141417" src="https://github.com/user-attachments/assets/c4e990a1-1058-408c-9269-cb0a87fc0116" />



•	PDU details for remote communication<br>
<img width="1920" height="1080" alt="Screenshot 2025-09-13 144047" src="https://github.com/user-attachments/assets/32cb3b36-63b0-4c16-a6c8-99deabfebd0b" />
<img width="1920" height="1080" alt="Screenshot 2025-09-13 144011" src="https://github.com/user-attachments/assets/cb4c88fb-ff42-4d38-9dde-4868ca824fea" />
<img width="1920" height="1080" alt="Screenshot 2025-09-13 143934" src="https://github.com/user-attachments/assets/5a36660d-e0bc-4c84-82f5-afb39b6a068f" />
<img width="1920" height="1080" alt="Screenshot 2025-09-13 144345" src="https://github.com/user-attachments/assets/d98c44ca-018a-4ac0-b6b4-230c3ffbfe6e" />
<img width="1920" height="1080" alt="Screenshot 2025-09-13 144214" src="https://github.com/user-attachments/assets/74f8cfe3-b101-4c1b-9ba2-bb7773c5912e" />
<img width="1920" height="1080" alt="Screenshot 2025-09-13 144156" src="https://github.com/user-attachments/assets/1fa11d1b-824e-4176-a8a1-3d58bccc18c0" />



•	Tables showing MAC/IP changes through each device<br>
<img width="1920" height="1080" alt="Screenshot 2025-09-13 144820" src="https://github.com/user-attachments/assets/307d7d21-5df7-47ef-8468-76971ac72b6a" />
<img width="1920" height="1080" alt="Screenshot 2025-09-13 144740" src="https://github.com/user-attachments/assets/75f91671-9be1-4ef9-83e7-ca6976bc1cf3" />

________________________________________
# Result
Successfully captured and analyzed MAC and IP addresses for both local and remote communications. Verified that MAC addresses change at each hop while IP addresses remain constant from source to destination.

