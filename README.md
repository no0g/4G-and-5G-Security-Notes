# 4G and 5G Security

## Protocols
- Signaling (SS7 and Diameter Signaling)
  ```
  SS7 is being used for 35 years to provides signaling that enables mobile and fixed network operators to setup/teardown calls, to route text (SMS) messages, support inter-network connectivity and transparent roaming, and to provide per-session information such as caller ID. While SS7 was the foundation for signaling in 2G/3G circuit switch networks, Diameter has been introduced for 4G LTE and VoLTE packet networks and IP Multimedia Subsystem (IMS) based systems, and is key to enabling new revenue-generating IP services. Diameter signaling is also implemented in 5G network as there's no changes in requirement in terms of signaling
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

  - Performs Man in The Middle attack by mimicking base station with IMSI catcher. With this hacker can get user's MC (some identification) and connect to the legitimate network with it. Hacker can use this connection to initiate call, sms as the hacked user and track the precise location of the user
  
  - Performs a Denial of Service, by mimicking base station hacker can force the user go to 2G or 3G connection, once the user is using 2G or 3G hacker can sniff all messages and calls.

  Hacker can build this IMSI catcher with $800 
  ```
  source: [NDC Conference: Hacking 4G and how to get arrested in 10 minutes - Christian Sørseth
](https://www.youtube.com/watch?v=DEeOFE_DreU)


