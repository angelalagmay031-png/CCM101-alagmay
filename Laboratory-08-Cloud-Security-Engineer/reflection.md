# Mission Reflection

Completing this cloud security mission helped me understand why protecting a server is important. I learned that a host-based firewall can protect a server even if the physical network security is breached. It works directly on the server by controlling incoming and outgoing network traffic. This adds another layer of security against unauthorized connections.

Managing open network ports is also important because every open port can become a possible entry point for attackers. If unnecessary ports are left open, attackers may find vulnerable services and use them to access the server. By using UFW and allowing only the ports needed, I can reduce the server's attack surface and make it more secure.

In a real enterprise environment, leaving a database port like 3306 for MySQL open to the public internet is dangerous because attackers can attempt to access the database, guess passwords, or exploit vulnerabilities. If they succeed, sensitive information such as customer records and company data could be exposed or stolen. Database access should be restricted to trusted servers and authorized users instead of allowing connections from everyone.

This mission changed my perspective because I realized that a server can become vulnerable when its security settings are not configured properly. Before this activity, I did not fully understand how important firewall rules were. Now, I know that even simple commands, such as setting a Default Deny policy and allowing only necessary ports, can help improve server security. I also learned that testing the configuration is important to make sure the application still works after applying security rules.

With eight completed missions, my GitHub portfolio is becoming more organized and meaningful. It shows the commands I used, the documentation I created, and the skills I practiced in cloud computing and security. I am also gaining more confidence in using Linux commands and documenting my work. Overall, this mission helped me understand that securing a server requires careful configuration, regular checking, and continuous learning.
