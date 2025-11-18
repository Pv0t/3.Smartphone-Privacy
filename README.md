# 1.0 Hardware & Operating System
## 1.0 Introduction
Companies like Google, Samsung, Apple, Microsoft, and other big tech collect tons of data about our personal information, who cares about privacy and security already knows that, but the big problem is when you buy a phone you have a pre-installed operating system with apps of the brands you bought, and you can't uninstall them, that means they can collect your data with service and their apps that run in the background. These operating systems are not built to provide a user with security and privacy but to please average users, making the device functional and easy to use.
It's not new that Apple, Google, and Facebook collect every piece of data you produce in their applications, all your data will be profiled and sold to third-party companies, these third-party companies can also be government agencies. An example is the famous program **PRISM** owned by the **National Security Agency (NSA)** they were able to see every name, chat, video, file, picture, and other personal information from users thanks to companies like Google and Apple that allowed the **National Security Agency (NSA)** access to these types of personal data being collected. This issue is not present only in the **United States** but also has a minor impact in the **European Union**.
In the **European Union** exists the **General Data Protection Regulation (GDPR)** that protects the user's data being sold from companies, but a company like **META** can be able to circumvent the **General Data Protection Regulation (GDPR)** just transferring the European Union people's data to the servers of the United States so they can be able to sell it.

Some interesting articles you can read in this regard:
- [Facebook Fined €1.2 Billion for Transferring EU User Data to the US](https://restoreprivacy.com/facebook-fined-e1-2-billion-for-transferring-eu-user-data-to-the-us/)
- [Who Can We Call On? How Our Phones Are Tracked By Big Tech, Telecom, and Government](https://takebackourtech.org/phones-who-can-we-call-on/?ref=kb.above.im)
<details>

<summary>More articles:</summary>

  - ['Alexa, are you invading my privacy?' – the dark side of our voice assistants](https://www.theguardian.com/technology/2019/oct/09/alexa-are-you-invading-my-privacy-the-dark-side-of-our-voice-assistants)
  - [WikiLeaks dump shows CIA could turn smart TVs into listening devices](https://theintercept.com/2017/03/07/wikileaks-dump-shows-cia-could-turn-smart-tvs-into-listening-devices/)
  - [The Stringray: How Law Enforcement Can Track You Every Move](https://www.youtube.com/watch?v=wzSgLpNrr2E)
  - [Edward Snowden: How Your Cell Phone Spies on You](https://www.youtube.com/watch?v=VFns39RXPrU)
  - [Police are tracking you and your license plates](https://www.youtube.com/watch?v=DH7edXaZS0A)
  - [How Police Cameras Recognize and Track Your | WIRED](https://www.youtube.com/watch?v=9Xg-7FfLIVw)

</details>

## 1.2 Choosing the right phone & operating system
Doing some research I discovered that the Google Pixel is more secure than other devices because they have the [Google Tensor security Core and Titan M2 chips](https://security.googleblog.com/2021/10/pixel-6-setting-new-standard-for-mobile.html?ref=devilreef.net). The next step is to choose a pixel model that has long-guaranteed security updates, so we can receive the security updates without changing our device every 2 years. All the last pixel modem guarantee a minimum of 7 years of security updates. For more information about how many years the security update are guarantee by Google on a specific model you can visit this page [Google Pixel Phone LifeTime](https://support.google.com/nexus/answer/4457705?hl=en#zippy=%2Cpixel-a-pixel-pixel-pro).

The second step is to choose the operating system, about the operating system we have a lot of choice, but if you want an operating system secure and privacy-focused the bests is [GrapheneOS](https://grapheneos.org/) that provide a lot of feature about security (e.g. LTE-only mode) and privacy (e.g. Google Play Services sandboxed) over the Google Pixel operating system. For more information about the features click [here](https://grapheneos.org/features).

## 1.3 Installing GrapheneOS
In this GitHub repository, I cover the installation and configuration of the operating system GrapheneOS because it is currently considered the best operating system related to security and privacy.
Before proceeding to the installation, ensure your pixel phone model is supported [here](https://grapheneos.org/faq#supported-devices).
The official site of GrapheneOS provides a detailed guide on how to install the OS on your Pixel phone. You need only choose whether to do so with Web Installer or CLI commands.

- [Web Installer](https://grapheneos.org/install/web)
- [CLI Install](https://grapheneos.org/install/cli)

> [!IMPORTANT]
> After the installation of GrapheneOS ensure your bootloader is locked. | **Settings ➜ System ➜ Developer Options ➜ OEM unlocking ➜ [OFF]**

---

# 2.0 System settings (GrapheneOS)
All the settings I cover up are accessible on the app **'Settings'** of the GrapheneOS operating system. These settings are based only on my threat model and meet a high security and privacy level, feel free to copy or change them based on your preferences. I don't cover personal aspects such as the theme of the keyboard or night light mode. 

## 2.1 Network & Internet
- Internet ➜ Network preferences ➜ Turn on Wi-Fi automatically ➜ ***[OFF]***
- Internet ➜ Network preferences ➜ Notify for public networks ➜ ***[OFF]***
- Internet ➜ Network preferences ➜ Allow WEP networks ➜ ***[OFF]***
- Internet ➜ (Choose your home network) ➜ Privacy ➜ ***[Use per-connection randomized MAC]***
- SIMs ➜ (Click on your carrier) ➜ 4G Calling ➜ ***[ON]***
- SIMs ➜ (Click on your carrier) ➜ Preferred network type ➜ ***[5G (recommended)]***
- SIMs ➜ (Click on your carrier) ➜ 2G network protection ➜ ***[ON]***
- Data Saver ➜ ***[ON]***
- Internet connectivity checks ➜ ***[OFF]***
- Private DNS ➜ Private DNS provider hostname ➜ ***[all.dns.mullvad.net](https://mullvad.net/it/help/dns-over-https-and-dns-over-tls)***

- VPN ➜ (Choose your VPN) ➜ Settings ➜ Always-on VPN & Block connections without VPN ➜ ***[ON]***
  <details>

  <summary>More information:</summary>

  > Using a **Virtual Private Network (VPN)** is a good practice nowadays. **Virtual Private Networks (VPNs)** can reduce some risks (e.g. **Man-in-the-middle/eavesdropping**) the downside is you need to trust the **Virtual Private Network (VPN)** provider. Using a **Virtual Private Network (VPN)** prevents your **Internet Service Provider (ISP)** reading your traffic. For almost two years, I have continued to use the **Mullvad VPN** because it meets my security and privacy standards. Obviously, do some research and choose a **Virtual Private Networks (VPN)** that meets your preferences.

  </details>

## 2.2 Connected devices
- Connection preferences ➜ Bluetooth ➜ Pair new device ➜ Device name ➜ ***[localhost]***

## 2.3 Apps
- Sandboxed Google Play ➜ Google Settings ➜ ***(Disable all settings you can)***
- Sandboxed Google Play ➜ Google Location Accurarcy ➜ ***[OFF]***
- Contacts storage ➜ ***[Device Only]***
- Special app access ➜ Special access to hardware accelerators for Google Apps ➜ ***[OFF]***

## 2.4 Notifications
- Notifications on lock screen ➜ ***[OFF]***
- Enhanced notifications ➜ ***[OFF]***

## 2.5 Display
- Screen timeout ➜ ***[15 seconds]***
- Smooth Display ➜ ***[ON]***

## 2.6 Security & privacy
- Device unlock ➜ Screen lock ➜ ***[PIN]***

> [!IMPORTANT]
> Remember that a biometric unlock isn't protected under the 4th amendment in the same way that a passphrase is. If your device is confiscated, you may be compelled to unlock it via biometrics fingerprint. For more [information](https://uclawreview.org/2020/01/28/smartphones-and-the-fourth-amendment-when-is-access-to-password-protected-information-permitted/).

- Device unlock ➜ Screen lock ➜ Auto-confirm unlock ➜ ***[OFF]***
- Device unlock ➜ Screen lock ➜ Scramble PIN input layout ➜ ***[OFF]***
- Device unlock ➜ Screen lock ➜ Enhanced PIN privacy ➜ ***[ON]***
- Device unlock ➜ Screen lock ➜ Allow camera access when locked ➜ ***[OFF]***
- Device unlock ➜ Screen lock ➜ Lock after screen timeout ➜ ***[Immediately after timeout]***
- Device unlock ➜ Screen lock ➜ Power button instantly locks ➜ ***[ON]***  

- Privacy controls ➜ Camera access ➜ ***[OFF]***
- Privacy controls ➜ Microphone access ➜ ***[OFF]***
- Privacy controls ➜ Show clipboard access ➜ ***[ON]***  
  
- Exploit protection ➜ Auto reboot ➜ ***[4 hours]***
- Exploit protection ➜ USB-C port ➜ ***[Charging-only]***
- Exploit protection ➜ Turn off Wi-Fi automatically ➜ ***[15 seconds]***
- Exploit protection ➜ Turn off Bluetooth automatically ➜ ***[15 seconds]***  
  
- Exploit protection ➜ Memory tagging ➜ Enable by default ➜ ***[ON]***
- Exploit protection ➜ Native code debugging ➜ Block for third-party apps by default ➜ ***[ON]***
- Exploit protection ➜ WebView JIT ➜ Disable for third-party apps by default ➜ ***[ON]***
- Exploit protection ➜ Dynamic code loading via memory ➜ Restrict for third-party apps by default ➜ ***[ON]***
- Exploit protection ➜ Dynamic code loading via storage ➜ Restrict for third-party apps by default ➜ ***[ON]***
- Exploit protection ➜ Secure app spawning ➜ Use secure app spawning ➜ ***[ON]***  
  
- More security & privacy ➜ Allow Sensors permission to apps by default ➜ ***[OFF]***

# 3.0 Strategy
## 3.1 Multiple users
The useful feature that GrapheneOS is the user profile(multiple users). 
Each user profiles have its own unique, randomly generated disk encryption key, and its unique key-encryption key is used to encrypt it. The owner profile does not have access to the data in other profiles. Filesystem-based encryption is designed so that files can be deleted without having the keys for their data and file names, which enables the owner profile to delete other profiles without them being active. GrapheneOS also added the 'end session' button in the power hold menu, which allows to put all the data of the user at rest. For more information [here](https://grapheneos.org/faq#encryption). In this chapter, I describe the two most used threat models.
## 5.1 Only-one user
![Model-1](https://github.com/user-attachments/assets/1cf2bdd5-c5f4-4754-97e2-ffd47fab4fa4)

I called the **'Only-one user'** model because it uses only the **'Owner'** profile. The **'Owner'** profile is created automatically when you configure the phone to the initial configuration, so there are no actions to make. As you can see in the image above, this model consists of installing and using all the apps on the **'Owner'** profile and using it with **Google Play Services** sandboxed provided by the **App Store** from GrapheneOS.

## 5.2 Legion users
![Model-2](https://github.com/user-attachments/assets/cf68a7ae-c314-4a81-8249-69f9f3508b2f)

I called this model **'Legion users'** for a large number of users it needs to be created, it consists of creating a multiple-user profile **[Settings -> System -> Multiple users -> Add user]**. As you can see in the diagram above, the **'Owner'** profile will be used only for the installation and updates of the apps there are on Google Play Store or other stores, after the installation of the applications you want to install, you have to disable it in the **'Owner'** profile and use the feature **'Install available apps'** **[Settings -> System -> Multiples users -> (Choose a profile you want to install the application) -> Install available apps]** to push the applications in the other profiles. GrapheneOS allows you to create a maximum of 31 profiles on your phone, however, it is a waste to create a profile for each app you go to download, so the best way is to create a categorized profile and insert in that profile only the apps involved in that category.

# 4.0 Software
If you want improve your privacy, reduce the attack surface and tracking, you should install only the applications you really needs it. Reduce the permissions of applications to the minimum of necessary.
Here are some permissions features that GrapheneOS added and you need to know because can be a game changer: 
- [Sensors permission](https://grapheneos.org/features#sensors-permission-toggle)
- [Network permission](https://grapheneos.org/features#network-permission-toggle)
- [Contact scopes](https://grapheneos.org/features#contact-scopes)
- [Storage scopes](https://grapheneos.org/features#storage-scopes)

> [!IMPORTANT]
> The list of apps below are in order from recommended to least recommended apps. Some apps are not FOSS and can go against your privacy perspective (e.g. Google Play Store), however, they are on the top of the list because the alternative privacy-focused (e.g. Aurora Store) has security known issues or some are not completely FOSS.

## 4.1 Virtual Private Network(VPN) & Proxy
- ![MullvadVPN-icon](https://github.com/user-attachments/assets/59172ced-cc1d-4c06-8c95-d68c52950080) Mullvad VPN | **<sub><sup>[[Site](https://mullvad.net/it/download/vpn/android)]</sup></sub>** **<sub><sup>[[Google Play Store](https://play.google.com/store/apps/details?id=net.mullvad.mullvadvpn)]</sup></sub>** **<sub><sup>[[F-Droid](https://f-droid.org/packages/net.mullvad.mullvadvpn/)]</sup></sub>**
- ![Orbot-icon](https://github.com/user-attachments/assets/0a917a7b-ba32-4ce6-b653-aecc2d7d64db) Orbot | **<sub><sup>[[Site](https://orbot.app/)]</sup></sub>** **<sub><sup>[[Google Play Store](https://play.google.com/store/apps/details?id=org.torproject.android&hl=it)]</sup></sub>** **<sub><sup>[[Github](https://github.com/guardianproject/orbot)]</sup></sub>** **<sub><sup>[[F-Droid](https://guardianproject.info/fdroid/)]</sup></sub>**
- ![IVPN-icon](https://github.com/user-attachments/assets/eef7bf5e-5a82-496a-b2da-e42390fe9ebf) IVPN | **<sub><sup>[[Site](https://www.ivpn.net/en/)]</sup></sub>** **<sub><sup>[[Google Play Store](https://play.google.com/store/apps/details?id=net.ivpn.client&hl=it)]</sup></sub>** **<sub><sup>[[F-Droid](https://f-droid.org/packages/net.ivpn.client/)]</sup></sub>**
- ![ProtonVPN-icon](https://github.com/user-attachments/assets/f123099d-f796-4615-a528-56df69fefafc) Proton VPN | **<sub><sup>[[Site](https://protonvpn.com/it)]</sup></sub>** **<sub><sup>[[Google Play Store](https://play.google.com/store/apps/details?id=ch.protonvpn.android&hl=it)]</sup></sub>** **<sub><sup>[[Github](https://github.com/ProtonVPN/android-app)]</sup></sub>** **<sub><sup>[[F-Droid](https://f-droid.org/it/packages/ch.protonvpn.android/)]</sup></sub>**

## 4.2 App stores
- ![Google-Play-Store](https://github.com/user-attachments/assets/2ff731b9-6e20-44bc-85e1-f708c78492d4) Google Play Store 
- ![Accrescent](https://github.com/user-attachments/assets/64284d2f-bc49-4e6a-8c30-4907daf90a61) Accrescent | **<sub><sup>[[Site](https://accrescent.app/)]</sup></sub>** **<sub><sup>[[F-Droid](https://f-droid.org/it/packages/com.aurora.store/)]</sup></sub>**
- ![Obtainium](https://github.com/user-attachments/assets/64b54da7-889d-4b8e-944e-798c211cee55) Obtainium | **<sub><sup>[[Github](https://github.com/ImranR98/Obtainium)]</sup></sub>** **<sub><sup>[[F-Droid](https://f-droid.org/packages/dev.imranr.obtainium.fdroid/)]</sup></sub>**
- ![Aurora-Store](https://github.com/user-attachments/assets/b0c10086-d883-43f1-9a86-c4de85490464) Aurora Store | **<sub><sup>[[Site](https://auroraoss.com/)]</sup></sub>** **<sub><sup>[[Gitlab](https://gitlab.com/AuroraOSS/AuroraStore)]</sup></sub>** **<sub><sup>[[Github](https://github.com/accrescent/accrescent)]</sup></sub>**

## 4.3 Browsers
- ![Vanadium-icon](https://github.com/user-attachments/assets/90f35a4a-c0b5-4e9d-b44d-94ae5fa71197) Vanadium | **<sub><sup>[[Github](https://github.com/GrapheneOS/Vanadium)]</sup></sub>**
- ![brave-browser-icon](https://github.com/user-attachments/assets/63a4fa32-d83f-4af2-a08f-c2e4c2a62dba) Brave | **<sub><sup>[[Site](https://brave.com/it/)]</sup></sub>** **<sub><sup>[[Google Play Store](https://play.google.com/store/apps/details?id=com.brave.browser&hl=it)]</sup></sub>**
- ![Firefox-focus-icon](https://github.com/user-attachments/assets/ce4f83cd-0bb1-4d1b-af4d-c58a12ead4c9) Firefox focus | **<sub><sup>[[Site](https://support.mozilla.org/it/products/focus-firefox)]</sup></sub>** **<sub><sup>[[Google Play Store](https://play.google.com/store/apps/details?id=org.mozilla.focus&hl=it)]</sup></sub>**

## 4.4 Youtube Alternative
- ![NewPipe](https://github.com/user-attachments/assets/ffa39e45-93e2-4892-b568-b0035deb0ccd) NewPipe | **<sub><sup>[[Site](https://newpipe.net/)]</sup></sub>** **<sub><sup>[[Github](https://github.com/TeamNewPipe/NewPipe)]</sup></sub>**
- ![LibreTube](https://github.com/user-attachments/assets/995944ef-7f1d-4557-8c03-e6e0d9a898b7) LibreTube | **<sub><sup>[[Site](https://libretube.dev/)]</sup></sub>** **<sub><sup>[[Github](https://github.com/libre-tube/LibreTube)]</sup></sub>** **<sub><sup>[[F-Droid](https://f-droid.org/en/packages/com.github.libretube/)]</sup></sub>**

## 4.5 Podcast
- ![AntennaPodcast](https://github.com/user-attachments/assets/4f1f7f58-ca5a-492f-8054-f74da4d0a273) AntennaPodcast | **<sub><sup>[[Site](https://antennapod.org/)]</sup></sub>** **<sub><sup>[[Google Play Store](https://play.google.com/store/apps/details?id=de.danoeh.antennapod)]</sup></sub>** **<sub><sup>[[F-Droid](https://f-droid.org/packages/de.danoeh.antennapod/)]</sup></sub>**

## 4.6 Communications
- ![SimpleX](https://github.com/user-attachments/assets/dfe1d872-dc86-48bb-a618-17d8d2d8f75c) SimpleX | **<sub><sup>[[Site](https://simplex.chat/)]</sup></sub>** **<sub><sup>[[Google Play Store](https://play.google.com/store/apps/details?id=chat.simplex.app)]</sup></sub>** **<sub><sup>[[F-Droid](https://simplex.chat/fdroid/)]</sup></sub>** 
- ![Molly](https://github.com/user-attachments/assets/e3562fa4-03fe-4ddf-9a97-602f944f15c2) Molly | **<sub><sup>[[Site](https://molly.im/)]</sup></sub>** **<sub><sup>[[F-Droid](https://molly.im/download/fdroid/)]</sup></sub>** **<sub><sup>[Accrescent]</sup></sub>**
- ![Signal-icon](https://github.com/user-attachments/assets/c2266606-51e0-4e1e-a223-c729737a118e) Signal | **<sub><sup>[[Google Play Store](https://play.google.com/store/apps/details?id=org.thoughtcrime.securesms)]</sup></sub>**
- ![Session-icon](https://github.com/user-attachments/assets/347eabc3-02ce-46d2-b57e-f4e4ab431ab6) Session | **<sub><sup>[[Site](https://getsession.org/)]</sup></sub>** **<sub><sup>[[Google Play Store](https://play.google.com/store/apps/details?id=network.loki.messenger&hl=it)]</sup></sub>** **<sub><sup>[[F-Droid](https://fdroid.getsession.org/)]</sup></sub>**

## 4.7 Password Managers
- ![KeePass-icon](https://github.com/user-attachments/assets/3950bcbc-a414-423f-bfe7-b4e9a39a1721) KeePass | **<sub><sup>[[Site](https://www.keepassdx.com/)]</sup></sub>** **<sub><sup>[[Google Play Store](https://play.google.com/store/apps/details?id=com.kunzisoft.keepass.free)]</sup></sub>** **<sub><sup>[[F-Droid](https://f-droid.org/packages/com.kunzisoft.keepass.libre/)]</sup></sub>**
- ![Proton_Pass](https://github.com/user-attachments/assets/a9b60846-f4de-4605-8b6a-8f84fc058fa2) ProtonPass | **<sub><sup>[[Site](https://proton.me/it/pass/download)]</sup></sub>**

## 4.8 2-Factor Authentication
- ![Aegis-icon](https://github.com/user-attachments/assets/d580a7b4-399f-47a0-a7b6-f6b75d6dd71d) Aegis | **<sub><sup>[[Site](https://getaegis.app/)]</sup></sub>** **<sub><sup>[[Google Play Store](https://play.google.com/store/apps/details?id=com.beemdevelopment.aegis&hl=it)]</sup></sub>** **<sub><sup>[[Github](https://github.com/beemdevelopment/Aegis)]</sup></sub>**
- ![EnteAuth-icon](https://github.com/user-attachments/assets/cc9f403f-3935-4675-86b2-4a2b91409345) Ente Auth | **<sub><sup>[[Site](https://ente.io/auth/)]</sup></sub>** **<sub><sup>[[Google Play Store](https://play.google.com/store/apps/details?id=io.ente.auth)]</sup></sub>** **<sub><sup>[[F-Droid](https://f-droid.org/packages/io.ente.auth/)]</sup></sub>**
- ![Yubikey-icon](https://github.com/user-attachments/assets/1d1d989f-fd92-419a-8359-a69216877281) Yubikey |  

## 4.9 Encryption files
- ![Cryptomator-icon](https://github.com/user-attachments/assets/cbf5108a-ccda-4b8c-9afa-a3969fd60fd7) Cryptomator | **<sub><sup>[[Site](https://cryptomator.org/)]</sup></sub>** **<sub><sup>[[Google Play Store](https://play.google.com/store/apps/details?id=org.cryptomator&hl=it)]</sup></sub>** **<sub><sup>[[Github](https://github.com/cryptomator/android/releases)]</sup></sub>**

## 4.10 E-mail provider
- ![Protonmail-icon](https://github.com/user-attachments/assets/e935c1fc-99c3-4803-9575-36ad5a531fbc) Protonmail | **<sub><sup>[[Site](https://proton.me/it/mail)]</sup></sub>** **<sub><sup>[[Google Play Store](https://play.google.com/store/apps/details?id=ch.protonmail.android&=)]</sup></sub>**
- ![Tutanota-icon](https://github.com/user-attachments/assets/33729376-32d3-4acf-b11d-f688ba9f0556) Tuta | **<sub><sup>[[Site](https://tuta.com/it)]</sup></sub>** **<sub><sup>[[Google Play Store](https://play.google.com/store/apps/details?id=de.tutao.tutanota&hl=it)]</sup></sub>**

## 4.11 E-mail clients
- ![Fairmail-icon](https://github.com/user-attachments/assets/c89a1d37-79a9-4bf7-866a-607bfcfd0850) Fairmail | **<sub><sup>[[Site](https://email.faircode.eu/)]</sup></sub>** **<sub><sup>[[Google Play Store](https://play.google.com/store/apps/details?id=eu.faircode.email&hl=it)]</sup></sub>** **<sub><sup>[[Github](https://github.com/M66B/FairEmail)]</sup></sub>** **<sub><sup>[[F-Droid](https://f-droid.org/it/packages/eu.faircode.email/)]</sup></sub>**
- ![K-9-Mail-icon](https://github.com/user-attachments/assets/61a47e7a-b3bd-4e88-9c96-fc3b43e3bded) K-9 Mail | **<sub><sup>[[Site](https://k9mail.app/)]</sup></sub>** **<sub><sup>[[Google Play Store](https://play.google.com/store/apps/details?id=com.fsck.k9&hl=it)]</sup></sub>** **<sub><sup>[[Github](https://github.com/k9mail)]</sup></sub>** **<sub><sup>[[F-Droid](https://f-droid.org/it/packages/com.fsck.k9/)]</sup></sub>**
- ![Thunderbird-icon](https://github.com/user-attachments/assets/7e701ef5-8011-4f0c-8a57-d0f378477a96) Thunderbird | **<sub><sup>[[Site](https://www.thunderbird.net/it/thunderbird/115.0/eoy/)]</sup></sub>** **<sub><sup>[[Google Play Store](https://play.google.com/store/apps/dev?id=8696262544613553264&hl=it)]</sup></sub>**

## 4.12 E-Mail aliases
- ![SimpleLogin-icon](https://github.com/user-attachments/assets/a76237a7-603e-4a11-bd94-796ac7dc6565) Simplelogin | **<sub><sup>[[Site](https://simplelogin.io/it/)]</sup></sub>** **<sub><sup>[[Google Play Store](https://play.google.com/store/apps/details?id=io.simplelogin.android&hl=it)]</sup></sub>** **<sub><sup>[[Github](https://github.com/simple-login/app)]</sup></sub>**
- ![Addy.io-icon](https://github.com/user-attachments/assets/7bf6c1e2-6f9f-4d56-a5a1-88aea0630106) Addy.io | **<sub><sup>[[Site](https://addy.io/)]</sup></sub>** **<sub><sup>[[Google Play Store](https://play.google.com/store/apps/details?id=host.stjin.anonaddy&hl=it)]</sup></sub>** **<sub><sup>[[Github](https://github.com/anonaddy/anonaddy)]</sup></sub>**

## 4.13 File Sharing & Syncting
- ![Syncthing-icon](https://github.com/user-attachments/assets/b3b7ed16-0c8b-44c0-bf7d-b2a34689db97) Syncthing | **<sub><sup>[[Site](https://syncthing.net/)]</sup></sub>** **<sub><sup>[[F-Droid](https://f-droid.org/it/packages/com.nutomic.syncthingandroid/)]</sup></sub>**
- ![Onionshare-icon](https://github.com/user-attachments/assets/7b07938d-1d5a-42d4-a8b5-8d13b965a083) OnionShare | **<sub><sup>[[Site](https://onionshare.org/)]</sup></sub>** **<sub><sup>[[Google Play Store](https://play.google.com/store/apps/details?id=org.onionshare.android&hl=en_US)]</sup></sub>** **<sub><sup>[[F-Droid](https://f-droid.org/packages/org.onionshare.android.fdroid/)]</sup></sub>**

## 4.14 Cloud Storage
- ![Proton-Drive](https://github.com/user-attachments/assets/400cada9-e141-4c49-8a5c-3b2db8f43c2a) Proton Drive | **<sub><sup>[[Site](https://proton.me/it/drive)]</sup></sub>** **<sub><sup>[[Google Play Store](https://play.google.com/store/apps/details?id=me.proton.android.drive)]</sup></sub>**

## 4.15 Calendar
- ![Proton-Calendar](https://github.com/user-attachments/assets/cfa9f468-aead-4a12-8d07-bdf3c3e38e7b) Proton Calendar | **<sub><sup>[[Site](https://proton.me/calendar)]</sup></sub>** **<sub><sup>[[Google Play Store](https://play.google.com/store/apps/details?id=me.proton.android.calendar)]</sup></sub>**

## 4.16 Maps
- ![OSMAnd](https://github.com/user-attachments/assets/7dc1354c-b3a5-4b43-afe6-e78884eb240e) OSMAnd~ | **<sub><sup>[[Site](https://osmand.net/)]</sup></sub>** **<sub><sup>[[Google Play Store](https://play.google.com/store/apps/details?id=net.osmand)]</sup></sub>** **<sub><sup>[[F-Droid](https://f-droid.org/packages/net.osmand.plus/)]</sup></sub>**
- ![Organic-map](https://github.com/user-attachments/assets/593b11ff-d1b7-4059-8a24-e9f711640a97) Organic Maps | **<sub><sup>[[Site](https://organicmaps.app/it/)]</sup></sub>** **<sub><sup>[[Google Play Store](https://play.google.com/store/apps/details?id=app.organicmaps&hl=it)]</sup></sub>** **<sub><sup>[[F-Droid](https://f-droid.org/it/packages/app.organicmaps/)]</sup></sub>**

## 4.17 Notes
- ![Joplin](https://github.com/user-attachments/assets/0651a709-7e24-4bc1-988a-8d9345d470b7) Joplin | **<sub><sup>[[Site](https://joplinapp.org/)]</sup></sub>** **<sub><sup>[[Google Play Store](https://play.google.com/store/apps/details?id=net.cozic.joplin)]</sup></sub>** **<sub><sup>[[Github](https://github.com/laurent22/joplin/)]</sup></sub>** 
- ![OBsidian](https://github.com/user-attachments/assets/5bc5b4df-63ca-496b-9dd7-cf32434baecb) Obsidian | **<sub><sup>[[Site](https://obsidian.md/)]</sup></sub>** **<sub><sup>[[Google Play Store](https://play.google.com/store/apps/details?id=md.obsidian)]</sup></sub>**

## 4.18 Social Media
- ![Mastodon](https://github.com/user-attachments/assets/39434404-d3cd-4dbb-b1f9-cb59307d9f7a) Mastodon | **<sub><sup>[[Site](https://joinmastodon.org/it)]</sup></sub>** **<sub><sup>[[Google Play Store](https://play.google.com/store/apps/details?id=org.joinmastodon.android)]</sup></sub>** 
- ![Bluesky](https://github.com/user-attachments/assets/3744595b-c406-4e9d-9470-777e95e29a42) Bluesky | **<sub><sup>[[Site](https://bsky.app/)]</sup></sub>** **<sub><sup>[[Google Play Store](https://play.google.com/store/apps/details?id=xyz.blueskyweb.app&hl=it)]</sup></sub>**

## 4.19 Phone Number & SMS Masking
- ![SMS-Pool](https://github.com/user-attachments/assets/adbf54b2-e168-4db5-84e9-1e4e0ea10364) SMSPool | **<sub><sup>[[Site](https://www.smspool.net/)]</sup></sub>**
- ![Silent.link](https://github.com/user-attachments/assets/130b6a2f-2b34-4f9a-bf88-7b41e355241b) Silent.lnk | **<sub><sup>[[Site](https://silent.link/)]</sup></sub>**
- ![Crypton.sh](https://github.com/user-attachments/assets/06a04df1-d901-4a5d-b466-9c40cb6eca7b) Crypton.sh | **<sub><sup>[[Site](https://crypton.sh/)]</sup></sub>**
- ![Jmp.chat](https://github.com/user-attachments/assets/736726d8-dcf3-4cc6-a8c6-0ed9d2874226) Jmp.chat | **<sub><sup>[[Site](https://jmp.chat/)]</sup></sub>**
- ![MoneroSMS](https://github.com/user-attachments/assets/b8ab4784-61d4-4729-8164-a76494224917) MoneroSMS | **<sub><sup>[[Site](https://monerosms.com/)]</sup></sub>**

## 4.20 Payments
- ![Cash](https://github.com/user-attachments/assets/4b66ba12-f109-4051-9c07-0d46dbc81545) Cash
- ![Gift-cards](https://github.com/user-attachments/assets/6426d485-d0b8-45b8-86c0-3a6671a2cbf3) Gift cards
- ![Privacy.com](https://github.com/user-attachments/assets/5c13a082-2ab9-4dea-aa77-f2f265c3e43e) Privacy.com [US] | **<sub><sup>[[Site](https://privacy.com/)]</sup></sub>** **<sub><sup>[[Google Play Store](https://play.google.com/store/apps/details?id=com.privacy.pay&pli=1)]</sup></sub>**
- ![Revolut](https://github.com/user-attachments/assets/5632f011-1ca3-48c8-b1c0-7faea44a23d6) Revolut [EU] | **<sub><sup>[[Site](https://www.revolut.com/)]</sup></sub>** **<sub><sup>[[Google Play Store](https://play.google.com/store/apps/details?id=com.revolut.revolut&hl=it)]</sup></sub>**po

## 4.21 Cryptocurrencies & Wallet
- ![Monero](https://github.com/user-attachments/assets/a1cfabe1-ecb8-4ec0-969e-071a11fab73f) Monero | **<sub><sup>[[Site](https://www.getmonero.org/)]</sup></sub>** **<sub><sup>[[Download](https://www.getmonero.org/downloads/)]</sup></sub>**
- ![Cake-Wallet](https://github.com/user-attachments/assets/162000ad-54b1-4199-b1a0-d4e29858ef82) Cake Wallet | **<sub><sup>[[Site](https://cakewallet.com/)]</sup></sub>** **<sub><sup>[[Google Play Store](https://play.google.com/store/apps/details?id=com.cakewallet.cake_wallet)]</sup></sub>** **<sub><sup>[[Github](https://github.com/cake-tech/cake_wallet/releases)]</sup></sub>**

# 5.0 Stay update
The privacy world is continuously changing, with new applications, new features, and some downgrades. It's fundamental to stay updated on what is happening in this world, for this purpose I suggest some youtube channels and news so you can stay updated. 
<details>

<summary>News:</summary>

- [Electronic Frontier Foundation](https://www.eff.org/) | **<sub><sup>[[RSS Feed](https://www.eff.org/rss)]</sup></sub>**

</details>

<details>

<summary>Youtubers:</summary>

- [Naomi Brockwell TV](https://www.youtube.com/@NaomiBrockwellTV)
- [Side Of Burritos](https://www.youtube.com/@sideofburritos)

</details>

<details>

<summary>Forums:</summary>

- [GrapheneOS](https://discuss.grapheneos.org/)
- [PrivacyGuides](https://discuss.privacyguides.net/)

</details>

<details>

<summary>Sites:</summary>

- [WikiLeaks](https://wikileaks.org/)
- [Privacy-Guides](https://www.privacyguides.org/en/)
- [Exodus](https://reports.exodus-privacy.eu.org/en/)
- [Tor Project](https://www.torproject.org/)
- [PrivacySpy](https://privacyspy.org/)

</details>

> [!IMPORTANT]
> You need this only for informative scopes, don't take what they are said as "always true", stay in doubt, do your research, create your personal opinion, and apply it to your threat model.

# 6.0 Clarify some doubts and possible questions.

1. **What is a Duress PIN?** The Duress PIN feature that GrapheneOS provides, is able to set a PIN of your choice and if this PIN is entered on the lock screen your entire device will be wiped. Fore more information [here](https://grapheneos.org/features#duress).

2. **Why in the 'Settings' section the Duress PIN is not suggested?** The Duress PIN has only one problem, you can be charged if it is used against law enforcement to hide something, so using it, most of the time it's pretty useless nowadays. For more information, this is a law that you can be charged if used in the **United States** [Destruction of Evidence](https://www.chamberslawfirmca.com/what-does-it-mean-to-be-charged-with-destruction-of-evidence-a-criminal-defense-attorney-explains/).

3. **What is PIN scramble?** When you have to insert your PIN to unlock your phone, as you have notice the numbers have always the same order from lower number(top) to higher number(bottom), PIN scramble prevents that. When PIN scrambe is enabled the layout will be generated randomly. A possible side-eye can try to steal your PIN depending on the possition where you press on screen lock, so if some side-eye is trying to steal your PIN this feature will make it harder. For more information [here](https://grapheneos.org/features#pin-scrambling).

6. **Why in the 'Settings' section the scramble PIN are not suggested?** This feature has some disadvantages. The first one is that the layout is always randomized, so your brain needs to "check" every time you want to unlock the phone where the numbers you want to press are, which means it will take you longer to unlock your phone. Let's make an example: Imagine you are in the subway or in some crowded place and you want to unlock your phone. With this feature enabled, the people beside you and watching your phone will know your PIN because the slower you have to realize where the numbers you need to press are, the more time it requires you to unlock the phone. This gives a lot of advantages to the hacker to read your PIN.

