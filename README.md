# 4G and 5G Security

## Protocols
- Signaling (SS7 and Diameter Signaling)
  ```
  SS7 is being used for 35 years to provides signaling that enables mobile and fixed network operators to setup/teardown calls, to route text (SMS) messages, support inter-network connectivity and transparent roaming, and to provide per-session information such as caller ID. 
  While SS7 was the foundation for signaling in 2G/3G circuit switch networks, Diameter has been introduced for 4G LTE and VoLTE packet networks and IP Multimedia Subsystem (IMS) based systems, and is key to enabling new revenue-generating IP services. 
  Diameter signaling is also implemented in 5G network as there's no changes in requirement in terms of signaling
  ```
  source: [ribboncommunication: SS7 and Diameter Signaling](https://ribboncommunications.com/solutions/service-provider-solutions/mobile-network-evolution/ss7-and-diameter-signaling)
## 4G Security 
- Concerns
  ```
  The incorrect use of Diameter leads to the presence of several vulnerabilities in 4G networks, resembling the ones found in older networks that use SS7. These are vulnerabilities that the Diameter protocol is supposed to prevent.

  4G operators rarely using important diameter protocol features, leaving subscribers and providers exposed to several threats, including:

  - Subscriber information disclosure
  - Network information disclosure
  - Subscriber traffic interception
  - Fraud
  - Denial of Service

  The risks of these misconfigurations “could lead to sudden failure of ATMs, payment terminals, utility meters, car alarms, and video surveillance", the researchers state in their report. One of the reasons is the use of 4G SIM card modules that connect to servers when located in remote areas, where classic internet connections are unavailable.

  Open door for hackers to target 4G enabled IoT-devices
  Even tracking the location of users, intercepting SMS or phone calls are possible on Diameter due to these misconfigurations. With the rise of the Internet of Things devices, Positive Technologies warns such flaws cause major threats. As stated on Positive Technologies’ website, “in the case of many 4G-enabled devices—such as pipeline safety sensors and gas leak detectors—lack of connectivity can lead to major financial losses and life-threatening accidents.”



  ```
  source: [infradata: Diameter protocol has same vulnerablities as SS7 standard](https://www.infradata.com/news-blog/diameter-protocol-has-same-vulnerablities-as-ss7-standard/)

- Hacking 4G Phone
  ```
  IMSI CATCHER

  - Performs Man in The Middle attack,
  by mimicking base station with IMSI catcher. With this hacker can get user's MC (some identification) and connect to the legitimate network with it. Hacker can use this connection to initiate call, sms as the hacked user and track the precise location of the user
  
  - Performs a Denial of Service, 
  by mimicking base station hacker can force the user go to 2G or 3G connection, once the user is using 2G or 3G hacker can sniff all messages and calls.

  Hacker can build this IMSI catcher with $800 
  ```
  source: [NDC Conference: Hacking 4G and how to get arrested in 10 minutes - Christian Sørseth
](https://www.youtube.com/watch?v=DEeOFE_DreU)

- Hacking 4G Module in IOTs and Cars 
  ```
  What XiaoHuiHui and team have found:

  - General Vulnerabilities on Embede Linux or RTOS
  - Authentication risk in several modules
  - Remote Code Executionin 5+ cars T-Box
  - Vulnerabilities in all parts of 4G including Web Vuln in server-side and System Management Service in Client-side
  ```
  source: [DEFCON27: XiaoHuiHui - All the 4G Modules Could Be Hacked](https://www.youtube.com/watch?v=OORUkEsannA)

## 5G Security

- What's new?
  ![alt text](https://i.imgur.com/CUHSdyv.jpg)
  source: [thalesgroup: 5G AND 4G: WHAT’S THE DIFFERENCE?](https://www.thalesgroup.com/en/worldwide-digital-identity-and-security/mobile/magazine/5g-and-4g-whats-difference)

- New Security Measure
  ```
  The 5G SA network supports more security features to tackle potential security challenges in the future 5G
  lifecycle. 5G NSA and 4G networks share the same security mechanisms and work in standard and practice
  consistently to keep improving their security levels.
  
  • Stronger air interface security: In addition to user data encryption on 2G, 3G, and 4G networks, 5G
  standards provide user data integrity protection to prevent user data from being tampered with.
  
  • Enhanced user privacy protection: In 2G, 3G, and 4G networks, users' permanent IDs (international mobile
  subscriber identities — IMSIs), are transmitted in plain text over the air interface. Attackers can exploit this
  vulnerability using IMSI catcher attacks to track users. In 5G networks, users' permanent IDs (in this case,
  SUPIs) are transmitted in ciphertext to defend against such attacks.
  
  • Better roaming security: Operators usually need to set up connections via third-party operators. Attackers
  can forge legitimate core network nodes to initiate Signaling System 7 and other attacks by manipulating
  third-party operators' devices. 5G SBA defines Security Edge Protection Proxy (SEPP) to implement E2E
  security protection for inter-operator signaling at the transport and application strata. This prevents thirdparty operators' devices from tampering with sensitive data (e.g. key, user ID, and SMS) exchanged
  between core networks.
  
  • Enhanced cryptographic algorithms: 5G R15 standards currently define security mechanisms such as 256-
  bit key transmission. Future 5G standards will support 256-bit cryptographic algorithms to ensure that such
  algorithms used on 5G networks are sufficiently resistant to attacks by quantum computers. The 3GPP
  has recommended that the ETSI Security Algorithms Group of Experts (SAGE) start to evaluate 256-bit
  cryptographic algorithms.  
  ```
  source: [Huawei: 5G Security Assurance](https://huawei.eu/file-download/download/public/1442#:~:text=4.1-,Industry%2Dleading%20Security%20Measures%20for%20the%20Access%20Network,security%20mechanisms%20used%20in%204G.&text=5G%20inherits%20security%20protection%20mechanisms,tampering%20on%20the%20user%20plane.)
- Security Research and Result
  ```
  - Purdue University and the University of Iowa

  The researchers, using their tool called the "5GReasoner", found that 5G is still subject to some of the same exploits as 4G, despite touting a more "robust security posture" than previous cellular network generations.

  The 5GReasoner discovered 11 new surveillance and disruption threats to the network by conducting a series of attacks against 5G-connected phones from a radio base station.

  In one of these attacks, researchers obtained old and new temporary network identifiers of a victim's phone, which allowed them to track its location through its paging occasion. They could also broadcast fake emergency alerts by hijacking the paging channel, which could lead to "artificial chaos." Both real-time location tracking and false emergency alerts are vulnerabilities shared by 4G and 5G networks.

  Another attack discovered a means to create a prolonged denial-of-service condition, which could completely disconnect a target's phone from the network for an extended period of time. It could also downgrade the phone to a less secure connection, leaving it open for law enforcement and other hackers to launch surveillance attacks.

  ```
  source: [ITPRO: 5G networks are vulnerable to hacking](https://www.itpro.co.uk/mobile-security/34807/5g-networks-are-vulnerable-to-hacking)
