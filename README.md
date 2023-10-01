# Inspecting-Network-Traffic 🕵️‍♂️ <p align="center">
<img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>Inspecting Traffic Between Azure Virtual Machines in Wireshark / SSH Remote Connection</h1>
In this tutorial, we observe various network traffic to and from Azure Virtual Machines with Wireshark as well as experiment with SSH(Secure Shell Protocol) to remotely connect to another terminal. <br />


<h2>Video Demonstration</h2>

- ### [YouTube: Azure Virtual Machines, Wireshark, and Network Security Groups]https://www.youtube.com/watch?v=lb1Dw0elw0Q&list=PLR0bgGon_WTK9PHDzrlje4bqEh3p0NxxX

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Observe Network Protocols (ICMP, RDH, DNS, HTTP/S, SSH)
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
<br />
 <p>
<img src="https://github.com/Klinsmannn/Inspecting-Network-Traffic/assets/146140975/ede0c315-d49f-484e-b289-7bacab3d009b">
</p>
<br />
<p>

Go into Azure and create your two virtual machines, one on windows and the other on linux. Remote desktop in to your windows VM by using Remote Desktop Connection and inserting the public ip address as shown. If using a MAC or some other OS then download the Windows app for remote desktop.
<p>
<br /> 
 <br />
 
</p>
<img src="https://github.com/Klinsmannn/Inspecting-Network-Traffic/assets/146140975/7d56ad88-9be9-444e-9452-e72111603e80">
<P>
 
</P>
Go to your browser and install Wireshark so we can monitor traffic
</p>
<br />

<img src="https://github.com/Klinsmannn/Inspecting-Network-Traffic/assets/146140975/cfc01424-3f5c-4f1f-93c4-c0de2b07a615">

<br />

<p>
Wireshark is an open source software that used to analyze traffic or packets of data in a Network. Hit the ethernet button and the bluefin button to start capturing data. To filter out what protocol your looking for type in the bar like DNS,ICMP,DHCP,SSH, etc.... You can also look for your traffic if you know the port number by typing in "tcp.port ==#"

<p>
</p>
 <img src="https://github.com/Klinsmannn/Inspecting-Network-Traffic/assets/146140975/65e6b494-070f-4533-9840-c1f23c765e3a">
  <img src="https://github.com/Klinsmannn/Inspecting-Network-Traffic/assets/146140975/cb8121f1-c724-4b69-8ab9-0074f3225f40">
</p>

<p>
Go into your Powershell command line or Command Prompt and ping the private ip address of the other VM. Ping is for checking the connectivity of a computer and its ip address.  You can check the ping in Wireshark by typing in ICMP in the bar.
</p>
<br />

<p>
<img src="https://github.com/Klinsmannn/Inspecting-Network-Traffic/assets/146140975/f5f6951c-0bb4-4908-b6f1-19890be5ae5b">
<img src="https://github.com/Klinsmannn/Inspecting-Network-Traffic/assets/146140975/e9310592-15f3-490f-abef-d128bb069c06">

</p>
Go into your CLI or Powershell prompt and type in "SSH" and the username of the computer you want to connect to along with the private ip address like so "SSH username@private ip address". When typing in password the letters wont show so make sure your typing in the password correctly. The new username will be highlighted if connected successfully.Type "exit" when your done with connection.
<p>
</p>
<br />
