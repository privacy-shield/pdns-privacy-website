---
title: pDNS?
subtitle: What is pDNS?
layout: default
modal-id: pDNS
order: 1
---
<!--div class="container-fluid"-->
  <div class="row">
    <div class="col-md-12 text-left">
      <h3 class="section-heading">What Is pDNS?</h3>
      <p class="lead">
        The pDNS is short for Passive Domain Name System, a technique commonly used for security and network monitoring purposes. While <a href="https://en.wikipedia.org/wiki/Domain_Name_System">DNS</a> (Domain Name System) serves as the protocol that translates human-readable domain names (i.e. www.mydomain.com) into IP addresses for enabling communication between devices over the internet, pDNS goes a step further. Instead of actively querying DNS servers, pDNS sensors observes and records DNS response data that has already been made, either by other users, systems, or devices. pDNS is written with a lowercase "p" to be recognizable among other projects which using the same acronym. It also highlights the "passive" nature of the technique which helps lowering the workload from the DNS servers.
      </p>
      <img src="{{ '/img/portfolio/dns_flowchart.jpg' | relative_url }}" alt="pDNS Flowchart" style="max-width: 100%; height: auto; margin: 20px 0;">
      <p class="lead">
       With pDNS, security teams can discover potential access to a malicious infrastructure, detect suspicious behavior, and even investigate incidents after they occur, without compromising users' communication privacy. In the recommended setup, pDNS does not collect personally identifiable information; instead, it logs only anonymized DNS server response data. This can be turned into an effective tool for cybersecurity monitoring while respecting user privacy.
      </p>
      <h3 class="section-heading">Why pDNS privacy matters</h3>
      <p class="lead">
      As cyberattacks have become more sophisticated, modern threat actors often begin with reconnaissance, using techniques like <a href="https://attack.mitre.org/techniques/T1590/002/">T1590.002</a> (Gather Victim Network Information – DNS) and <a href="https://attack.mitre.org/techniques/T1596/001">T1596.001</a> (Active Scanning – DNS/Passive DNS) from the MITRE ATT&CK framework to leverage DNS data for gathering critical information, affecting individual user browsing privacy and organization security. The pDNS Shield project is an enabler that is aimed to encourage users provide pDNS data openly without compromise of their privacy and security.</p>
      <h4>Individual User browsing Privacy</h4>
      <p class="lead">
      pDNS records when accessed from the database can reveal browsing activities of users, which can be exploited by advertisers, trackers and potenial malicious actors. This prevents users' anonymity and leaks sensitive behavioral information that can lead to phishing and targeted exploitation.
      </p>
      <h4>Organizational Security</h4>
      <p class="lead">
      For organization unprotected pDNS data exposes valuable insights about their internal networks, external communication that attackers can use to either exploit business relations or plan intrusions like watering hole attacks. 
      </p>
    </div>
  </div>
<!--/div-->
