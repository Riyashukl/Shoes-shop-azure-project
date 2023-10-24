# Shoes-shop-azure-project
Create and Deploy Static e-commerce shoes Shop website on cloud Using Azure cloud provider
Virtual Network and Subnets:
We started by setting up a Virtual Network in Azure to create a secure and isolated environment for our resources. Within this network, we divided it into two subnets. Subnet 1 was designated for our frontend, where we hosted two virtual machines for deploying our website. Subnet 2 was dedicated to the database, which was hosted on another virtual machine.

Traffic Manager: 
To enhance the availability and performance of our website, we implemented Azure Traffic Manager. This service efficiently distributed incoming web traffic between the two virtual machines in Subnet 1, ensuring a seamless experience for our visitors.

DNS Zone: 
We created a DNS Zone to manage the domain name of our shoe shop website. This allowed us to map our user-friendly domain (shoes.riyashukla.online ) to the IP address of our Traffic Manager. So, when visitors access our site, they are seamlessly routed to the appropriate VM.

Monitoring and Alerts: 
To ensure the optimal functioning of our website, we implemented monitoring and alerting systems. These tools provided insights into the performance, health, and potential issues of our website, enabling us to take timely actions and maintain a high-quality user experience.

Azure CDN: 
To further enhance the website's performance, we integrated Azure Content Delivery Network (CDN). This technology cached and delivered website content from locations closer to the end-users, resulting in faster load times and a smoother browsing experience.

Conclusion:
In conclusion, by harnessing Azure's cloud services and following best practices, we've not only created a functional online presence but also ensured that it's accessible, reliable, and responsive, providing an excellent shopping experience for our customers. This project demonstrates the power of cloud computing in enabling e-commerce businesses to thrive in the digital age.
