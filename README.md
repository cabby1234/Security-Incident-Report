# Security Incident Report
<h1>Hacking WPA/WPA2</h1>

<h2>Description</h2>
This project is a security incident report I completed while studying for my Google Cybersecurity Certificate. A incident was reported where there was a possible brute force attack used to compromise the admin account.
<br />

<h2>Lab walk-through:</h2>

<p align="center">
<strong>Step 1: Identify the network protocol involved in the incident.</strong>
 <br/>
The protocol impacted in the incident is the Hypertext transfer protocol (HTTP). Running tcpdump and accessing the yummyrecipesforme.com website to detect the problem and capture protocol and traffic activity in a DNS & HTTP traffic log file provided the evidence needed to conclude. The malicious file is observed being transported to the users’ computers using the HTTP protocol at the application layer.


<br>
<br>
 <br>
<strong>Perform our reconaissance on the target and capture the WPA handshake, deauthenticate if needed:</strong>
 <br>
<img align="center" alt="Coding" width="400" height="150" src="https://github.com/cabby1234/HackingWPA2Lab/assets/131496256/de076149-e800-4c3c-9138-876a1df4bf30">
<br>
<br>
<br>
<strong>The capture of our WPA handshake pulled up in Wireshark:</strong>
<br>
<img align="center" alt="Coding" width="400" height="150" src="https://github.com/cabby1234/HackingWPA2Lab/assets/131496256/bb486f75-80e9-466b-afb4-bba0030f9206">
<br>
<br>
 <br>
<strong>Aircrack-ng command to obtain the wireless keys, using the rockyou.txt wordlist:</strong>
<br>
<img align="center" alt="Coding" width="400" height="150" src="https://github.com/cabby1234/HackingWPA2Lab/assets/131496256/0a4f0847-8700-46ac-bb0e-047f1191e6f7">
<br>
<br>
 <br>
<strong>After running the command we were able to obtain the keys in seconds. (Keys are blocked out to maintain lab integrity)</strong>
<br>
<img align="center" alt="Coding" width="400" height="150" src="https://github.com/cabby1234/HackingWPA2Lab/assets/131496256/9a7ff105-3b76-4ec3-97ae-c80ec7cb94fc">




<!--
 ```diff
- text in red
+ text in green
! text in orange
@@ text in purple (and bold)@@
```
--!>
