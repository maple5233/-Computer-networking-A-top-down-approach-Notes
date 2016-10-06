### Chapter 1 Review Questions

1. There is no difference. Throughout this text, the words “host” and “end system” are used interchangeably. End systems include PCs, workstations, Web servers, mail servers, PDAs, Internet-connected game consoles, etc.

2. From Wikipedia: Diplomatic protocol is commonly described as a set of international courtesy rules. These well-established and time-honored rules have made it easier for nations and people to live and work together. Part of protocol has always been the acknowledgment of the hierarchical standing of all present. Protocol rules are based on the principles of civility.

3. Standards are important for protocols so that people can create networking systems and products that interoperate.

4. 
	1. Dial-up modem over telephone line: home; 
	2. DSL over telephone line: home or small office; 
	3. Cable to HFC: home; 
	4. 100 Mbps switched Ethernet: enterprise; 
	5. Wifi (802.11):  home and enterprise: 
	6. 3G and 4G: wide-area wireless.

5. HFC bandwidth is shared among the users. On the downstream channel, all packets emanate from a single source, namely, the head end. Thus, there are no collisions in the downstream channel.

6. In most American cities, the current possibilities include: dial-up; DSL; cable modem; fiber-to-the-home.

7.  Ethernet LANs have transmission rates of 10 Mbps, 100 Mbps, 1 Gbps and 10 Gbps. 

8.  Today, Ethernet most commonly runs over twisted-pair copper wire. It also can run over fibers optic links.

9.  Dial up modems: up to 56 Kbps, bandwidth is dedicated; ADSL: up to 24 Mbps downstream and 2.5 Mbps upstream, bandwidth is dedicated; HFC, rates up to 42.8 Mbps and upstream rates of up to 30.7 Mbps, bandwidth is shared. FTTH: 2-10Mbps upload; 10-20 Mbps download; bandwidth is not shared.

10. There are two popular wireless Internet access technologies today:

	a) Wifi (802.11) In a wireless LAN, wireless users transmit/receive packets to/from an  base station  (i.e., wireless access point) within a radius of few tens of meters. The base station is typically connected to the wired Internet and thus serves to connect wireless users to the wired network.
	
	b)3G and 4G wide-area wireless access networks. 	In these systems, packets are transmitted over the same wireless infrastructure used for cellular telephony, with the base station thus being managed by a telecommunications provider. This provides wireless access to users within a 	radius of tens of kilometers of the base station.

11. At time t0 the sending host begins to transmit. At time t1 = L/R1, the sending host completes transmission and the entire packet is received at the router (no propagation delay). Because the router has the entire packet at time t1, it can begin to transmit the packet to the receiving host at time t1. At time t2 = t1 + L/R2, the router completes transmission and the entire packet is received at the receiving host (again, no propagation delay). Thus, the end-to-end delay is L/R1 + L/R2.

12.  A circuit-switched network can guarantee a certain amount of end-to-end bandwidth for the duration of a call. Most packet-switched networks today (including the Internet) cannot make any end-to-end guarantees for bandwidth. FDM requires sophisticated analog hardware to shift signal into appropriate frequency bands.

13. list:
	(a)	2 users can be supported because each user requires half of the link bandwidth.
    	
	(b)	Since each user requires 1Mbps when transmitting, if two or fewer users transmit 	simultaneously, a maximum of 2Mbps will be required. Since the available 	bandwidth of the shared link is 2Mbps, there will be no queuing delay before the 	link. Whereas, if three users 	transmit simultaneously, the bandwidth required 	will be 3Mbps which is more than the available bandwidth of the shared link. In 	this case, there will be queuing delay before the link.
	
	(c)	Probability that a given user is transmitting = 0.2
	
	(d)  Probability that all three users are transmitting simultaneously = 
	= (0.2)3 = 0.008. Since the queue grows when all the users are transmitting, the 	fraction of time during which the queue grows (which is equal to the probability 	that all three users are transmitting simultaneously) is 0.008. 

14. If the two ISPs do not peer with each other, then when they send traffic to each other they have to send the traffic through a provider ISP (intermediary), to which they have to pay for carrying the traffic. By peering with each other directly, the two ISPs can reduce their payments to their provider ISPs. An Internet Exchange Points (IXP)  (typically in a standalone building with its own switches) is a  meeting point where multiple ISPs can connect and/or peer together. An ISP earns its money by charging each of the the ISPs that connect to the IXP a relatively small fee, which may depend on the amount of traffic sent to or received from the IXP.

15. Google's private network connects together all its data centers, big and small. Traffic between the Google data centers passes over its private network rather than over the public Internet. Many of these data centers are located in, or close to, lower tier ISPs. Therefore, when Google delivers content to a user, it often can bypass higher tier ISPs. What motivates content providers to create these networks? First, the content provider has more control over the user experience, since it has to use few intermediary ISPs. Second, it can save money by sending less traffic into provider networks. Third, if ISPs decide to charge more money to highly profitable content providers  (in countries where net neutrality doesn't apply), the content providers can avoid these extra payments. 

16. The delay components are processing delays, transmission delays, propagation delays, and queuing delays. All of these delays are fixed, except for the queuing delays, which are variable.

17. a) 1000 km, 1 Mbps, 100 bytes
	b) 100 km, 1 Mbps, 100 bytes

18. 10msec; d/s; no; no

19. a) 500 kbps
	b) 64 seconds
	c) 100kbps; 320 seconds

20. End system A breaks the large file into chunks. It adds header to each chunk, thereby generating multiple packets from the file. The header in each packet includes the IP address of the destination (end system B). The packet switch uses the destination IP address in the packet to determine the outgoing link. Asking which road to take is analogous to a packet asking which outgoing link it should be forwarded on, given the packet’s destination address.

21. The maximum emission rate is 500 packets/sec and the maximum transmission rate is 
350 packets/sec. The corresponding traffic intensity is 500/350 =1.43 > 1. Loss will     eventually occur for each experiment; but the time when loss first occurs will be different from one experiment to the next due to the randomness in the emission process.

22. Five generic tasks are error control, flow control, segmentation and reassembly, multiplexing, and connection setup. Yes, these tasks can be duplicated at different layers. For example, error control is often provided at more than one layer.

23. The five layers in the Internet protocol stack are – from top to bottom – the application layer, the transport layer, the network layer, the link layer, and the physical layer. The principal responsibilities are outlined in Section 1.5.1.

24. Application-layer message: data which an application wants to send and passed onto the transport layer; transport-layer segment: generated by the transport layer and encapsulates application-layer message with transport layer header; network-layer datagram: encapsulates transport-layer segment with a network-layer header; link-layer frame: encapsulates network-layer datagram with a link-layer header.
 
25. Routers process network, link and physical layers (layers 1 through 3). (This is a little bit of a white lie, as modern routers sometimes act as firewalls or caching components, and process Transport layer as well.) Link layer switches process link and physical layers (layers 1 through2). Hosts process all five layers.

26. a) Virus 
	Requires some form of human interaction to spread. Classic example: E-mail     viruses.
	b) Worms
	No user replication needed. Worm in infected host scans IP addresses and port 	numbers, looking for vulnerable processes to infect.

27.  Creation of a botnet requires an attacker to find vulnerability in some application or system (e.g. exploiting the buffer overflow vulnerability that might exist in an application). After finding the vulnerability, the attacker needs to scan for hosts that are vulnerable. The target is basically to compromise a series of systems by exploiting that particular vulnerability.  Any system that is part of the botnet can automatically scan its environment and propagate by exploiting the vulnerability. An important property of such botnets is that the originator of the botnet can remotely control and issue commands to all the nodes in the botnet. Hence, it becomes possible for the attacker to issue a command to all the nodes, that target a single node (for example, all nodes in the botnet might be commanded by the attacker to send a TCP SYN message to the target, which might result in a TCP SYN flood attack at the target). 

28. Trudy can pretend to be Bob to Alice (and vice-versa) and partially or completely modify the message(s) being sent from Bob to Alice. For example, she can easily change the phrase “Alice, I owe you $1000” to “Alice, I owe you $10,000”. Furthermore, Trudy can even drop the packets that are being sent by Bob to Alice (and vise-versa), even if the packets from Bob to Alice are encrypted. 


## Chapter 1 Problems

+ Problem 1

	There is no single right answer to this question.  Many protocols would do the trick.  Here's a simple answer below:

	Messages from ATM machine to Server
	Msg name	purpose
	--------	-------
	HELO <userid>	Let server know that there is a card in the ATM machine
		ATM card transmits user ID to Server
	PASSWD <passwd>	User enters PIN, which is sent to server
	BALANCE	User requests balance
	WITHDRAWL <amount>	User asks to withdraw money
	BYE	user all done

	Messages from Server to ATM machine (display)
	Msg name	purpose
	--------	-------
	PASSWD	Ask user for PIN (password)
	OK	last requested operation (PASSWD, WITHDRAWL) OK
	ERR	last requested operation (PASSWD, WITHDRAWL) in ERROR
	AMOUNT <amt>	sent in response to BALANCE request
	BYE	user done, display welcome screen at ATM

	Correct operation:

	client                          server

	HELO (userid)	-------------->	(check if valid userid)
		<-------------	PASSWD
	PASSWD <passwd>	-------------->	(check password)
		<-------------	OK (password is OK)
	BALANCE	-------------->
		<-------------	AMOUNT <amt>
	WITHDRAWL <amt>	-------------->	check if enough $ to cover 				withdrawl
		<-------------	OK
	ATM dispenses $
	BYE	-------------->
		<-------------	BYE

	In situation when there's not enough money:

	HELO (userid)	-------------->	(check if valid userid)
		<-------------	PASSWD
	PASSWD <passwd>	-------------->	(check password)
		<-------------	OK (password is OK)
	BALANCE	-------------->
		<-------------	AMOUNT <amt>
	WITHDRAWL <amt>	-------------->	check if enough $ to cover withdrawl
		<-------------	ERR (not enough funds)
	error msg displayed
	no $ given out
	BYE	-------------->
				<-------------	BYE

+ Problem 2 
	At time N\*(L/R) the first packet has reached the destination, the second packet is stored in the last router, the third packet is stored in the next-to-last router, etc. At time N\*(L/R) + L/R, the second packet has reached the destination, the third packet is stored in the last router, etc. Continuing with this logic, we see that at time N\*(L/R) + (P-1)\*(L/R) = (N+P-1)*(L/R) all packets have reached the destination. 

+ Problem 3 

	a) A circuit-switched network would be well suited to the application, because the application involves long sessions with predictable smooth bandwidth requirements. Since the transmission rate is known and not bursty, bandwidth can be reserved for each application session without significant waste. In addition, the overhead costs of setting up and tearing down connections are amortized over the lengthy duration of a typical application session.

	b) In the worst case, all the applications simultaneously transmit over one or more network links. However, since each link has sufficient bandwidth to handle the sum of all of the applications' data rates, no congestion (very little queuing) will occur. Given such generous link capacities, the network does not need congestion control mechanisms.



+ Problem 4

	a)Between the switch in the upper left and the switch in the upper right we can have 4 connections. Similarly we can have four connections between each of the 3 other pairs of adjacent switches. Thus, this network can support up to 16 connections. 

	b)We can 4 connections passing through the switch in the upper-right-hand corner and another 4 connections passing through the switch in the lower-left-hand corner, giving a total of 8 connections. 
	c)Yes. For the connections between A and C, we route two connections through B and two connections through D. For the connections between B and D, we route two connections through A and two connections through C. In this manner, there are at most 4 connections passing through any link. 



+ Problem 5

	Tollbooths are 75 km apart, and the cars propagate at 100km/hr. A tollbooth services a car at a rate of one car every 12 seconds.

	a) There are ten cars. It takes 120 seconds, or 2 minutes, for the first tollbooth to service the 10 cars. Each of these cars has a propagation delay of 45 minutes (travel 75 km) before arriving at the second tollbooth. Thus, all the cars are lined up before the second tollbooth after 47 minutes. The whole process repeats itself for traveling between the second and third tollbooths. It also takes 2 minutes for the third tollbooth to service the 10 cars. Thus the total delay is 96 minutes.
	 
	b) Delay between tollbooths is 8\*12 seconds plus 45 minutes, i.e., 46 minutes and 36 seconds. The total delay is twice this amount plus 8\*12 seconds, i.e., 94 minutes and 48 seconds.  

+ Problem 6-31
	(See Solutions6thEdition.doc)