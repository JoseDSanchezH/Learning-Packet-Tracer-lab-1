# Learning-Packet-Tracer-lab-1


In a previous project I worked on in My Portfolio, not my GitHub, I installed package tracer to learn more about networking with Cisco systems. I still want to get my CCNA in the future, but for now, I'm going to just learn Packet Tracer and do some labs and projects to get familiarized with different topologies.

# Let's build a basic connection
In Cisco packing tracer, there is a lot of drag and drop for either PCs, network devices, components, connections, miscellaneous, and multi user connections. 

1. I will add 2 PCs, which are under end devices, and then connect a switch to those two PCs.

<img width="1713" height="1078" alt="image" src="https://github.com/user-attachments/assets/7c5aa47a-20e7-4ed0-a327-e15e18616ca8" />


2. I will select the connections icon, and I will select the copper crossover cable to connect the PC to the switch, which I will then right-click on FastEthernet0. 

<img width="1384" height="860" alt="image" src="https://github.com/user-attachments/assets/276b2596-468a-4d01-b685-3140bfac4c4b" />


<img width="232" height="184" alt="image" src="https://github.com/user-attachments/assets/11fe3572-a8fa-49a1-841c-ad6fe5e24648" />


3. Then I will select the switch and select FastEthernet0/1.

<img width="572" height="178" alt="image" src="https://github.com/user-attachments/assets/298f2bf3-1eb6-4a84-a456-a1a9dd0d5be1" />

<img width="342" height="284" alt="image" src="https://github.com/user-attachments/assets/87cb1c46-b9cc-4bc2-bfd2-ce74fcdc6893" />

4. I will do the same with the second computer, and we will have both devices connected to the switch.

<img width="502" height="286" alt="image" src="https://github.com/user-attachments/assets/f2199a04-1ea5-4c7e-bb99-479dc7218147" />

5. Let's configure our first computer. I will make sure the computer is on and then head over to the Desktop tab and select the IP Configuration setting. 

<img width="1314" height="676" alt="image" src="https://github.com/user-attachments/assets/e4f8ddd9-c8f2-4a07-8b3d-f2db9940e2d1" />

<img width="408" height="286" alt="image" src="https://github.com/user-attachments/assets/9934de99-1c75-4263-9aff-3165ef9a1905" />

6. We're going to be adding an IP address to this computer because an IP address is like a home address. If someone wants to send a letter to me they need to know where I live. Computers work the same way, so if a computer talks to another and needs to know its actual address within the network.
I will input 192.168.0.1 because this address is in the private IP range. Meaning the standard address range for local users like my home or office, is recognized and used as a safe range for internal communication. I am setting it up manually as static because I am assigning it to my own network.

Right now, I don't have a router or a DHCP server in my lab, so I will only use a static range.

<img width="1093" height="552" alt="image" src="https://github.com/user-attachments/assets/f42b9c55-c145-4055-b949-3f5b48715e53" />


7. I will do the same with the second computer, but this time set the IP Address to 192.168.0.2.

<img width="822" height="704" alt="image" src="https://github.com/user-attachments/assets/c89f44bd-7838-497a-8daf-239b61282427" />


8. Let me simulate our mini lab by filtering for the ICMP.
 ICMP stands for Internet Control Message Protocol. I would think of it as a walkie-talkie call. Imagine you and a friend have walkie-talkies, and before you start sending messages to each other, you press the button and say, " Hey, can you hear me?" and the friend replies, "Yes, I can hear you loud and clear." That's basically ICMP. Computers do the same thing before sending data. One computer can say hey are you there? Can we communicate, and the other computer will reply, "Yes, I'm here," which is the back-and-forth check.


On the right-hand side, I will click on simultaneous and select "edit filters."

<img width="384" height="864" alt="image" src="https://github.com/user-attachments/assets/abf48ec8-dc8c-4714-95bf-0427635e6cb0" />


9. I will select ICMP and then close the window. 


<img width="434" height="556" alt="image" src="https://github.com/user-attachments/assets/3e743e04-24d3-4186-8b1a-7ca5a26ae5ff" />

10. I will then click on our first computer and head over to the Command Prompt. 

<img width="864" height="582" alt="image" src="https://github.com/user-attachments/assets/41de3a16-cbff-40d7-94da-2f4236716962" />

11. I typed in "ping 192.168.0.2" and pressed enter. I can now see the envelope travel through the network to ping the second computer.

<img width="1144" height="658" alt="image" src="https://github.com/user-attachments/assets/980cffbc-03f2-4b7d-8f2b-46e02c36deb3" />


12. I can now hit the play button over at the Simulation panel and simulate what happens. 


<img width="1409" height="832" alt="image" src="https://github.com/user-attachments/assets/d66c798e-0de9-44e4-bec8-984127584a9d" />

<img width="826" height="320" alt="image" src="https://github.com/user-attachments/assets/4502a0c0-4bcb-4269-a644-2f7c4dda516a" />

<img width="680" height="288" alt="image" src="https://github.com/user-attachments/assets/04003cc8-312e-412a-a745-f97e5d557427" />


<img width="840" height="410" alt="image" src="https://github.com/user-attachments/assets/6b4a0473-f000-44f1-bc5f-c26ac7fa930b" />


We can see that PC1 replies to PC0, saying, "Yes, I am here." 


This is just the beginning, though I want to keep building on this and exploring more complex setups and different topologies. One thing I'm really looking forward to is intentionally breaking things and misconfiguring IP addresses, maybe adding different subnets to see what goes wrong, and then figuring it out or troubleshooting it. My goal is to eventually get my CCNA, but right now, I'm just focusing on building these labs and learning different topologies and getting comfortable with everything and how it works.

