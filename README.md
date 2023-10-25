# Shoes-shop-azure-project:
Create and Deploy Static e-commerce shoes Shop website on cloud Using Azure cloud provider
Virtual Network and Subnets:
We started by setting up a Virtual Network in Azure to create a secure and isolated environment for our resources. Within this network, we divided it into two subnets. Subnet 1 was designated for our frontend, where we hosted two virtual machines for deploying our website. Subnet 2 was dedicated to the database, which was hosted on another virtual machine.
------------------------------------------------------------------------
Youtube Video Link:

https://youtu.be/5ZYcGSnf_5E?si=DssRQ3yNLvCxb8bn

Shoes-shop website link:

http://shoes.riyashukla.online/index.html

------------------------------------------------------------------------

[Architecture](https://github.com/Riyashukl/Shoes-shop-azure-project/assets/103056264/593411ba-a39f-4c1e-a1a2-f29747baf59d)

[Create virtual Machine](https://github.com/Riyashukl/Shoes-shop-azure-project/assets/103056264/345b823e-dece-46b5-a78c-509070630bb9)

[1](https://github.com/Riyashukl/Shoes-shop-azure-project/assets/103056264/a36b3ff9-6c98-458e-ba56-8335d527a20a)




Resource group: 
Resources group is a collection or group in azure cloud,it making easier to manage , monitor or organize them


Traffic Manager: 
To enhance the availability and performance of our website, we implemented Azure Traffic Manager. This service efficiently distributed incoming web traffic between the two virtual machines in Subnet 1, ensuring a seamless experience for our visitors.


Virtual Network :
In Azure to isolate your resources and enhance security. Mention that it's like your private network in the cloud.
Within the Virtual Network, you divided it into two subnets. Subnet 1 is for the frontend of your website, and Subnet 2 is for the database. Explain that this segregation helps manage and secure traffic.
In Subnet 1, you have two Virtual Machines. One is for deploying your website, and the other is for redundancy or scaling. The VM in Subnet 2 is for hosting the database.VMs are like virtual computers running in the cloud.

DNS Zone: 
1.We created a DNS Zone to manage the domain name of our shoe shop website. This allowed us to map our user-friendly domain (shoes.riyashukla.online ) to the IP address of our Traffic Manager. So, when visitors access our site, they are seamlessly routed to the appropriate VM.
2.In your case, you created a DNS Zone to host your website's domain name. This means that when someone types in your website's address in a web browser, the DNS Zone directs them to the correct destination. In this setup, it's linked to the Traffic Manager.
3.So, when a user accesses your website, the DNS Zone plays a crucial role. It translates your user-friendly domain name (e.g., www.yourwebsite.com) into the IP address of your Traffic Manager. The Traffic Manager then takes care of distributing the user's request to the appropriate Virtual Machine within your Subnet 1. This ensures that your website loads efficiently and reliably for your visitors.

Monitoring and Alerts: 
To ensure the optimal functioning of our website, we implemented monitoring and alerting systems. These tools provided insights into the performance, health, and potential issues of our website, enabling us to take timely actions and maintain a high-quality user experience.

Azure CDN: 
To further enhance the website's performance, we integrated Azure Content Delivery Network (CDN). This technology cached and delivered website content from locations closer to the end-users, resulting in faster load times and a smoother browsing experience.

Conclusion:
In conclusion, by harnessing Azure's cloud services and following best practices, we've not only created a functional online presence but also ensured that it's accessible, reliable, and responsive, providing an excellent shopping experience for our customers. This project demonstrates the power of cloud computing in enabling e-commerce businesses to thrive in the digital age.
Youtube video link

