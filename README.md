<h1>Analyze Network Traffic with TCPDump</h1>

<h2>Description</h2>
Project consists of using tcpdump to capture TCP packets from websites, and analyzing the captured packets with Wireshark.
<br />


<h2>Languages and Utilities Used</h2>

- <b>Linux</b>
- <b>Shell</b>
- <b>Wireshark</b>

<h2>Environments Used </h2>

- <b>Windows 10</b> (21H2)

<h2>Dump File Creation(1/3):</h2>
<br />
<p align="center">
Launch the utility and create Linux Shell file: <br/>
<img src="https://i.imgur.com/oISub0o.jpg" height="80%" width="80%" alt="Shell"/>
<br />
<br />
Execute TCP script to capture 10 packets from skyroute66.com:  <br/>
<img src="https://i.imgur.com/hHdysMY.jpg" height="80%" width="80%" alt="10 Packets"/>
<br />
<br />
After visting skyroute66.com: <br/>
<img src="https://i.imgur.com/9eNOcZg.jpg" height="80%" width="80%" alt="Skyroute66"/>
<br />
<br />
Create Dump file:  <br/>
<img src="https://i.imgur.com/JenTeSt.jpg" height="80%" width="80%" alt="Dump file"/>
<br />
<br />
Make the Dump file readable:  <br/>
<img src="https://i.imgur.com/J9gHHAd.jpg" height="80%" width="80%" alt="readable dump"/>
<br />
<br />
Execute the file again, but with -#XXtttt. Then open Wireshark to look at the packet:  <br/>
<img src="https://i.imgur.com/6doVJvS.jpg" height="80%" width="80%" alt="wireshark"/>
<br />
<br />
 <h2>Creating Dump Files with Limits(2/3):</h2>
<br />
<br />
<p align="center">
Creating packets that when exceeds 1 million bytes, it should create a new file:  <br/>
<img src="https://i.imgur.com/dmpm8sJ.jpg" height="80%" width="80%" alt="Bytes"/>
<br />
<br />
Using ls -al to show file size:  <br/>
<img src="https://i.imgur.com/V7k5nMd.jpg" height="80%" width="80%" alt="ls -al"/>
<br />
<br />
 This will create a new file if the packet exceeds 1 million bytes or after 10 minutes:  <br/>
<img src="https://i.imgur.com/9I1Xiy8.jpg" height="80%" width="80%" alt="Size and Time"/>
<br />
<br />
 <h2>Capture TCP traffic for GET (3/3):</h2>
<br />
<br />
<p align="center">
Execute, then find a website with a GET operation:  <br/>
<img src="https://i.imgur.com/3djiEHH.jpg" height="80%" width="80%" alt="GET"/>
<br />
<br />
Execute it into a file:  <br/>
<img src="https://i.imgur.com/ejXL4OD.jpg" height="80%" width="80%" alt="GET"/>
<br />
<br />
Open Wireshark and find GET:  <br/>
<img src="https://i.imgur.com/xYuriKH.jpg" height="80%" width="80%" alt="GET"/>
</p>


<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
