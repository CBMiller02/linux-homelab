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

---------------------

Next I will go through the basics of adding a user 'analyst1'.

![Screenshot 2026-05-11 at 8 20 45 AM](https://github.com/user-attachments/assets/63c727f9-513e-45d4-8254-0a641a75389c)

![Screenshot 2026-05-11 at 8 21 33 AM](https://github.com/user-attachments/assets/69867fef-70e4-4013-b34b-094cd43192b3)

![Screenshot 2026-05-11 at 8 22 03 AM](https://github.com/user-attachments/assets/f249d5d2-3dc0-44df-b7e8-69bd0878d2d2)

---------------------

Now, for networking basics:

First running the command 'ip a' so I can view my IP configuration:

![Screenshot 2026-05-11 at 8 25 49 AM](https://github.com/user-attachments/assets/d73b9573-34d6-447a-a763-0810f6a5b3ed)


Now for open connections and ports I run 'ss -tuln'.

![Screenshot 2026-05-11 at 8 26 37 AM](https://github.com/user-attachments/assets/32719bd6-c0e0-4a48-9d63-9353a0e5d22f)


Finally I will text the connectivity.  For this I'll just use a popular search engine website, Google.com. To run this command, I'll simply run the command 'ping google.com'.  To stop or quit the command, I'll simply use 'CTRL +C'.

![Screenshot 2026-05-11 at 8 28 21 AM](https://github.com/user-attachments/assets/4aa03ca0-2530-4e57-9e6b-141ccfd5e770)

----------------------------

Firewall configuration
First off, we will run the command of 'sudo ufw enable' to enable our firewall.

![Screenshot 2026-05-11 at 8 32 54 AM](https://github.com/user-attachments/assets/a708c31a-55c1-479b-b8f7-be48213ab646)


We can see that the firewall is active and enabled, which was due to us installing 'ufw' at the beginning of this Linux home lab setup. Now we're going to run out firewall with verbose to get a better representation of what's going on. To do this we'll run the command of 'sudo ufw status verbose'.

![Screenshot 2026-05-11 at 8 33 16 AM](https://github.com/user-attachments/assets/a067f2b3-9f70-47ba-b9ea-d81e33877d37)

---------------------------




