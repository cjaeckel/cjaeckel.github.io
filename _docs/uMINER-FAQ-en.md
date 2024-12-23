---
permalink: /docs/uMINER/
title: "CRYPTO μMINER FAQ"
layout: single
toc_sticky: true
sidebar:
	nav: "docs"

---

# **CRYPTO μMINER FAQ**

**CONTROLS**

## A. WTF \- what is this for?

Apart from the fact that crazy gadgets are of course completely legitimate, here are a few ideas as suggested use cases:  
(Terms marked with 👁‍🗨 are best looked up on Google...)

1. **CLOCK WITH DATE**  
   If you switch to screen \#2, you have a great time display.  
   (The time display is very accurate and is automatically updated via *Network Time Protocol (NTP) 👁‍🗨.)*  
2. **MINING RIG** 👁‍🗨  
	 Like the gold prospectors in the wilderness of old, you can become *rich* and *famous* as a modern digital Bitcoins miner \!  
	 All you need is Wi-Fi, very little power and a lot of luck… (If you manage to verify a new transaction block of the global Bitcoin *blockchain 👁‍🗨 with the* **CRYPTO μMINER** , you will currently receive the following as a reward:

   >**3,125 BTC**  
	 (Screen \#3 shows you the price at which a single Bitcoin is currently being traded…)

1. **Mobile Device**  
   If you want to be really cool, connect the **CRYPTO μMINER** to a power bank or your smartphone using a USB cable. If you then set up a hotspot, you have a mobile **CRYPTO μMINER** that you can show all your friends everywhere...

2. **Competition**  
   In exchange with other **CRYPTO μMINER** owners you can compare all kinds of high scores: Who has the longest *up-time* , the most *shares or the highest difficulty* achieved ...

3. **Insight**  
   You can also use this little piece as an opportunity to delve deeper into the cyber world of the Internet and the completely decentralized digital money (also called *cryptocurrency* 👁‍🗨) in order to better understand how it all works and how it is actually programmed. Yes, you can do it yourself\! (see below).

## B. What's in there?

In the small plastic box (which you could have made with a 3D printer if you only had one 😢) there is of course a *small* computer, so the

### **HARDWARE**

| CPU (microcontroller) | ESP32-S3R8 32 bit Dual-core LX7 @240MHz |
| :---- 								| :---- |
| Wi-Fi 								| 802.11 |
| Bluetooth (unused) 		| BLE 5 \+ BT mesh |
| RAM 									| 8 Mbyte |
| Flash 								| 16 Mbyte |
| Display 							| TFT 170x320 (H)RGB |
| Interface 						| USB, 16 GPIO, <br/> Reset \+ 2xButton |
| Power 								| 3.3V \< 180mA |

Well, so far so cute today. \- But just for comparison:

* In 1980, my first computer had an **8 bit MOS 6502 CPU with 1 MHz** (just like the `Apple II`),
  1 kB RAM, 1 kB ROM and a 6-digit 7-segment display.  
* In 1985 my first car had less than 50 hp

If the *v8 steam diesel* technology in cars had developed the way it did with the **CRYPTO μMINER** ,
then a small car would easily have 50,000 hp and would be so cheap that some people would order it from China and give it as a Christmas present...

In addition, completely invisible from the outside, the flash memory contains about 1.8 Mbyte of something called:

### **SOFTWARE**

And I made some of it myself.  
(The majority of the software is based on components that others have already made at some point
and that I then found and put together.)

| 		|  	|
| :--- | :--- |
| <ul><li>Real-time multitasking core</li><li>network stack: WiFi, TCP-IP, HTTP, Stratum</li><li>Web server for configuration via WiFi access point</li><li>Graphics library for the display</li><li>Crypto library for the mining functions</li></ul> | The whole thing (including my part) can be found on the Internet as open source software 👁‍🗨 <br/>Well, there really is a lot more than dancing influencers and cat videos… |
|![][image1] | ![][image2] https://github.com/cjaeckel/uMiner |

## B. What exactly is in the screens?

### SCREEN \#1

The first screen (yellow border) shows your current progress and your achievements in the Bitcoin search:

1. BLOCK TEMPLATES  
   This is the number of search tasks from the Bitcoin network that have been processed so far.  
   (The task basically consists of looking for a tiny needle in a huge intergalactic haystack. Whoever finds it first can use it to verify a transaction block in the blockchain and receives the reward.)  
   In principle, there are two strategies for success in the search:  
   1. To search really quickly with a lot of electrical energy and computer power.  
   2. Just be super lucky\!  
2. BEST DIFFICULTY  
   Okay, the search task is a bit more complicated. In the haystack of intergalactic size, needles of different sizes can be found. The maximum needle size that has to be found is constantly adjusted by the Bitcoin network to the computing capacity in the network. (In the world of computers, this doubles every two years, not like with *v8 steam diesel* engines...)  
   The smaller the needle size, the higher the DIFFICULTY. (See also SCREEN \#3)  
   The value shown here corresponds to the smallest needle that your **CRYPTO μMINER** has found so far.  
3. 32 BIT SHARES  
   The number of needles that your **CRYPTO μMINER** has found that are so small that they would have been considered a solution at the beginning of the Bitcoin network (around 2008).  
   (Which corresponds to a DIFFICULTY \> 1...)  
4. VALID BLOCKS  
   This always shows 0\. (Unless you win.)  
5. TOTAL MILLION HASHES  
   A hash is like reaching into a haystack.  
6. UP TIME  
   The time in days, hours, minutes and seconds since the last start of the **CRYPTO μMINER.**  
7. HASHRATE  
   The current number of searches in the haystack per second.  
   This number varies depending on the computing power that the **CRYPTO μMINER** has to divert to other tasks such as network communication or screen display. (Sometimes the supply of new search tasks can also be a little slow...)

### SCREEN \#2

Here you can see how time passes, which is synchronized with the internet with great precision.  
(Of course, we always keep an eye on the fact that crypto mining continues to run in the background...)

### SCREEN \#3

On this screen you can get an overview of important parameters of the global Bitcoin network.

1. BTC PRICE  
   If you ever had Bitcoins and actually wanted to exchange them for plain old money, this number corresponds to the current trading value of one Bitcoin in USD.  
2. BLOCK REWARD  
   The amount of the reward in Bitcoins for a solution that would verify a block of transactions.  
3. DIFFICULTY  
   The DIFFICULTY currently specified in the network for the search tasks.  
   (A numerical value with T (Tera) at the end corresponds to a factor of 10^12 \- so quite large, or quite difficult. Mega, i.e. 10^6, would be less difficult...) The numerical value is therefore given with so-called *Metric SI prefixes* 👁‍🗨  
   for better readability .  
4. CURRENT BLOCK  
   All transaction blocks verified in the blockchain are numbered. This is the number of the last one. This number should be increased by one approximately every 10 minutes.  
5. REMAINING  
   The number of blocks remaining until the reward for a successful block verification is halved. (See *Bitcoin Halving* 👁‍🗨)  
6. GLOBAL HASHRATE  
   The current number of search attempts by all mining computers in the global Bitcoin network in a single second.  
   (Okay, again SI prefixed. Here with E, i.e. EH/s, i.e. *Exa* , i.e. factor 10^18 😨- our **CRYPTO μMINER** just manages 80 kH/s, i.e. factor 10^3 \- but we're just relying on a lot more luck\!

### SCREEN \#4

This screen provides information about further status parameters of the **CRYPTO μMINER.**

1. NTP UPDATE  
   Time at which the time was last synchronized with the network. (Synchronization currently occurs every 5 hours.)  
2. POOL  
   TCP/IP network address of the mining pool from which the **CRYPTO μMINER** obtains its search tasks.  
3. NAME  
   Pool registration name. Is sometimes listed in pool statistics…  
4. SESSION  
   Pool Session ID (assigned via Stratum Protocol)  
5. BEST DIFF Best solution DIFFICULTY reported  
   by your **CRYPTO μMINER to the pool so far.**  
6. CPU & POWER  
   If you do a lot of calculations, your head can get hot. Anything under 70° is OK. (Turning off the backlight will help cool it down.)  
   The voltage is an indicator of the quality of the USB cable. (The closer to 5V, the better...)  

## D. Any Tips & Tricks?

1. ALWAYS ON  
   Keep the **CRYPTO μMINER** switched on as often as possible. This increases your chance of winning.  
   The power consumption is so low (approx. 170 mA at 5V corresponds to less than one watt) that it shouldn't play a role.  
2. ABSENCE  
   Turn off the display backlight when you leave the **CRYPTO μMINER** alone.  
   Without the otherwise necessary screen update, the hashrate increases and you also keep the CPU temperature low.  
3. DARK ENVIRONMENT  
    Dim the display brightness down to avoid being blinded by the maximum bright display.  
4. BUTTON CUSTOMIZING  
    Depending on whether you prefer the USB connection on the left or right, you can rotate the display by 180° by double-clicking on the display button. It is best to add a *custom*  
    marking to one of the buttons (eg with a permanent marker) so that the buttons are not confused.


## E. How to start the setup of the **CRYPTO μMINER**?

To connect to the Bitcoin network, the **CRYPTO μMINER** needs:

* The access data for a Wi-Fi network  
* A so-called Bitcoin address to be used for possible rewards booking.

If the connection to a Wi-Fi network fails, the **CRYPTO μMINER** will automatically switch to the `“CONNECTING”` screen
(which also has a QR code on the right).  
In this state, a Wi-Fi access point called **`uMINER`** will be opened, which can be used to connect to another computer for configuration.  
(Your smartphone, for example, is a handy computer, and its camera is also good for reading the QR code…)

After connecting to the **`uMINER`** Access Point, the **CRYPTO μMINER** Setup Portal page will appear on your computer.  
With the `“Wifi Setup”` button you can now

* Configure the access data for a Wi-Fi network (SSID and password)  
* Adjust your mining pool data.  

## F. Where are my Bitcoins?**

As soon as your **CRYPTO μMINER** has verified a transaction block in the blockchain,
your reward will be transferred to your Bitcoin address. (I.e. a corresponding entry will be stored in the global blockchain.)

You can view the transactions to any (or even **your** ) Bitcoin address at any time in the network:

![][image3] https://mempool.space/

If you not only want to enjoy your winning Bitcoins, but also want to spend them again, it will be necessary for you to set up a digital cryptocurrency wallet.

## G. How do cryptocurrencies work?

A very good question, but unfortunately also very difficult to answer.  
As a starting point, the following is recommended as further reading:

| ![][image4]https://en.wikipedia.org/wiki/Bitcoin\_protocol | ![][image5]https://en.bitcoin.it/wiki/Difficulty |
| :---- | :---- |
| ![][image6]https://en.bitcoin.it/wiki/Block\_hashing\_algorithm | ![][image7]https://learnmeabitcoin.com/technical/block/hash/ |

[image1]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAGgAAABpCAYAAADWQGYEAAAAAXNSR0IArs4c6QAACsFJREFUeF7tXTF6FD0MnfSU9EAfzgAcgIoDAAeg4gDAAag4AHAAKg4A9HShh/Qp6eHX5vP+L2/nad9qvMmSeCrI2h6N3kiW5SfP0cnJyZ9pXAergaMB0MFisxJsAHTY+AyADhyfAdAA6NA1cODybcxB9+/f34vId+/enX7+/Dk79ps3b6bXr1+vfnv48OH05cuXdbujo6Ot8mRjP3/+fPrw4cNOY4csr169mr3vvXv3pl+/fm2VqdLg5ORko9sAaEaTAyBSyrCgc4XsbEHxJj148KBiras+3759W7uuqov7+vXr7P157Bh/7nr69OmEv8XL0C4cG581xm6/Rd/379+v+6CLW6qfcJXhgtu1M0AxF8ScUL3C9zcBqgCpe+PYmXyh3GfPnq2ahNIfPXo02xyfNbNoBAjHruiI5RkAXWeAAu0w/W0XuhTXgpaOHTK1KJDlCzfSXFz8u0V03AflRnnu3LmztsDooyzIfYaYMppX6mpBaPauS3EBwvFcN+SOjWE2y/3nz+55YgWQ63IxQhwATdNqDkSrQZAGQGaQgAu/eKsw0sLfcCJnC8LFLYLw8eNHCZDqoyLCzMVdawty10EKINflcjuVpXAXqhjFDYCmaZUCahOsq5AsFB4AmS5uWNC5bS9aB+0zisN5hv0/vuWuBUW7Ng7OQfE3lYgNS2vWOeagbYsp+L0CUGTNm5LdbLabNbnxYXY2kbsWdCMBivDX2QcJN9He3mwxGb+1zESsrlu+LO6BYTYma1ubADELEhAglhuzIZwInsuUxLPg3pCyoJBbJXbxpUP9dF2o7uCV1k0zgCJp2R4oW12rxaQLUJalwLFRHlYozls3Jlk6ANrMru8cxcWbHcnC6hUuo6VZeLuhAhC6q9PT0wsuF9M5ysWxC0MXh7+hu+IteLSgcLlL98tQ7p0BqgIz168HQAhqKKdtpIVCQ3HtWhokuPtBPfVTWgf1FGAAtF2blgU9fvx4+0iFFrxIjPVJCxLCjbRIiZOlyATiPo4FhTUgq4cjsvYouFBFGUI23PIOK3ai2YKKps+fP29022D1HB8fV8Ze1CdzKc7AmYvLojg1dpYsdeSptvnx48cASHESUDMDIHpPhgWdK8SyoBcvXqzVF/5asXrwTQwf3bIHoWy1osYFH7aLe2C4ipkExFLJEy4O54VIkKp5QjFGUR60IKZGqWfFeXSvLg6pvyqB6Ia1KGg1isMxKglN7M9rGvzNXZepEB7D/gHQFg0o/vS1BghpRUhlCl0pyhLqkelLEfpGNiCujIqk6FTYJ8ZAtxhjNxcXb3ZzvywDyofyZPjjs8d47Rl4bJRHudUYK9xxu548ebI9ilMuDifyjCVaNe/WjzO8KqGZZRJQhgr7080kqLGrYb+1UB0AnVujKodxstmXBhBGLLx1jCt8Zx+ELSuscG5rObOgyCQ014VRE0daWeTnyIrkeY4wMULEqBIjySzyQ9nwPvH3d+/e7ebilLtiF1cpalIRWQZQb/epxsv2pzCK4zkMKxUcWTlosdZBToXdAGiz1MWlgWVh/wAoqW5Axf2TFlRhW+JD88SpFJK5hsp+UDaeYgxVUk/Z9r67LltkQQOgfFYZAP1XUjksaJomFSS4FqTCZ05o4vuIfbgmFNtlAGFyVCV4OfzFFT724UW5YpqqMDvaY0SHmRZeruDYi8JsFyAnvMzauPmySnLSDeErNOdsvsXQPBt750yCO5FX1kEKpAHQRc1sbHm/fft2VndML0KWpwIozBddB1KMkGGZ0ZywD7NCUQbHcjMLQkpXuCGVccB7huuac6fMjg1XiGxbVev78uXL7ZkExUnIkqUKoCyh6Za9q1DYAYTbuInYbGyVSajIw32sMHsAlKv6ygG6devWrIRIRWIKFVKROJpCahRuk2cWxDSnJhBGTVkNj1LxtkRsc2u8XY73wgRyD6vBMX7//r3dxVXCbBw1q6rGdgogltDZD3IVVYniMuqve1+33d6iuAGQC0HebgBEyVJV2uJu2PWB5f9RFgHk+nw1B/HD4HjZ4g3bZbWsjrK2zS0tZOaIlReh7f+xeI9Qe+5CMj/XzLbdWp7LF81BjgK4jbvad1fuFRncPu6ciONVOAmZdVphtrNh5z70AOhcUyrVU9pR/f79+1r/uKKOwZQ5x1sxx+TkTAICi6twdimKpoT9sTiMXxhVeBYUKaRxYTiPGQJXHiwi4zpbzESosUsA4UJVsS1ZIZVcnJtJUNbau0YV7+Nu2OGSouItBkCEbo91kFpS/DMAqf0gtgR0YxnNCfvh2FzoxZN3i/5wHwrPOY32bpjtEO4ZIHRxnDBubFKmdN2+fXvDYaQFXBUX5zI5XbI6SuyS59Vbzk/vAFQJiPZKXFw6Bw2AplXApIqaEfDSQRYDoIvU34OzoKXc7MtKlvLcpD47kB2m5Cif33JVH+TK03XLW4XCWXXDAGha7Z4636ngF2TnXNwAaPO4liu3oLOzszWwGB5iuMqhNFYdYLusblPRnLJIC0NX97MDTPfCwip1qGwsglsozP2vHKDKOQkOJyHz95lfdk67cgvKKgtVlnsARBoZANFnOj99+rRWkVN7Go2xVhP1y7WsTtQUfZzj+7G+U93fud9cm7C0jHbVshSqHVu0OlaA792tRjUze/zNrZnJyj2cTEJWOYH9OTnpfN2rAnJWP5UxdHfeD3I3sZZWnQ2Azl8DCyA8aQQpRhjZ8FulqEhZQhOjo0g0tr0mTmjivdR9uJyd3SzWtWLkhjSwjNyvyPjqPpkF4bOyHndOllbM2+2jzgh1+7srdzeT4J5ZquSr1AeVFqqVMLui1AHQptasTMIA6KLismoLFRBVi6wtgPZ14mI8DOan5jgMc5aIaXs+FRG/j8fRXguF0cUxdUzJE1kEdZAF0pxjI6/xDTIXh8+KY1857cqdJzIX2fPTAHwfZ8Muo/6qz9O4ydISJ6En7WoAtPnqdeXF9TwXmt8q/DQAA4kcAP68WSt+wqKv6I8UKqRDxX3V2d9YSKVoYPyWqyI0dnEqNMdCMaalWQVczoF+btTmfhogW+3jbyryyyZl9wNP+6SBufqygoQBUH7albMOcgEprYMUQOxSlBBYe5pZkGKjZrWwaEHoHtiN4diZm0YXh3WkPE8oRi3qgJmubv3sok8DuLk4FLQS2WB/t47UPdAve5udKK5iDdX9qUUuzq1AGADlnITsZTwogFStzxyLpj1U9mkATHxmtUx4X0XswMVk3FvVKCnr4gWoasfJZOvTAA7tKjN714IqzFLX3ajtDwbfGW+fNaqLF6r7nIMGQNPqEAzc/rD2g4YFXbSrG2tBOBegL3aTqKE4zB5wNmLOfbnzW7ZwVvLF2M6ZpRF9YqYE586DmoNQCW6EiH3cepxKCO9mNrBdD/7FQUVxA6AOHxnEICFMWJ3ShMrGI/uzTIICKEJUXIVjTSke89+b0oWfE2B3ifKoYi62IPVJgyxyXES7ckJSblMBKKNGuV8irsjq9nEYTJe2H1SpaFN+uSp0ZcPOVXal3UEBtPRkp4zgjjQnPMczsyCUJ6NnsYvKMgtzIGUULKUTflaMMFWhwOJ1UOUNy9IfmFpxaU5L2Z9uSebSoCXTVdeDLC5ry3sA1CGTMCyojwa6WlAfkcYovTSwcU5Cr4HHOH00MADqo8e9jTIA2ptq+wz8F/GcRLB4iUbmAAAAAElFTkSuQmCC>

[image2]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAEYAAABGCAYAAABxLuKEAAAAAXNSR0IArs4c6QAABYtJREFUeF7tml1MFFcUx/98JJCQwEtVyocrLrQPaqgPgIbUkEiT2kL4qIlp0UJBW4TYCLXCNgpCa2kfyvZBKWBBbdRUYpNSKLhYw1OlsKE+UBNaJIK2SLQvfNlACDSXZMkKM3vPnbmzuw8zb+z87zn/87vn3p25bMDy8vIyzGsdgQATjHJXmGBUVosJxgQjtpGaHWN2jNkxYgTMjhHj5dM95kx1NZoaG6H0jFl0+DA+O3sWAQEBYhVJUnsVzIubNilCoNYy+eQJVapbZziYwoICdHV16TbqHiAtLQ3ft7VJjbk2mGFgcrKz0XfnjqHmExMT4bh1y5Ac0sH89+wZ4rZsMcSsWtA/R0YQEREhNadUMAlWK2ZmZqQapAYLDQ3F2MOHVDlXJw1M5MaN3GTeEMjaoKWA8RcoLvAy4OgG429QZMHRBcZfociAoxmMv0PRC0cTmEsXL6KyokJ1L3Wt8ZGREbyammrInnvT4cArO3euxPY0SR+fPImPTpwQ9qAJDK9blDY/3hiqcy2xtWzGwmB4BW62WDDgdKrW6Rrf2NSE7JwcjzxudnejID9/RTMxOYnAwEBFff6hQ3A4HB5jicKRDqbebsc7eXnUBpCi+31wEG/s2+c7MLxuYc4uXb6M1zkmpdBwCzI2NoZdycncsCJdI9QxFDA5OTn4pqmJa1Km4Gu7HV/U1XFDGgLm5YQETE1NcZMzgYgBUkCOiDJhLERISAjGHz0ipSR3DDW5L8BsjonBwsICqWDqpEkHQ01MqkJARJ04qj8SGPYwxx7qeNfg3buIjo7myQy5v7S0hKjISG7st/bvx/mGBq6OBEb2bHBdaRTI9CkNTFBQEP55/FhjSXKGpe3Zg+HhYW4wynKSBuaX27exfccOrikjBYuLi4iJiuKm8CoYSjKuYwkCynKieJXWMZRkEurmhjDBqCDyOzDshJ6d1Pv68jswJaWlqKqu9imXtuvX8eGxY1wPlGUvbY/xxavAWgKUbqH6NMGo9JcJRg8Ya1wc5ubmuGuX2qakQIIi6jIKCwvD6IMH3Oikjpmfn4clNpYbjAlYUpbcmxf1BZJ5Yucx7FyGd5HAsCDUGfFF1xjhzRAw3oQjAkXEFxnMv0+fYvu2bbwOfO5+UnIyOjo7hcZQxZkZGXAODFDlK7o/7t3DCxs2kMaQwagtJ9fDUk9PD949eFAxaXBwMP6emCAZ4onYYRTbU7RclAc7V1whMOwknp3Iu1/FR4/iTE3N6kfU1qaapMbjgTpeXo7KykqebPW+EBhPm7B7obxiRN6rRL5xPFVNnQhNHcMGjY6OInX37nUeYmNj4RwcXPn87QMH0Nvbq+pT1CQPNK8Nfu3rg9Vq5cmeuy/cMdSueW3vXgwNDSmaEQUTv3UrZmdnhQpzF4vmY2M1gVGDo/RUWXX6NL69cAHp6en47soVTcU1Nzej6tQpTWO1QNEFRg2OViOequ7u6sJ7BQXCYPR40dwxzOVvfX3IzspaZ1iPIaXqf+7sRFFhoRCYH9vbsUthL6QG0QWGJWltacEnNtu6fCL/J+aZ/am9He8fOcKTrd7/vK4OhUVFZL2SUDcYFrS/vx9ZmZkkIy2trXgzI4OkdYl+uHEDpSUlpDHtHR1ISUkhaT2JpIBxJaB8rTY0NiI3N1fI+LWrV1FeVsYdI3MJSwWjtiG7V/RVfT3yVF4d1CpXW67ueplQdH8rqRUyPj6OlKQkxds1tbX4oLiYO/vugvPnzuHT2lrFMf1OJywWi1A8ilh6x7gnVfqlU4XNhjLCsnCPY7fb8eWaX0xV2mw4LhiHAsSlMRSMK8n09DReio9f+VNry7v2r7/u30d4eLhIjZq0XgGjyZmPB5lgVCbABGOCEVubZseYHWN2jBgBs2PEeJl7jAqv/wHDEOJNzCU1cwAAAABJRU5ErkJggg==>

[image3]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAGkAAABoCAYAAADy3t6fAAAAAXNSR0IArs4c6QAAB/tJREFUeF7tXb1R9EAM9VUCBUBGDlQCFEBEAUABRBTAUQmQk8FcDAkRlHDjb8Q359E923or79p3gC6D/bGst5J29bOefX191R8fH1X8tpcDs+VyWS8Wi+2lMCirZnVd16+vr8GKLeZAgLTF4KxIC5B+Kkj7+/uTkH56elrd3d01zzo7O6vm83nz98PDQ3V0dNT8PZvNeunyzuV5QaTLM9bb9+XlpTWkU5ICpHU+BUghSWsrYrAkaZXjFV/s//j42PwLVdT19XWl20UV7u7uNv2Pj497Hy/9Tk5Omvb7+/vq7e2t+RvnsuiSufRzUZKwPYcnQqOmcxBIApDYhhI/AUAzGkHKeYbYMmHm6iegyPwpP0YXs5Upz+jrI/zQCzNA6uFUgKQYw5iRsyJDkpS6E/2pxZMxVqscBpK0a/0sqlbbButZCJI89/Dw0NyyrxoZXUzd6WMD4we+0yjqDpnBiKrruumSywwPSFPSZZ3fkA60lQGSgVTJxRMgKY9DSJLigPY44BZ8THWHNgm30HqLLbbq8vKyoXpMuphN+lOSxOyIZsaUiydAUm6hAKmqihxmx1QrAdIvBwl9YOgHxAWgd3c4lvnuPCGUX7cFz5EkHMvCCxok9tywSYVsUoCk3ELbapMCpIlCFR61wrbgnlBFrrpj4632UdxCOQTl+u4856QAaSBSAVKbccUkSbtfBuLzPezp6am6urpqpvBm+ORIEm6zMSVAh1/YFpyF4j08EhWfHT73PNDbd0qQcMXmeMG97+npP8jj4HmAt2+A1OZYgKQylX68JN3c3HiFYlB/CW/rcIScwcRurX4Y/mZtOozNIqA6c1bm1WNRwpGuQS+bOOji4qLVszODdW9vL3HKcbt57AhSwkCyKC+ZaublUFeFS4DUwcUAybG0QpL+M6tTkrRNwjC1nCckhXf1k9Te1DRkOQ9ICKHvh3NhqpS2STKHlbKFqVNW2tX7+7t5fkN60UZp+4Z9Gb9wrmSb5Mlx8Lhf0OPA7Ai2W4dZh4C2ujJPCA6wJLwLUCv9uZjHQeeCl8wUDZCq79z44rngAVKbsVYAkfGrCEjox2IlJkztWH5ALFeRvn2Vfqz8BMd2qSz9P00Xzo2heEyzxlA8pp5ZJTk4VxGPA3PlWCCxMhpPPIktBmYrPfbNE4pn9o3NFSApZAOknmUeklR9F7pZx4FBksTC1EzteNqZK6ekgfa4hcZUw0U2DgFSe/X/ury7kKR1DjBtsRF1l+oyklfBbTOGlnH7ruf2nkes8Lm06Wd1HQ0061lVvK5WZO94e3vbWtf0so1cdefJFGVSl5Pj8FOctcmhCo/vjjE2QFq/mofxK0BKDJ8znyJKpWenOBpI2q0hbn2dgoTVeV0v2EeY6GptG1j1uaXuWEhAXDt4Q8qKLvQSIF3y987OTvMaOJd1qQemCCAv8J0PDg78NglH5LiFvHNZW112MGYrVrfnunJyVHqRc5KXsR7mMMADpP/cpLu7AIm7cjYiSc/Pzw02LLSMLhN2E4kGHXV/11y6vw6X41iPBEtfHU7AW16YhOOzPCBhuBz9eMmHWZ3S5dXXqKI8zGPORw8z2HNzbqHMAYm9Y4CkuBsgJd5igiuSrbKQJMWx8/Pz5i9WmY3tqO4svxb6yBAkKZPRdkifqeS52q7gXBjyZqF4nZaF4XN8R1xcFl3YV86c2peHdCaru5yLcj1ufGagLfuWays9kVlm36wzF44dxQvuIVD6BkjrV5gGSOriXK9U/nhJ8lRVjGnsLUem1y3kcYp6V7+lbbzJ/8le8ABpne3MjgRIKrygmfHnJenz8zN5v4ChZRxoZayyrS5WYOhsT9xy43NxblR3Vvgc58KjAIb1rS050smONMnqzrMF92SKep21np2i145YNbPJK7SjI5Nwlh4WIA2MzHpAC5CMT/P8OUnyVJ+zSj/tukFGYmiZqQJrrq5wg3YpYZWgdgOx8DmTJB1uYJLEKuyTw+eeLTh7AU87A8mai13xluNiYu+QczAeHD4PkHxpWAFSYtjjz0mSxyYxVWC1M5uEqVJWlTf7oIiVdsU86mhH0A5vRJI856QckJhTFOfOKX2x6GQgMVsZICnuBkiKGSFJwz+tyrbgKNGDd3caJPGBWbbAo+4w5I3qLidMjWPRXWVd5o5jGV3o99u4uvOujBzd7wHce7uKJ57kjQEFSD3IBUjqs9ohSVy+t06S2KHR2jazrS4zqp68OxbW56wf1sO7qItsHEqWYwZIbeADpPl8mDhkjApJUp9DZXxEdYfhdLx4yZqPXTaFYX199Rw7VmCKwMarzzep7kqG4hFQT1U8jkW6BoXPf4tNCpAMXeG5JH3M3V2AVAgkrMS2KsbxkVj5h+EFSS3T1QxWKB7nxtAE0onVHZ5qfUkX05XtyeHzsS7bYDYp52zjdeWwjYfVnuNiYu84qPRlSpvEXsBiXIA00Tf9AqRC35nF1CmmNnTYmqk7drsKXkCLl9virV06jctKPcNL5dktJpa6w8vu2a0vyL8iNomBMmaowuPIZCFvTSdbPGzXqdu9Hgecu8g5KUBq3wseICkOhCQpZmD4XJ8vciSJhanZ98q1j4z501hVvKXu2Nyi0qyPmWh/HCvRwXce5LvLAYWN9aZ0sfmsdk+aMXuOZy52NCgSqmAE57QHSIU+KJIDAhsbIGWAxJgb7dNyoPO+u2lJiKcxDgRIjENb0D5bLpf1YrHYAlKChD4O/AMRC38ZlOKndgAAAABJRU5ErkJggg==>

[image4]: <data:image/png;base64,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>

[image5]: <data:image/png;base64,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>

[image6]: <data:image/png;base64,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>

[image7]: <data:image/png;base64,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>
