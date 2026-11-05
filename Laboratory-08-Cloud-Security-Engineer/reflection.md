# Mission 8 Reflection

Completing this laboratory activity helped me understand why server security is important in cloud computing. A host-based firewall protects a server by monitoring and controlling network traffic. Even if the physical network perimeter is breached, the firewall can still block unauthorized connections based on its rules. This provides an additional layer of security for the server.

Managing open network ports is also important because every open port can become a possible entry point for attackers. Unnecessary open ports may expose services to security threats. By allowing only the ports needed by the application, we can reduce the attack surface and make the server more secure.

In a real enterprise environment, leaving a database port like 3306 for MySQL open to the public internet is dangerous. Attackers could attempt to guess passwords, exploit vulnerabilities, or access sensitive information stored in the database. Database connections should only be allowed from trusted application servers or authorized networks.

This mission changed my perspective because I realized that a working server is not automatically a secure server. Even a newly deployed application can become vulnerable if the proper security configurations are ignored. I learned that configuring a firewall and controlling network access are important responsibilities of a cloud security engineer.

Looking at my GitHub portfolio with eight completed missions makes me feel proud of my progress. I started by learning basic cloud concepts, and now I can deploy applications, manage containers, and configure firewall rules. Each mission gave me new knowledge and practical experience. I also learned how important it is to document my activities and provide screenshots as evidence. I still have many things to learn, but these eight missions have helped me become more confident in cloud computing.
