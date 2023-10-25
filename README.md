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
-------------------------------------------------------------------------
INTRODUCTION
 
Creating and deploying a static e-commerce shoe shop website on the Azure cloud platform is an excellent way to establish an online presence for your shoe business. Azure offers a robust and scalable infrastructure that can provide the reliability and security needed to run your e-commerce site effectively. In this guide, we'll take you through the process of setting up your website on Azure. In today's digital age, establishing an online e-commerce presence is crucial for the success of any retail business. Whether you're a small shoe boutique or a large footwear retailer, creating a website that allows customers to browse and purchase your products can significantly expand your customer base and boost sales. Azure, Microsoft's cloud computing platform, provides a reliable and scalable environment to host your e-commerce site. Our Azure-powered website ensures lightning-fast performance, secure transactions, and an impeccable user experience. Azure's robust infrastructure guarantees 24/7 availability, assuring you can shop for your favorite shoes at any time, from anywhere in the world. Explore our extensive collection of sneakers, heels, boots, and more, and enjoy a user-friendly interface that makes browsing and shopping a breeze. With Azure's cloud resources, we can effortlessly scale to meet peak demand during sales and promotions, ensuring you never miss out on the latest trends.



BACKGROUND

 In the early 2000s, the e-commerce landscape witnessed the emergence of online shoe shops, marking a significant shift in the way people shopped for footwear. These websites aimed to provide customers with a convenient and extensive platform for browsing, selecting, and purchasing shoes from the comfort of their homes. The background of these e-commerce shoe shops is rooted in the digital revolution and the growing consumer preference for online shopping. With the advent of secure online payment methods and advancements in web technology, it became feasible to create user-friendly, visually appealing platforms for showcasing a wide range of shoe brands and styles. These websites offered various advantages, such as a vast product catalog, detailed product descriptions, high-quality images, and customer reviews, empowering shoppers to make informed choices. Additionally, e-commerce platforms streamlined the purchasing process, offering features like wish lists, cart management, and easy returns. These websites offered various advantages, such as a vast product catalog, detailed product descriptions, high-quality images, and customer reviews, empowering shoppers to make informed choices. Additionally, e-commerce platforms streamlined the purchasing process, offering features like wish lists, cart management, and easy return.
 
Resource group: 

Resources group is a collection or group in azure cloud,it making easier to manage , monitor or organize them

Traffic Manager: To enhance the availability and performance of our website, we implemented Azure Traffic Manager. This service efficiently distributed incoming web traffic between the two virtual machines in Subnet 1, ensuring a seamless experience for our visitors.

Virtual Network : In Azure to isolate your resources and enhance security. Mention that it's like your private network in the cloud. Within the Virtual Network, you divided it into two subnets. Subnet 1 is for the frontend of your website, and Subnet 2 is for the database. Explain that this segregation helps manage and secure traffic. In Subnet 1, you have two Virtual Machines. One is for deploying your website, and the other is for redundancy or scaling. The VM in Subnet 2 is for hosting the database.VMs are like virtual computers running in the cloud.

DNS Zone: 1.We created a DNS Zone to manage the domain name of our shoe shop website. This allowed us to map our user-friendly domain (shoes.riyashukla.online ) to the IP address of our Traffic Manager. So, when visitors access our site, they are seamlessly routed to the appropriate VM. 2.In your case, you created a DNS Zone to host your website's domain name. This means that when someone types in your website's address in a web browser, the DNS Zone directs them to the correct destination. In this setup, it's linked to the Traffic Manager. 3.So, when a user accesses your website, the DNS Zone plays a crucial role. It translates your user-friendly domain name (e.g., www.yourwebsite.com) into the IP address of your Traffic Manager. The Traffic Manager then takes care of distributing the user's request to the appropriate Virtual Machine within your Subnet 1. This ensures that your website loads efficiently and reliably for your visitors.

Monitoring and Alerts: To ensure the optimal functioning of our website, we implemented monitoring and alerting systems. These tools provided insights into the performance, health, and potential issues of our website, enabling us to take timely actions and maintain a high-quality user experience.

Azure CDN: To further enhance the website's performance, we integrated Azure Content Delivery Network (CDN). This technology cached and delivered website content from locations closer to the end-users, resulting in faster load times and a smoother browsing experience.

Architecture:

![image](https://github.com/Riyashukl/Shoes-shop-azure-project/assets/103056264/593411ba-a39f-4c1e-a1a2-f29747baf59d)

Create Virtual Network:



![Create virtual Network](https://github.com/Riyashukl/Shoes-shop-azure-project/assets/103056264/345b823e-dece-46b5-a78c-509070630bb9)

![steps1](https://github.com/Riyashukl/Shoes-shop-azure-project/assets/103056264/a36b3ff9-6c98-458e-ba56-8335d527a20a)

![step2](https://github.com/Riyashukl/Shoes-shop-azure-project/assets/103056264/9c4964fa-b3c4-4139-92cb-4364522df822)

![step3](https://github.com/Riyashukl/Shoes-shop-azure-project/assets/103056264/6fb4838d-ce46-4d47-9dc1-906a05c536ef)


Create Virtual machine:
1.Create Machine 1 in subnet1

![image](https://github.com/Riyashukl/Shoes-shop-azure-project/assets/103056264/62167709-878d-44d6-8ed1-ea63ed9c7adf)

![image](https://github.com/Riyashukl/Shoes-shop-azure-project/assets/103056264/c86a9953-cee9-446d-bd3d-42627f6d0dd5)

![image](https://github.com/Riyashukl/Shoes-shop-azure-project/assets/103056264/afc0ec9e-73b8-4ca6-b1d3-c808695daaa8)

![image](https://github.com/Riyashukl/Shoes-shop-azure-project/assets/103056264/fa2b8edb-6054-4d85-8582-b8bfa9d24bf4)

![image](https://github.com/Riyashukl/Shoes-shop-azure-project/assets/103056264/f1be0b8c-3ad6-4bf7-bdb2-fafcdc8c1ef5)


Create virtual machine for database in subnet2:

![image](https://github.com/Riyashukl/Shoes-shop-azure-project/assets/103056264/d0aded5d-628f-460b-a89c-64a2f7d2c5c7)

Create Azure MySqL database:

![image](https://github.com/Riyashukl/Shoes-shop-azure-project/assets/103056264/3efcd0ab-0a8c-4755-9e24-3a922a47f982)

![image](https://github.com/Riyashukl/Shoes-shop-azure-project/assets/103056264/69cffae6-e85c-4aec-b663-b10a951696a4)

![image](https://github.com/Riyashukl/Shoes-shop-azure-project/assets/103056264/d90f7326-74ea-4d91-ac85-145a0aeae934)

Install Mysql database in Machine3(Database Server Machine):

![image](https://github.com/Riyashukl/Shoes-shop-azure-project/assets/103056264/7ce146b1-1bd4-40e0-94ff-3eb23c9494f6)

Create Azure CDN:

![image](https://github.com/Riyashukl/Shoes-shop-azure-project/assets/103056264/c225deed-141c-40ba-b30c-885f527ddf4d)

![image](https://github.com/Riyashukl/Shoes-shop-azure-project/assets/103056264/27399591-1f2d-4a5e-a925-ff7c63c3b300)

![image](https://github.com/Riyashukl/Shoes-shop-azure-project/assets/103056264/c24a4202-4d9a-4315-8faf-cdafdcbd8c66)

Deploy code on virtual machine using Github:

Deploy same code on machine1 and Machine2

![image](https://github.com/Riyashukl/Shoes-shop-azure-project/assets/103056264/28339b30-f19f-485e-8388-3477e6600e0a)

![image](https://github.com/Riyashukl/Shoes-shop-azure-project/assets/103056264/5b030123-00ff-4679-8a20-a6e329e69b32)

![image](https://github.com/Riyashukl/Shoes-shop-azure-project/assets/103056264/9c005b6c-aa28-4334-9f68-20fb8f1a46d7)

![image](https://github.com/Riyashukl/Shoes-shop-azure-project/assets/103056264/aa18cf7a-acfc-4048-8fe9-a590064acc89)

![image](https://github.com/Riyashukl/Shoes-shop-azure-project/assets/103056264/46532c24-57c8-4461-be2f-056b3c03e900)

![image](https://github.com/Riyashukl/Shoes-shop-azure-project/assets/103056264/2cf3093b-1414-40ac-bf17-2c63515de6c7)

![image](https://github.com/Riyashukl/Shoes-shop-azure-project/assets/103056264/5f1f2e08-41e2-4fd7-9df2-5e302a4212dc)

Commands:

![image](https://github.com/Riyashukl/Shoes-shop-azure-project/assets/103056264/f41a5a7c-ca6b-4190-bf54-45b440b856bb)

![image](https://github.com/Riyashukl/Shoes-shop-azure-project/assets/103056264/9db4e71c-e3cc-4109-859a-fc4a6aa16c48)


Create DNS Zone for hosting:

Step 1:Visit Hostinger’s website
Step 2:Search for Your Domain(riyashukla.online)
Step 3:Review your cart, sign in or Create an account
Step 4:Place your order confirm
Step 5:Domain Registration

![image](https://github.com/Riyashukl/Shoes-shop-azure-project/assets/103056264/3a2542b1-ff3e-42cf-9055-fcb5a89454ac)

![image](https://github.com/Riyashukl/Shoes-shop-azure-project/assets/103056264/009e7350-a3ed-44b2-a4f3-6d0d5cb4f626)

•Create a DNS zone to host your website domain name .This means that when someone types in your websites address in a web browser, the DNS zone directs them to the correct destination.In this setup, its linked to the traffic manager

![image](https://github.com/Riyashukl/Shoes-shop-azure-project/assets/103056264/d35c7e29-9998-40e3-935f-461003560345)

Create traffic manager  (Priority based):

Traffic Manager to distribute incoming requests between the two VMs in subnet1.It improves the availability and Performance of your website by load balancing.  

•	Now we need to create Traffic Manager it distrubuting the Users request to the apporopriate Virtual Machine within your subnet 1.This ensures that your website loads efficiently and reliably for your visitors.
•	Create a Traffic Manager Profile:

•	In the Azure Portal, search for and select "Traffic Manager profiles."
•	Click the "+ Add" button to create a new Traffic Manager profile.
•	Follow the prompts to configure the profile with your desired settings, including routing method (e.g., Priority, Weighted, Geographic), and add the endpoints (the VMs in your Subnet 1).
•	We select routing method (Priority)

![image](https://github.com/Riyashukl/Shoes-shop-azure-project/assets/103056264/ac22a69c-dac3-4f1e-bb4a-9432be385351)

Link Traffic Manager to the DNS zone :

•	In the DNS Zone settings, under "Records," you should create a CNAME (Alias) record that points to your Traffic Manager profile. This is where you connect the DNS Zone to the Traffic Manager.
•	Add a CNAME record with a name like "www" or "@", and set its value to the fully qualified domain name (FQDN) of your Traffic Manager profile.


![image](https://github.com/Riyashukl/Shoes-shop-azure-project/assets/103056264/986241d4-0621-45cb-aeac-5429a57f8d1b)

Update Your Domain Registrar:

•	If your domain is registered with a domain registrar (Hostingr), you need to update the DNS settings there. Log in to your domain registrar's website.
•	Change the nameservers or DNS settings to point to Azure's DNS servers (you can find these DNS server details in your Azure DNS Zone settings).

![image](https://github.com/Riyashukl/Shoes-shop-azure-project/assets/103056264/46f923f2-cc69-4652-bf41-f0202e658bcc)

![image](https://github.com/Riyashukl/Shoes-shop-azure-project/assets/103056264/cd1ec117-1375-4c02-a8e7-e3153ad12eba)

Azure Monitor:

Monitoring in Azure is a crucial aspect of managing and maintaining the health, performance, and security of your cloud resources. Azure provides a comprehensive set of monitoring and management tools. Here's an overview of how monitoring works in Azure:


![image](https://github.com/Riyashukl/Shoes-shop-azure-project/assets/103056264/ed2caf0e-d52e-4702-b9b2-8aa0204a742e)


Azure Alerts: You can configure alerts to notify you when specific conditions are met. For example, you can set up alerts for high CPU usage, low memory, or any other metrics. These alerts can be sent to various notification channels, including email, SMS, or even third-party services like Slack.
Azure Monitor for VMs: If you're running virtual machines (VMs) in Azure, you can use this service to collect performance and health data for those VMs.
Metrics: Metrics are numerical data collected from your resources. Azure Monitor collects, stores, and analyse metrics to help you understand how your resources are performing. You can set up alerts based on these metrics to be notified of any issues.
Azure Application Insights: This service is part of Azure Monitor and is focused on application performance monitoring. It helps you track the performance and usage of your web applications and other services.



Azure Alerts:

![image](https://github.com/Riyashukl/Shoes-shop-azure-project/assets/103056264/13443264-1fe9-43c7-9330-7095307eb715)

Metrics:
![image](https://github.com/Riyashukl/Shoes-shop-azure-project/assets/103056264/e68db4dd-c1d3-48bd-89ac-69c1b5cdb8a3)

![image](https://github.com/Riyashukl/Shoes-shop-azure-project/assets/103056264/3e4b78a3-f755-40f3-bec2-19534878e1e1)

Network:

![image](https://github.com/Riyashukl/Shoes-shop-azure-project/assets/103056264/23dfc53b-75b9-4856-8537-643dfc7300cf)


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
In summary, our project successfully leveraged Azure's cloud computing capabilities to create and deploy a shoe shop website with a strong focus on availability, performance, and user experience. The use of Virtual Networks and Subnets ensured a secure and organized infrastructure. Traffic Manager efficiently managed incoming traffic, while DNS Zone facilitated seamless domain name resolution.

Our commitment to monitoring and alerts helped us stay proactive in maintaining the website's reliability. Lastly, the Azure CDN optimized content delivery, making our site faster and more responsive to our customers.

In conclusion, by harnessing Azure's cloud services and following best practices, we've not only created a functional online presence but also ensured that it's accessible, reliable, and responsive, providing an excellent shopping experience for our customers. This project demonstrates the power of cloud computing in enabling e-commerce businesses to thrive in the digital age.



