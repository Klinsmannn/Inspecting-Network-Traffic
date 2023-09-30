# Inspecting-Network-Traffic 🕵️‍♂️ <p align="center">
<img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>Inspecting Traffic Between Azure Virtual Machines in Wireshark / SSH Remote Connection</h1>
In this tutorial, we observe various network traffic to and from Azure Virtual Machines with Wireshark as well as experiment with Network Security Groups. <br />


<h2>Video Demonstration</h2>

- ### [YouTube: Azure Virtual Machines, Wireshark, and Network Security Groups]https://www.youtube.com/watch?v=lb1Dw0elw0Q&list=PLR0bgGon_WTK9PHDzrlje4bqEh3p0NxxX

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Various Command-Line Tools
- Various Network Protocols (SSH, RDH, DNS, HTTP/S, ICMP)
- Wireshark (Protocol Analyzer) 🦈

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)
- Ubuntu Server 20.04

<h2>High-Level Steps</h2>

- Create Resources/VMs
- CLI/Powershell 
- Wireshark🦈
- SSH Connection

<h2>Actions and Observations</h2>

<p>
<img src="https://github.com/Klinsmannn/Inspecting-Network-Traffic/assets/146140975/ce339f10-28e2-4064-939e-9d5d5d9d27c3">

</p>
 <p>
<img src="https://github.com/Klinsmannn/Inspecting-Network-Traffic/assets/146140975/ede0c315-d49f-484e-b289-7bacab3d009b">

 </p>
<p>
<img src="https://github.com/Klinsmannn/Inspecting-Network-Traffic/assets/146140975/7d56ad88-9be9-444e-9452-e72111603e80">


</p>
<p>
Go into Azure and create your two virtual machines, one windows and the other linux. Remote desktop in to your windows VM by using Remote Desktop Connection and inserting the public ip address as shown. If using a MAC or some other OS then download the Windows app for remote desktop. Search for and install wireshark so we can monitor network traffic between VM's. 
</p>
<br />

<p>
<img src="https://github.com/Klinsmannn/Inspecting-Network-Traffic/assets/146140975/65e6b494-070f-4533-9840-c1f23c765e3a">
  <img src="https://github.com/Klinsmannn/Inspecting-Network-Traffic/assets/146140975/cb8121f1-c724-4b69-8ab9-0074f3225f40">

</p>
<p>
Go into your Powershell command line or Command Prompt and ping the private ip address of the other VM. Ping is for checking the connectivity of a computer and its ip address.  You can check the ping in Wireshark by typing in ICMP in the bar. You can also check other traffic like DNS,UDP, RDP, etc....
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
Go into your CLI or Powershell prompt and type in "SSH" and the username of the computer you want to connect to along with the private ip address like so "SSH username@private ip address". When typing in password the letters wont show so make sure your typing in the password correctly. The new username will be highlighted if connected successfully.Type "exit" when your done with connection.
<p>
</p>
<br />
