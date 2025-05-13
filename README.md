# Physical-Networking-Lab


# Overview 
In this lab I will be taking the concepts I learned from cisco packet tracer and applying it in the real world using physical cisco  equipment. The equipment I will be using in this lab are 2 cisco 2811 routers, 2 cisco 2960 catalyst switches, 2 end devices, one CAT 6 crossover ethernet cable, and 4 CAT 6 straight through ethernet cables. I will be recreating the network topology shown in the image below.

![Alt text](https://github.com/user-attachments/assets/9e36f0d8-6bfc-4c1b-bb2d-c4e985178235)



![Alt text](https://github.com/user-attachments/assets/74dfb359-2ad1-49b0-8d59-60bfeb2fcccd)



# Networking concepts Implemented in this Lab:
  -	VLAN’s 
  -	Trunking
  -	DHCP
  -	RIP Routing Protocol
  -	Access Control Lists (ACL’s)



# Tasks:
    1.	Configure VLAN Interfaces for VLAN’s 10 and 20 on switches 1 and 2, assign ports 2-4 of each switch to VLAN 10 and the ports 5-8 to VLAN 20 (The first port on each switch will not be assigned to any VLAN we will be connecting it to the router)
    2.	Configure trunk interfaces on interface F0/1 on each switch so it can carry traffic from any VLAN
    3.	Configure IP addresses on router interfaces
    4.	Configure virtual VLAN router interface ip addresses so that each VLAN has a gateway
    5.	Configure the routers as DHCP servers to hand out IP addresses to their end devices
    6.	Configure the end devices to receive a DHCP IP address
    7.	Configure RIP routing protocol between the routers
    8.	Configure a standard ACL to prevent the devices on the printers VLAN from getting out of the network
    9.	Test communication

# Execute: 
1. First I will create VLANs 10 and 20 on both switches and assign interfaces to those VLANs

![Alt text](https://github.com/user-attachments/assets/77fd5f6e-0e09-43e2-8920-70358642e379)

2. Next I will configure interface F0/1 as a trunk interface on both switches so that it can carry traffic from any VLAN

![Alt text](https://github.com/user-attachments/assets/647304f0-09b2-45f4-a8d9-1e18b76bf240)

3. Next I will configure IP addresses on router interfaces for both routers 1 and 2
![Alt text](https://github.com/user-attachments/assets/265bacd0-a52c-43d5-a7ba-11ec57a8868e)

4. Now I will configure virtual VLAN router interface IP addresses on each router so that each VLAN has a default gateway

![Alt text](https://github.com/user-attachments/assets/ce887df0-7eec-48ab-b3e4-836ec2a5a025)


5. Next I will configure the routers to act as DHCP servers to hand out IP addresses to their end devices

![Alt text](https://github.com/user-attachments/assets/17cebd28-931d-45fb-b934-1789ab617a4c)

6. I connected end devices to each switch and made sure they were receiving an IP address from the DHCP router/server

7. Next I configured RIP routing protocol between the routers so that they could share their routing tables with each other and communicate

   ![Alt text](https://github.com/user-attachments/assets/c2b20301-2432-4d96-a841-57c61f4ddc6d)

8. Next I configured a standard ACL to prevent the devices on the printers VLAN from getting out of the network

![Alt text](https://github.com/user-attachments/assets/d20075cc-c183-447f-9286-e659f7f56ac5)

9. Once everything was configured I tested for connectivity by using the ping command, I verified each device could ping their gateway, devices on their same network, and devices on other VLANs

   

