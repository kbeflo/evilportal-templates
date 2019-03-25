## Evil Portals

![](https://img.shields.io/github/license/kbeflo/evilportals.svg?style=flat-square) 
[![HitCount](http://hits.dwyl.io/kbeflo/evilportals.svg)](http://hits.dwyl.io/kbeflo/evilportals) [![](https://img.shields.io/discord/413223793016963073.svg?style=flat-square)](https://discord.gg/Ka557WS)

[Evil Portals](https://github.com/kbeflo/evilportals) is a collection of portals that can be loaded into the Evil Portal module and can be used for phishing attacks against WiFi clients in order to obtain credentials or infect the victims with malware using the [Hak5](https://hak5.org/) [WiFi Pineapple](https://wifipineapple.com/) [Tetra](http://hakshop.myshopify.com/products/wifi-pineapple?variant=11303845317) and [Nano](http://hakshop.myshopify.com/products/wifi-pineapple?variant=81044992).

This project requires you to install [Evil Portal](https://github.com/frozenjava/EvilPortalNano) captive portal module created by [frozenjava](https://github.com/frozenjava). Install on the Pineapple, Modules -> Manage Modules -> Get Modules from WiFiPineapple.com -> Evil Portal 3.1.

---

#### Usage

Clone the repository

	git clone https://github.com/kbeflo/evilportals

Change directory to evilportals/portals/

	cd evilportals/portals/

Copy the portals you wish to use on the Tetra at `/root/portals/` or on the Nano at `/sd/portals/`

    scp -r portal-login root@172.16.42.1:/root/portals/

Alternatively you can use [Filezilla](https://filezilla-project.org/) to copy the portals

	Host: sftp://172.16.42.1 Username: root Password: lamepassword Port: 22 

Finally on the WiFi Pineapple web interface, start the Evil Portal module and then activate the portal you wish to use.

#### USING MAIL FUNCTION 

To use the sendmail function of the portals (mailtoken) you need to setup Smtp on your WiFi Pinapple first !
Instructions can be found at the info page of evilportal :
[Evil Portals](https://github.com/kbeflo/evilportals)


After gathering credentials, captured data will be shown as a notification on the WiFi Pineapple web interface, and also stored on the Tetra at `/root/evilportal-logs/portal-login.txt` or on the Nano at `/sd/evilportal-logs/portal-login.txt` with additional profiling.

---

#### Screenshots

<img src="https://user-images.githubusercontent.com/13497504/34363974-1b5e5f1e-eabc-11e7-99f5-78043f8b3ac9.png" width="200"/> <img src="https://user-images.githubusercontent.com/13497504/34363975-1d4b32ca-eabc-11e7-8532-2105a160c5c1.png" width="200"/> <img src="https://user-images.githubusercontent.com/13497504/34363977-1e8f4ca2-eabc-11e7-885e-e7dbd845e217.png" width="200"/>

<img src="https://user-images.githubusercontent.com/13497504/34363979-1f66e108-eabc-11e7-8dbb-39fa8b22c3a7.png" width="200"/> <img src="https://user-images.githubusercontent.com/13497504/34363982-20258324-eabc-11e7-93e0-b775fa1bcc25.png" width="200"/> <img src="https://user-images.githubusercontent.com/13497504/34366525-bba03dc4-ead7-11e7-8bea-a3fa9ae33ef4.png" width="200"/>

---

#### License
Evil Portals is distributed under the GNU GENERAL PUBLIC LICENSE v3. See [LICENSE](https://github.com/kbeflo/evilportals/blob/master/LICENSE) for more information.

#### Disclaimer
* Usage of Evil Portals for attacking infrastructures without prior mutual consistency can be considered as an illegal activity. It is the final user's responsibility to obey all applicable local, state and federal laws. Authors assume no liability and are not responsible for any misuse or damage caused by this program. 

---

Some of the portals here are also available for [Wifiphisher](https://github.com/wifiphisher/wifiphisher), available here [wifiphisher/extra-phishing-pages](https://github.com/wifiphisher/extra-phishing-pages)

Discussion thread - [Hak5 Forums](https://forums.hak5.org/index.php?/topic/39856-evil-portals/)

[Donate](https://paypal.me/kbeflo)

[Kleo Bercero](https://kbeflo.github.io/)
