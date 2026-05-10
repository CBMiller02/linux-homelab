# linux-homelab
Linux system administration and security home lab using Linux Mint and VirtualBox.

Virtual Machine Configuration

- Host system: macOS
- Virtualization Platform: Oracle VirtualBox
- GuestOS: Linux Mint
- Base Memory/RAM: 6144MB (or approx. 6GB)
- Virtual CPU's: 4
- Boot order: Optical Drive, Hard Disk
- Pointing Device: USB Tablet
- Video Memory: 16MB

Host name:

![Screenshot 2026-05-09 at 4 38 39 PM](https://github.com/user-attachments/assets/9809fe40-6b51-4cdc-91ee-1edd8d9f88f4)


Memory:

![Screenshot 2026-05-09 at 4 39 00 PM](https://github.com/user-attachments/assets/2417c989-8a6f-4a14-97f7-1c5424f25cf9)


Disk space usage:

![Screenshot 2026-05-09 at 4 39 24 PM](https://github.com/user-attachments/assets/0db9cd11-915b-4c41-8677-01fefdfe8454)


CPU architecture and breakdown:

![Screenshot 2026-05-09 at 4 42 57 PM](https://github.com/user-attachments/assets/126a9e73-e05f-4905-9ef7-6d507dbc6e6a)
![Screenshot 2026-05-09 at 4 43 15 PM](https://github.com/user-attachments/assets/f8a63fd9-aefc-4ee1-8914-96f5edfe4d6e)

------------
Updating the system:

![Screenshot 2026-05-09 at 5 17 52 PM](https://github.com/user-attachments/assets/46bd4fae-2132-442b-855b-5395427f73eb)

![Screenshot 2026-05-09 at 5 18 08 PM](https://github.com/user-attachments/assets/1d1d200d-b949-4aa6-9f06-00a700c40ab1)

------------
Next, I went to go and download the following:
- htop
- net-tools
- curl
- git
- openssh-server
- ufw
- -y flag

The purpose and reason for downloading these was to configure a more secure and user friendly environment. Utilizing 'htop' makes is easier to monitor CPU usage, running processes, and overall memory consumption. 'net-tools' so I can run command such as ipconfig and netstat.  'curl' is good for transferring data and downloading files. 'git' is essentially the version control system for tracking changes and collaborating on projects, so that could be useful in the future. 'openssh-server' allows me to remotely logon to my Linux device on a different network. And finally, 'ufw' or Uncomplicated Firewall, which will allow me to monitor firewall rules in a more user-friendly way.

**to note, I did download these packages before, but just wanted to document the command for downloading them.

![Screenshot 2026-05-10 at 5 09 22 PM](https://github.com/user-attachments/assets/8b068a59-b4b6-446f-b1bc-190cb3696144)

Now below are the respective outputs from running htop, git --version, and curl

![Screenshot 2026-05-10 at 5 10 25 PM](https://github.com/user-attachments/assets/d69b2156-abfd-4032-93bb-c1bac93efaab)

![Screenshot 2026-05-10 at 5 10 45 PM](https://github.com/user-attachments/assets/27108688-4d25-493c-b2a8-642895345551)

![Screenshot 2026-05-10 at 5 11 07 PM](https://github.com/user-attachments/assets/03d12d8b-e644-4175-9ca2-d35b4086b5de)

That concludes basic formatting and setup for my Linux home lab.


