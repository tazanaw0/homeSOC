In this lab, I will build a security operations center to further my understanding of endpoint detection and response, log analysis, and more. This entails configuring 4 virtual machines: 
- [x] attack
	kali linux  
- [ ] client
	windows 11
- [x] siem (wazuh)
	https://documentation.wazuh.com/current/quickstart.html
	ubuntu linux 
		ran into an issue using curl to install wazuh packages. used wget instead. 15-20 minute installation time. 
		![[Pasted image 20250725113113.png]]
		![[Pasted image 20250725114939.png]]
		Adding both ports to ufw allow list. 'sudo ufw reload' updates new rules
		- **1514/tcp** = agent log forwarding to manager
		- **1515/tcp** = agent registration
		- **443/tcp** = web dashboard access
		![[Pasted image 20250725115755.png]]
			Overwrote the initial installation because I was unable to access the dashboard. It's now accessible over port 443

	ubuntu linux 
