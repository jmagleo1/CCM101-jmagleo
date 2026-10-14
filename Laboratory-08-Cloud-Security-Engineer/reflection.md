
# Mission 8: The Cloud Security Engineer - Reflection

In this laboratory activity, I learned how important it is to secure a cloud server using a firewall. I used UFW in Ubuntu to manage network traffic and allow only the ports needed by the server.

A host-based firewall protects a server by controlling incoming and outgoing network traffic directly on the machine. Even if the main network security is breached, the firewall can still block connections that are not allowed by its rules. This gives the server an additional layer of protection.

Managing open network ports is also important because every open port can be a possible entry point for attackers. By closing unnecessary ports and allowing only required services, we can reduce the server's attack surface and make it harder for unauthorized users to access the system.

In a real company, leaving MySQL port 3306 open to the public internet can be dangerous because attackers may try to access the database or exploit security weaknesses. If the database is compromised, important information such as customer records and company data could be exposed. Database access should be limited to trusted servers and authorized users.

This activity changed my perspective because I realized that a server can become vulnerable when its security settings are not properly configured. I learned that deploying an application is not enough; we also need to protect it by setting firewall rules and checking which ports are open. The correct configuration can help reduce security risks.

Having eight completed missions in my GitHub portfolio makes me feel that I am improving my cloud computing knowledge. Each activity helped me learn different skills, from deploying applications to monitoring systems and configuring security. My portfolio also serves as proof of my progress and the practical activities I have completed. I still have more to learn, but I am more confident in understanding basic cloud security and server management.

Overall, this mission taught me that cloud security requires careful configuration, regular checking, and continuous improvement.
