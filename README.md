# test_sample
sample testing github


Problem:
Cannot see own wireless network but can see others around me

Every other device can detect my wifi but not my laptop. 
Seemingly after last Windows update (though I'm not sure) I cannot see my own wireless network on my home laptop. I can see all the networks of my neighbors, but not my own.

I can see it and connect to my wireless network with my Work laptop. My partner can see it and connect to it with her two laptops and her smartphone.

I checked the wireless network adapter (Realtek RTL8723AE Wireless LAN 802.11n PCI-E NIC) 

** Solve wifi issues **:

Best thing is to:
 1) To me the answer is get a new wireless card or a** USB wireless connector**.  or USB Wi-Fi Adapter
 
1) https://askubuntu.com/questions/721981/how-to-configure-rtl8723be-to-detect-wifi-networks-solved-for-hp-laptop

2) https://l.facebook.com/l.php?u=https%3A%2F%2Fanswers.microsoft.com%2Fen-us%2Fwindows%2Fforum%2Fall%2Fcannot-see-own-wireless-network-but-can-see-others%2Fae835a08-59a6-4aaa-830c-87a1dab5761b%3Fpage%3D5%26fbclid%3DIwAR1zHSgwkGOxL4UZ-dLZSPxb3VpDEQIsMP04ILBJrfzL5c5XCZVuFgJMeXc&h=AT0mCk6nl3Y4SX2D9d82qJ8huTw9ZE_wrepG_zGec5DnrjuaWUwo8PrtO1iK3GTwhM08B8NUe_Bk76FdrISfjeCD_XR-cv02vMImF1gxq1cBAHZFxQRKtgIt7Y1m_lQhShY4Xg


3) I turned on 802-11d and "lo
4) I turned on 802.11d in the network adapter.
5) I had this same issue and wanted to share my experience with a Lenovo IdeaPad Yoga 13 model 20175 and the Realtek Semiconductor Corp. RTL8723AU 802.11n WLAN Adapter. After trying all of the troubleshooting steps in this thread, I can confirm this issue to be driver related as installing Linux on the same hardware does allow finding and connecting to my home network.
6) I had exactly the same problem.It was solved when I changed the settings of the router. Specifically, I tried different "Wireless Modes" (f.x. 802.11b or 802.11b+g+n and so on) until I found one all my computers could see.Hope it helps.
7)  Easier fix.  Reboot router!
8)  Just resolved it. Just go to your router and at your 2.4 connection set the wi-fi mode to  **Mixed 802.11 b/n/g**
9)  I got thinking about this logically and my system said that the Wifi Adapter was working correctly and there were no updates for the drivers. So I thought to myself what controls this? 
This is the Realtek PCle GbE Family Controller.  I got mine to work by opening **Device Manager > Realtek PCle GbE Family Controller > Properties > Advanced > Power Saving Mode** ..  The Power Saving Mode was showing as Enabled... as soon as I made the value to **Disabled**(i.e., not in power saving mode) my wifi internet connection icon changed and it was online once more... So, it was the **Realtek PCle GbE Family Controller** that was stopping the Ralink 802.11n Wireless Lan Card being seen because of the power saving option in the controller... As such it could not connect to the internet.
10) Hi, I had exactly the same problem. I solved it by going in to my router (login as admin) and changed the wireless mode from 802.11ax to to another one such as **802.11b+g+n**


