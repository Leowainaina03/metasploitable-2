# metasploitable-2
In this project I will scanning metasploitable 2 and finding its open ports and how to exploit them

# tools
nmap
msfconsole

# steps
login to metaspoitable with username msfadmin and password msfadmin
<img width="1433" height="888" alt="Screenshot 2026-09-22 at 12 41 57" src="https://github.com/user-attachments/assets/c2a3ed54-9415-427c-bc3f-6200bbe9c389" />

finding metasploitable IP with the command ifconfig
<img width="1382" height="645" alt="Screenshot 2026-09-22 at 12 44 33" src="https://github.com/user-attachments/assets/d25e8599-bb26-437d-8e8d-5ff3837204fc" />

I pinged the machines IP addresses to make sure the virtual machines are communicating
<img width="722" height="252" alt="Screenshot 2026-09-22 at 15 30 44" src="https://github.com/user-attachments/assets/ab4213ca-1ed6-4fa3-b201-b65aa4084560" />

<img width="722" height="226" alt="Screenshot 2026-09-22 at 15 31 17" src="https://github.com/user-attachments/assets/d441faa5-ffed-4a08-b7c4-2d85e1c0e2ea" />

After running the map scan I found out that all port are open
After finding the open ports I will start exploiting the ports

# port 21 ftp
I scanned the port and found the vulnerability vsftpd 2.3.4
<img width="666" height="240" alt="Screenshot 2026-09-22 at 16 03 51" src="https://github.com/user-attachments/assets/1efd674d-77b6-42c5-9883-f8589b540a3d" />

I used the msgconsole to search it where I managed to find a backdoor
<img width="636" height="259" alt="Screenshot 2026-09-22 at 16 09 09" src="https://github.com/user-attachments/assets/1fef8a28-0cb2-470a-96c4-5bdf0d2cfdc6" />

After that I started exploiting the backdoor
<img width="636" height="169" alt="Screenshot 2026-09-22 at 16 16 23" src="https://github.com/user-attachments/assets/ec82d257-d27f-4954-b657-9b237aaf6689" />

<img width="651" height="684" alt="Screenshot 2026-09-22 at 16 50 56" src="https://github.com/user-attachments/assets/e9559ef8-7801-488f-af41-c4876d9ea45a" />

I gained access to the shell
<img width="651" height="529" alt="Screenshot 2026-09-22 at 16 53 53" src="https://github.com/user-attachments/assets/b094d9a8-5e18-4391-ab73-0cf030be46ad" />


# port 22 ssh
In port 22 I brute forced to the port using a users.txt and password.txt that I created
I used the auxiliary scanner to do it
<img width="1269" height="594" alt="Screenshot 2026-09-22 at 17 50 01" src="https://github.com/user-attachments/assets/3201932e-8bd3-4ce8-9147-07a422507763" />

creating the user.txt and password.txt
<img width="598" height="541" alt="Screenshot 2026-09-22 at 17 37 30" src="https://github.com/user-attachments/assets/ced1d474-e0b7-47f0-921c-6fffcbbc7cf8" />

using the users.txt and password.txt to run the brute force and did ssh to metasploitable
<img width="1269" height="660" alt="Screenshot 2026-09-22 at 18 41 06" src="https://github.com/user-attachments/assets/43668251-e8d0-44b4-8d7d-089a41437d05" />

<img width="752" height="639" alt="Screenshot 2026-09-22 at 18 52 18" src="https://github.com/user-attachments/assets/873117a0-d0ee-40e1-9e6b-5a9d8de0f3a6" />

