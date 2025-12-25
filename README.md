# doom-coding
Tired of Doom Scrolling? Replace one addiction with the marginally healthier addiction of Doom Coding. Here's a 5-minute guide for how to smartphone to code anywhere at anytime. 

# What You Need
1. A Computer running 24/7 with Internet Connection
2. A Smartphone

# Overview
Use Tailscale, Termius, Claude Code, and laptop to continue building anywhere you have Internet connection.

# Getting Started

1. Set Up Your Computer
- Disable sleep in power settings
<img width="960" height="564" alt="image" src="https://github.com/user-attachments/assets/3305aaf1-046c-4505-89ba-2398d0601bf7" />
- Enable SSH/Remote Login
<img width="944" height="626" alt="image" src="https://github.com/user-attachments/assets/b13ee636-ecec-4962-bf83-d32adc219809" />
- Install Tailscale and sign in
[https://tailscale.com/](https://tailscale.com/download)
<img width="1179" height="1493" alt="image" src="https://github.com/user-attachments/assets/f3d68264-0aa4-47a6-b7c9-2efe18bc3627" />
- Install Claude Code on your laptop
https://code.claude.com/docs/en/quickstart

2. Set Up Your Phone
- Install Tailscale -> Sign in with the same account
- Install Termius
https://termius.com/index.html
- Note your MagicDNS address of your computer (e.g., my-computer.tailnet-name.ts.net)
<img width="1179" height="1075" alt="image" src="https://github.com/user-attachments/assets/39e3d25a-167b-466d-8113-a9d3c6abe450" />
- Create a new host in Termius:
  * Hostname: Your MagicDNS address (my-computer.tailnet-name.ts.net)
  * Port: 22
  * Username/Password: Your login for your computer
 
3. Connect and Code
- Turn on Tailscale VPN on your phone
<img width="1179" height="721" alt="image" src="https://github.com/user-attachments/assets/03646788-619b-427e-8e47-5bf8219c1c36" />
- Tap your host in Termius
<img width="1179" height="1090" alt="image" src="https://github.com/user-attachments/assets/18d5a03e-acf7-4069-93c2-c67d45a25183" />
- Run "claude" and start coding

# Doom Coding Best Practices
- Track your progress: End sessions by asking Claude to update CLAUDE.md with where you left off
- Preview websites:
  Go to your desired directory and start an HTTP server
  '''python -m http.server 3005'''
  then visit http://your-machine.tailnet-name.ts.net:3005 in a browser on your phone
  _Whereever you would use localhost:PORT to view an application, you need to replace localhost with your-machine.tailnet-name_
- View Databases: Use the PostgreSQL app to troubleshoot databases on the go
  https://apps.apple.com/us/app/postgresql-client/id1233662353
