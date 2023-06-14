<h2>📁 Basic Home Lab Running Active Directory</h2>

<h3>Description</h3>

For this project, I've built an basic home AD using a virtualized environment with Oracle VirtualBox. AD is a Microsoft's service and can easily span whole corporations, acting as a “phone book” for Windows desktops, printers, and other computers that need authentication services. 

<h3>AD project diagram:</h3>

<p align="center">
<img src= "https://i.imgur.com/eOE9oPM.jpg" height="80%" width="80%"/>
</p>

<h3>Main steps:</h3>

- First, install Server 2019 ISO and set up a virtual machine to run as the Domain Controller. It should be connected to the external network and also to a private network that we're going to create for client connections.
- Assign an IP address to the internal network, while the external network can obtain an IP address automatically from the home router.
- Next, install AD and create the domain. Configure NAT and routing to allow the clients (Windows 10) in the private network to access the internet.

<p align="center">
<img src= "https://i.imgur.com/DdfSRmI.png" height="80%" width="80%"/>
</p>

- Set up DHCP on the Domain Controller to automatically assign IP addresses to the clients.

<p align="center">
<img src= "https://i.imgur.com/AFGAEaW.png" height="80%" width="80%"/>
 </p>
 
- Utilize a user creation script to add over 1,000 users to the AD.

<p align="center">
<img src= "https://i.imgur.com/CroG5aj.png" height="80%" width="80%"/>
</p>

<p align="center">
<img src= "https://i.imgur.com/fZYc47k.png" height="80%" width="80%"/>
</p>

- Finally, log in to the client machine to verify if it is successfully connected to our domain.

<p align="center">
<img src= "https://i.imgur.com/vMB3kzF.png" height="80%" width="80%"/>
</p>

<p align="center">
<img src= "https://i.imgur.com/4rMz6kQ.png" height="80%" width="80%"/>
</p>

<h4>You can see that we got ours users installed and our client is running on the domain we've created! This kind simulates how you utilize a computer on a corporate network, after you've added to the AD of the company.</h4>

