# Honey Share
(Antisyphon training lab from Cyber Deception/Active Defense)<br><br>
Full lab explanation available on my <a href="https://medium.com/@swathitadepalli/active-defense-and-cyber-deception-antisyphon-training-44c0ee851be4#0331">Medium</a>
## Honey Share
- Obtain you Kali IP, become root (```sudo su -```), and navigate to ```/opt/impacket/examples```
- Start the SMB server:
<pre>python3 ./smbserver.py -smb2support -comment 'secret' SECRET /secret </pre>
<img width="584" alt="Screenshot 2025-03-31 at 12 42 11 PM" src="https://github.com/user-attachments/assets/e67e2ffa-897f-4787-8c7f-c84c976fd872" /><br><br>
## Connect to the SMB Share
- In cmd, let's attempt to connect to the SMB share using:
<pre>net use * \\{YOUR KALI IP}\secret</pre>
- You should get an error: <br><br>
<img width="962" alt="Screenshot 2025-03-31 at 12 44 18 PM" src="https://github.com/user-attachments/assets/4228131d-21c2-40da-912b-01be6bb67c36" /><br><br>
- All connection attempts are logged:<br><br>
<img width="645" alt="Screenshot 2025-03-31 at 12 46 03 PM" src="https://github.com/user-attachments/assets/fb15c90e-1214-434a-85d6-b1655da71c44" /><br><br>
<a href="https://github.com/swathinator/Homelabs">Back to Homelabs</a>
