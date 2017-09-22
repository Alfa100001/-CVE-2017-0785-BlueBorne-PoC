# -CVE-2017-0785-BlueBorne-PoC
CVE-2017-0785 BlueBorne PoC
General Overview

Armis Labs revealed a new attack vector endangering major mobile, desktop, and IoT operating systems, including Android, iOS, Windows, and Linux, and the devices using them. The new vector is dubbed “BlueBorne”, as it spread through the air (airborne) and attacks devices via Bluetooth. Armis has also disclosed eight related zero-day vulnerabilities, four of which are classified as critical. BlueBorne allows attackers to take control of devices, access corporate data and networks, penetrate secure “air-gapped” networks, and spread malware laterally to adjacent devices. Armis reported these vulnerabilities to the responsible actors, and is working with them as patches are being identified and released.

Blueborne Brief Overview

What Is BlueBorne?
BlueBorne is an attack vector by which hackers can leverage Bluetooth connections to penetrate and take complete control over targeted devices. BlueBorne affects ordinary computers, mobile phones, and the expanding realm of IoT devices. The attack does not require the targeted device to be paired to the attacker’s device, or even to be set on discoverable mode. Armis Labs has identified eight zero-day vulnerabilities so far, which indicate the existence and potential of the attack vector. Armis believes many more vulnerabilities await discovery in the various platforms using Bluetooth. These vulnerabilities are fully operational, and can be successfully exploited, as demonstrated in our research. The BlueBorne attack vector can be used to conduct a large range of offenses, including remote code execution as well as Man-in-The-Middle attacks.

Additional Information: Download our Technical White Paper on BlueBorne
What Is The Risk?

The BlueBorne attack vector has several qualities which can have a devastating effect when combined. By spreading through the air, BlueBorne targets the weakest spot in the networks’ defense – and the only one that no security measure protects. Spreading from device to device through the air also makes BlueBorne highly infectious. Moreover, since the Bluetooth process has high privileges on all operating systems, exploiting it provides virtually full control over the device.

Unfortunately, this set of capabilities is extremely desireable to a hacker. BlueBorne can serve any malicious objective, such as cyber espionage, data theft, ransomware, and even creating large botnets out of IoT devices like the Mirai Botnet or mobile devices as with the recent WireX Botnet. The BlueBorne attack vector surpasses the capabilities of most attack vectors by penetrating secure “air-gapped” networks which are disconnected from any other network, including the internet.
How Wide Is The Threat?
The threat posed by the BlueBorne attack vector

The BlueBorne attack vector can potentially affect all devices with Bluetooth capabilities, estimated at over 8.2 billion devices today. Bluetooth is the leading and most widespread protocol for short-range communications, and is used by devices of all kinds, from regular computers and mobile devices to IoT devices such as TVs, watches, cars, and even medical appliances. The latest published reports show more than 2 billion Android, 2 billion Windows, and 1 billion Apple devices in use. Gartner reports that there are 8 billions connected or IoT devices in the world today, many of which have Bluetooth.
What Is New About BlueBorne?
A new airborne attack vector

BlueBorne concerns us because of the medium by which it operates. Unlike the majority of attacks today, which rely on the internet, a BlueBorne attack spreads through the air. This works similarly to the two less extensive vulnerabilities discovered recently in a Broadcom Wi-Fi chip by Project Zero and Exodus. The vulnerabilities found in Wi-Fi chips affect only the peripherals of the device, and require another step to take control of the device. With BlueBorne, attackers can gain full control right from the start. Moreover, Bluetooth offers a wider attacker surface than WiFi, almost entirely unexplored by the research community and hence contains far more vulnerabilities.

Airborne attacks, unfortunately, provide a number of opportunities for the attacker. First, spreading through the air renders the attack much more contagious, and allows it to spread with minimum effort. Second, it allows the attack to bypass current security measures and remain undetected, as traditional methods do not protect from airborne threats. Airborne attacks can also allow hackers to penetrate secure internal networks which are “air gapped,” meaning they are disconnected from any other network for protection. This can endanger industrial systems, government agencies, and critical infrastructure.

Finally, unlike traditional malware or attacks, the user does not have to click on a link or download a questionable file. No action by the user is necessary to enable the attack
A comprehensive and severe threat

The BlueBorne attack vector requires no user interaction, is compatible to all software versions, and does not require any preconditions or configurations aside of the Bluetooth being active. Unlike the common misconception, Bluetooth enabled devices are constantly searching for incoming connections from any devices, and not only those they have been paired with. This means a Bluetooth connection can be established without pairing the devices at all. This makes BlueBorne one of the most broad potential attacks found in recent years, and allows an attacker to strike completely undetected.
Next generation Bluetooth vulnerabilities

In the past, most Bluetooth vulnerabilities and security flaws originated in issues with the protocol itself, which were resolved in version 2.1 in 2007. Nearly all vulnerabilities found since were of low severity, and did not allow remote code execution. This transition occurred as the research community turned its eyes elsewhere, and did not scrutinize the implementations of the Bluetooth protocol in the different platforms, as it did with other major protocols.

Bluetooth is a difficult protocol to implement, which makes it prone to two kinds of vulnerabilities. On the one hand, vendors are likely to follow the protocol’s implementation guidelines word-for-word, which means that when a vulnerability is found in one platform it might affect others. These mirrored vulnerabilities happened with CVE-2017-8628 and CVE-2017-0783 (Windows & Android MiTM) which are “identical twins”. On the other hand, in some areas the Bluetooth specifications leave too much room for interpretation, causing fragmented methods of implementation in the various platforms, making each of them more likely to contain a vulnerability of its own.

This is why the vulnerabilities which comprise BlueBorne are based on the various implementations of the Bluetooth protocol, and are more prevalent and severe than those of recent years. We are concerned that the vulnerabilities we found are only the tip of the iceberg, and that the distinct implementations of the protocol on other platforms may contain additional vulnerabilities.
A Coordinated Disclosure

Armis reached out to the following actors to ensure a safe, secure, and coordinated response to the vulnerabilities identified.

    Google – Contacted on April 19, 2017, after which details were shared. Released public security update and security bulletin on September 4th, 2017. Coordinated disclosure on September 12th, 2017.
    Microsoft – Contacted on April 19, 2017 after which details were shared. Updates were made on July 11. Public disclosure on September 12, 2017 as part of coordinated disclosure.
    Apple – Contacted on August 9, 2017. Apple had no vulnerability in its current versions.
    Samsung – Contact on three separate occasions in April, May, and June. No response was received back from any outreach.
    Linux – Contacted August 15 and 17, 2017. On September 5, 2017, we connected and provided the necessary information to the the Linux kernel security team and to the Linux distributions security contact list and conversations followed from there. Targeting updates for on or about September 12, 2017 for coordinated disclosure.

Affected Devices
The threat posed by the vulnerabilities Armis disclosed

The vulnerabilities disclosed by Armis affect all devices running on Android, Linux, Windows, and pre-version 10 of iOS operating systems, regardless of the Bluetooth version in use. This means almost every computer, mobile device, smart TV or other IoT device running on one of these operating systems is endangered by at least one of the eight vulnerabilities. This covers a significant portion of all connected devices globally.
What Devices Are Affected?

Android
All Android phones, tablets, and wearables (except those using only Bluetooth Low Energy) of all versions are affected by four vulnerabilities found in the Android operating system, two of which allow remote code execution (CVE-2017-0781 and CVE-2017-0782), one results in information leak (CVE-2017-0785) and the last allows an attacker to perform a Man-in-The-Middle attack (CVE-2017-0783).

Examples of impacted devices:

    Google Pixel
    Samsung Galaxy
    Samsung Galaxy Tab
    LG Watch Sport
    Pumpkin Car Audio System

Google has issued a security update patch and notified its partners. It was available to Android partners on August 7th, 2017, and made available as part of the September Security Update and Bulletin on September 4, 2017. We recommend that users check that Bulletin for the latest most accurate information. Android users should verify that they have the September 9, 2017 Security Patch Level,

Note to Android users: To check if your device is at risk or is the devices around you are at risk, download the Armis BlueBorne Scanner App on Google Play.

Windows
All Windows computers since Windows Vista are affected by the “Bluetooth Pineapple” vulnerability which allows an attacker to perform a Man-in-The-Middle attack (CVE-2017-8628).

Microsoft issued has security patches to all supported Windows versions on July 11, 2017, with coordinated notification on Tuesday, September 12. We recommend that Windows users should check with the Microsoft release at here for the latest information.

Linux
Linux is the underlying operating system for a wide range of devices. The most commercial, and consumer-oriented platform based on Linux is the Tizen OS.

All Linux devices running BlueZ are affected by the information leak vulnerability (CVE-2017-1000250).
All Linux devices from version 3.3-rc1 (released in October 2011) are affected by the remote code execution vulnerability (CVE-2017-1000251)

Examples of impacted devices:

Samsung Gear S3 (Smartwatch)
Samsung Smart TVs
Samsung Family Hub (Smart refrigerator)

Patches to Linux vulnerabilities have been pushed to the upstream projects. The information leak vulnerability was patched here, and the remote code execution was patched here Linux distributions have started to push updates as well, please look for specific updates made by your distribution.

iOS
All iPhone, iPad and iPod touch devices with iOS 9.3.5 and lower, and AppleTV devices with version 7.2.2 and lower are affected by the remote code execution vulnerability (CVE-2017-14315). This vulnerability was already mitigated by Apple in iOS 10, so no new patch is needed to mitigate it. We recommend you upgrade to the latest iOS or tvOS available.

If you are concerned that your device may not be patched, we recommend disabling Bluetooth, and minimizing its use until you can confirm a patch is issued and installed on your device.
Technical Overview
BlueBorne Explained: How The Attack Vector Works

The BlueBorne attack vector has several stages. First, the attacker locates active Bluetooth connections around him or her. Devices can be identified even if they are not set to “discoverable” mode. Next, the attacker obtains the device’s MAC address, which is a unique identifier of that specific device. By probing the device, the attacker can determine which operating system his victim is using, and adjust his exploit accordingly. The attacker will then exploit a vulnerability in the implementation of the Bluetooth protocol in the relevant platform and gain the access he needs to act on his malicious objective. At this stage the attacker can choose to create a Man-in-The-Middle attack and control the device’s communication, or take full control over the device and use it for a wide array of cybercriminal purposes.

Download our Technical White Paper on BlueBorne
BlueBorne attack on Android

Once the attacker determined his target is using the Android operating system, he can use four of the vulnerabilities disclosed by Armis to exploit the device, or they can use a separate vulnerability to conduct a Man-in-The-Middle attack.


Demo Android

Information Leak Vulnerability (CVE-2017-0785)
The first vulnerability in the Android operating system reveals valuable information which helps the attacker leverage one of the remote code execution vulnerabilities described below. The vulnerability was found in the SDP (Service Discovery Protocol) server, which enables the device to identify other Bluetooth services around it. The flaw allows the attacker to send a set of crafted requests to the server, causing it to disclose memory bits in response. These pieces of information can later be used by the attacker to overcome advanced security measures and take control over the device. This vulnerability can also allow an attacker to leak encryption keys from the targeted device and eavesdrop on Bluetooth communications, in an attack that very much resembles heartbleed.

Remote Code Execution Vulnerability #1 (CVE-2017-0781)
This vulnerability resides in the Bluetooth Network Encapsulation Protocol (BNEP) service, which enables internet sharing over a Bluetooth connection (tethering). Due to a flaw in the BNEP service, a hacker can trigger a surgical memory corruption, which is easy to exploit and enables him to run code on the device, effectively granting him complete control. Due to lack of proper authorization validations, triggering this vulnerability does not require any user interaction, authentication or pairing, so the targeted user is completely unaware of an ongoing attack.

Remote Code Execution vulnerability #2 (CVE-2017-0782)
This vulnerability is similar to the previous one, but resides in a higher level of the BNEP service – the Personal Area Networking (PAN) profile – which is responsible for establishing an IP based network connection between two devices. In this case, the memory corruption is larger, but can still be leveraged by an attacker to gain full control over the infected device. Similar to the previous vulnerability, this vulnerability can also be triggered without any user interaction, authentication or pairing.

The Bluetooth Pineapple – Man in The Middle attack (CVE-2017-0783)
Man-in-The-Middle (MiTM) attacks allow the attacker to intercept and intervene in all data going to or from the targeted device. To create a MiTM attack using Wi-Fi, the attacker requires both special equipment, and a connection request from the targeted device to an open WiFi network. In Bluetooth, the attacker can actively engage his target, using any device with Bluetooth capabilities. The vulnerability resides in the PAN profile of the Bluetooth stack, and enables the attacker to create a malicious network interface on the victim’s device, re-configure IP routing and force the device to transmit all communication through the malicious network interface. This attack does not require any user interaction, authentication or pairing, making it practically invisible.
BlueBorne attack on Windows

We have disclosed a vulnerability in Windows which allows an attacker to conduct a Man-in-The-Middle attack.

Demo Windows
The Bluetooth Pineapple #2 – Man in The Middle attack (CVE-2017-8628)

This vulnerability is identical to the one found in the Android operating system, and affects both systems since they shared the same principals in implementing some of the Bluetooth protocol. The vulnerability resides in the Bluetooth stack, and enables the attacker to create a malicious  network interface on the victim’s device, re-configure IP routing and force the device to transmit all communication through it. This attack does not require any user interaction, authentication or pairing, making it also practically invisible.
BlueBorne attack on Linux

Armis has disclosed two vulnerabilities in the Linux operating system which allow attackers to take complete control over infected devices. The first is an information leak vulnerability, which can help the attacker determine the exact version used by the targeted device and adjust his exploit accordingly. The second is a stack overflow with can lead to full control of a device.

Demo Linux
Information leak vulnerability (CVE-2017-1000250)

Similar to the information leak vulnerability in Android, this vulnerability resides in the SDP server responsible for identifying other services using Bluetooth around the device. The flaw allows the attacker to send a set of crafted requests to the server, causing it to disclose memory bits in response. This can be used by an attacker to expose sensitive data from the Bluetooth processthat may also contain encryption keys of Bluetooth communications. These can be used by the attacker to initiate an attack that very much resembles heartbleed.
A stack overflow in BlueZ (CVE-2017-1000251)

This vulnerability was found in the Bluetooth stack of the Linux Kernel, which is the very core of the operating system. An internal flaw in the L2CAP (Logical Link Control and Adaptation Protocol) that is used to connect between two devices causes a memory corruption. An attacker can use this memory corruption to gain full control of the device.
BlueBorne attack on iOS

This vulnerability found by Armis was disclosed to Apple. Since it was mitigated in iOS version 10 and Apple TV version above 7.2.2, a full exploit was not developed to demonstrate how this vulnerability can be leveraged for gaining full control of an iOS device. However, this vulnerability still poses great risk to any iOS device prior to version 10, as it is does not require any interaction from the users, or configuration of any sort on the targeted device. The vulnerability can be leveraged by an attacker to gain remote code execution in a high-privileged context (the Bluetooth process).
Remote code execution via Apple’s Low Energy Audio Protocol – CVE-2017-14315

This vulnerability was found in a new protocol Apple has invented, which operates on top of Bluetooth, called LEAP (Low energy audio protocol). The protocol is designed to stream audio to low energy audio peripherals (such as low energy headsets, or the Siri Remote). This enables devices that only have Bluetooth Low Energy to stream audio and send audio commands. Due to a flaw in the implementation of LEAP, a large audio command can be sent to a targeted device and lead to a memory corruption. Since the audio commands sent via LEAP are not properly validated, an attacker can use the memory corruption to gain full control of the device.
Securing against BlueBorne

Vulnerabilities that can spread over the air and between devices pose a tremendous threat to any organization or individual. Current security measures, including endpoint protection, mobile data management, firewalls, and network security solution are not designed to identify these type of attacks, and related vulnerabilities and exploits, as their main focus is to block attacks that can spread via IP connections.

New solutions are needed to address the new airborne attack vector, especially those that make air gapping irrelevant. Additionally, there will need to be more attention and research as new protocols are using for consumers and businesses alike. With the large number of desktop, mobile, and IoT devices only increasing, it is critical we can ensure these types of vulnerabilities are not exploited. This is the primary mission of Armis in this new connected age.

To run, be sure to have pybluez and pwntools installed.

    sudo apt-get install bluetooth libbluetooth-dev
    sudo pip install pybluez
    sudo pip install pwntools
video : 
# https://www.youtube.com/watch?v=_g84d23t-zc&feature=youtu.be
----------------------------
Follow me :
# https://twitter.com/Alfa100001
# https://github.com/Alfa100001
