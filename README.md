# CYBERSECURITY LAB ON HOW TO SET-UP PRACTICE LAB WITH KALI LINUS AND ORACLE VIRTUAL MACHINE FOR BEGINNERS


## **INTRODUCTION**

A safe practice environment is the foundation of any cybersecurity or ethical hacking training, because it lets a learner test tools and techniques without risking real systems. This project documents the setup of such a lab for beginners using Oracle VirtualBox as the virtualisation platform and Kali Linux as the attacking machine. Kali Linux is a distribution that ships with many security and penetration testing tools. The tools used were 7-Zip, which extracts the downloaded Kali image, VirtualBox, which hosts the virtual machine, and Kali Linux itself.

## **OBJECTIVE**
-	Set up a beginner friendly cybersecurity practice lab using Oracle VirtualBox as the virtualization platform.
-	Install Kali Linux as the attacking machine, using 7-Zip to extract the downloaded Kali image.
-	Create an isolated NAT Network with the address range 10.0.0.0/24, keeping lab traffic separate from the host and home network.
-	Confirm that the virtual machines can still reach the Internet from the isolated network.


## **Tools Used;** 
-	7-Zip: Used to unzipped downloaded files.
-	Oracle VirtualBox: This is the Virtual Machine used to run our operating system.
-	Kali Linux: Operating System

## LAB REQUIREMENTS CHECKLIST
Tick each item once it is done and its evidence is inserted below.
-	VirtualBox installed (latest recommended version)
-	Kali Linux set up as the attacking machine
-	Network configured in subnet 10.0.0.0/24
-	NAT Network created with 10.0.0.0/24
-	Clipboard and file drag/drop enabled in VM settings
-	Shared folder enabled, with /downloads shared from the host
-	Kali Linux IP address set to 10.0.0.2/24
-	Kali Linux has full Internet access

## IMPLEMENTATION STEPS AND EVIDENCE
Evidence: Showing all tools downloaded; 7-Zip download, VirtualBox download and Kali download

<img width="975" height="192" alt="image" src="https://github.com/user-attachments/assets/4f17eab4-a858-464a-8f1a-b276affaf24e" />

## **DOWNLOADED TOOLS**
- 7-Zip was installed from 7-zip.org.
- VirtualBox was downloaded from virtualbox.org and installed with default options. 
- The Kali Linux virtual machine image was downloaded from kali.org/get-kali, and extracted with 7-Zip which was then imported into VirtualBox.

## **CONFIGURING NAT NETWORK (10.0.0.0/24)**

A NAT Network was created in VirtualBox with the IPv4 prefix 10.0.0.0/24 and DHCP [enabled/disabled]. Network name: Network.

<img width="975" height="518" alt="image" src="https://github.com/user-attachments/assets/2c7c1f64-7b3a-4bf2-931f-4acdeae0c962" />
<div align="center">Evidence: NAT Networks list showing the new network and its 10.0.0.0/24 prefix </div>
<br>
<br>

<img width="975" height="469" alt="image" src="https://github.com/user-attachments/assets/8787e05b-cceb-4b9c-b1f1-4d7297d5fc89" />
<div align="center"> Evidence: NAT Network Details/Settings Window</div>
<br>
<br>

<img width="975" height="516" alt="image" src="https://github.com/user-attachments/assets/034e7c9d-cc01-4308-959a-d5ff60e54e9b" />
<div align="center">Evidence: VM network settings with the adapter attached to the NAT Network</div>
<br>
<br>

## **SET UP THE IP CONFIGURATION OF KALI LINUX**

Network configuration screen of where the Static IP was set
<img width="975" height="513" alt="image" src="https://github.com/user-attachments/assets/d25ef2c5-e11c-427d-b5ef-7223021ee491" />
<div align="center">Kali was given the Static Address 10.0.0.2. Gateway: 10.0.0.1. DNS: 8.8.8.8.</div>
<br>
<br>

<img width="975" height="508" alt="image" src="https://github.com/user-attachments/assets/e4ed2030-688e-475f-9e64-7f6e17c9c1fd" />
<div align="center">Evidence: Terminal output of ping 10.0.0.2 showing replies (Kali Terminal)</div>
<br>
<br>

<img width="975" height="434" alt="image" src="https://github.com/user-attachments/assets/68d4c25d-465c-4096-a551-4996bb3f7691" />
<div align="center">Evidence: Terminal output of ping google.com showing replies (Kali Terminal)</div>
<br>
<br>

<img width="975" height="512" alt="image" src="https://github.com/user-attachments/assets/492007ae-6c78-4a3d-a349-d2f8b78f8ecc" />
<div align="center">Evidence: GUI browsing Google and Amazon after configuration (Firefox)</div>
<br>
<br>

## **TAKE A SNAPSHOT OF THE VM**
A snapshot named was taken after a working configuration was confirmed, so the lab can be restored if something breaks.
<img width="975" height="518" alt="image" src="https://github.com/user-attachments/assets/da3fa05a-dca6-42b4-af50-cabea4647150" />
<div align="center">Evidence: Snapshots showing the new snapshot after setup</div>
<br>
<br>

## **CONCLUSION**
The lab meets every requirement in the task, VirtualBox hosts a Kali Linux attacker VM on a 10.0.0.0/24 NAT Network, Kali holds the static address 10.0.0.2/24, host-guest clipboard, drag/drop and shared folder work, and Kali reaches the Internet.
<br>
<br>

- Author: Oyewale Saliu
- Linkedlin: www.linkedin.com/in/oyewalesaliu
