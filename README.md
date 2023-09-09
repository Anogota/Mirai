1.What is the name of the service running on TCP port 53 on Mirai? Don't include a version number.
Nmap results:

![obraz](https://github.com/Anogota/Mirai/assets/143951834/b7a17948-469e-4e24-9c78-058763355711)

that how you can see, the version of port 53 is dnsmasq, i don't know exacly what is this but i hope in this lab i will learn more about it :P

2.What unusual HTTP header is included in the response when visiting the service on port 80?
To find this unusual HTTP header is used a burp proxy, first intercept the trafic then small check, what's going on with this headers, but i found something intresting, here it is:
This also doesn't tell me anything but we will figure out.

![obraz](https://github.com/Anogota/Mirai/assets/143951834/228763d5-cbc2-4010-90bc-13f33859e7ba)

3.What relative path on the webserver presents the Pi-hole dashboard?
If you don't know something, try to search it on google i found answer for this question in documentation Pi-Hole
The answer is /admin, this is as dashboard

![obraz](https://github.com/Anogota/Mirai/assets/143951834/c8c3691f-f784-4fcd-98a2-c631be620ab1)

4.What was the default username on a Raspberry Pi device?
Still we need to find it on google, let's search it, this is also quick to find, in first link i found what i want, here is the result:

![obraz](https://github.com/Anogota/Mirai/assets/143951834/7f80383f-65ec-4666-a0ef-68c2ce27f24f)

5.What is the default password for the pi user?
Also this we can find in first pretty easy, check the screan shot, from the previous one task 

6.Submit the flag located on the pi user's desktop.
If you correctly read scan, you can see there some SSH, i got username and password and i tried use this in SSH, and we got this.

![obraz](https://github.com/Anogota/Mirai/assets/143951834/79cbd7c8-de34-42f7-b1aa-d5b5a84b14b0)

7.Can the pi user run any command as root on Mirai?
We can check this by command: sudo -l and we can run root, sudo su 

![obraz](https://github.com/Anogota/Mirai/assets/143951834/18c1e754-7c8e-418d-b1c5-c4a5c7065bf0)

8.The flag-less root.txt file mentions that it's on the USB stick. What is the mountpoint for a device that is labeled as a USB stick on this host?
We check this by command mount, there is many lines of code, but is very easy to find this path:

![obraz](https://github.com/Anogota/Mirai/assets/143951834/70f505a3-e1ee-45cb-9586-7b85819493a0)

9. What is the full path to the device that represents the raw USB media on Mirai?
On the screan shot looking above, before this path we can see the full path to the device that respresents the rwa USB media on Mirai.

![obraz](https://github.com/Anogota/Mirai/assets/143951834/22b8dfc7-a58e-4385-9b8b-84b9c66aa1ee)

10.When files are deleted from a drive, is the memory definitely immediately overwritten with something else?

![obraz](https://github.com/Anogota/Mirai/assets/143951834/d66a9d0b-1b44-467f-ab2b-6183a8cddd7c)

Submit the flag located on the USB device.
We can see the flag above 

This machine was very easy :P
