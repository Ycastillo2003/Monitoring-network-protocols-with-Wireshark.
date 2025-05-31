eeeeee![image](https://github.com/user-attachments/assets/0b8a4496-fed1-4cb0-b303-7980c2b3b1ea)


# Monitoring and Managing ICMP traffic with Azure and Wireshark.
In this tutorial, we observe various network traffic to and from Azure Virtual Machines with Wireshark as well as experiment with Network Security Groups. <br />




<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Various Command-Line Tools
- Network Protocol ICMP
- Wireshark (Protocol Analyzer)

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)
- Ubuntu Server 20.04


<h2>Actions and Observations</h2>

![image](https://github.com/user-attachments/assets/5a60790b-b54f-49bb-a34e-857066fdd660)

- Pinging our Ubuntu(linux) VM from the Windoes 10 VM.

![image](https://github.com/user-attachments/assets/fa44cd77-b72c-46e4-8235-a18f5b47b2b4)

- Filtering in Wireshark to Icmp to observe imcp Traffic.

![image](https://github.com/user-attachments/assets/658da4a9-fad2-4413-a38e-b58927bfb385)

- Observing the Traffic in wireshark.

![image](https://github.com/user-attachments/assets/3e8ef4f8-d54a-4ee7-8cfc-15da80da733a) ![image](https://github.com/user-attachments/assets/4ee7fd5b-16f5-4c26-b972-79750f86e92b)

- Using ping -t to start a perpetual ping  and and obsersving the traffic.

![image](https://github.com/user-attachments/assets/5d6882fc-e6d6-4343-82cb-616640958bea)

- Adding port rule on the Ubuntu(linux) VM to block ICMP traffic.

![image](https://github.com/user-attachments/assets/9eb0b03c-3884-4e0c-8dfd-15c78690748f)

- Observing how our perpetual ping has timed out due to the new port rule on the Ubuntu(linux) VM.

![image](https://github.com/user-attachments/assets/3eadc146-2eb2-4af9-b10a-e2b38153a622)

- Deleting our Port Rule that was denying ICMP traffic.

![image](https://github.com/user-attachments/assets/e15a7b1b-c943-4f0b-9d73-28fce6b6e2ef) ![image](https://github.com/user-attachments/assets/21a36add-7f83-4dca-a2f0-368d493f7bca)


- Ensuring that ICMP Traffic is being allowed from our Ubuntu(linux) VM and stopping the perpetual ping. 
