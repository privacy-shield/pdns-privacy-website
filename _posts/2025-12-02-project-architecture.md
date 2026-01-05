---
title: Components
subtitle: Design Layers
layout: default
modal-id: ProjArch
order: 2
---
<!--div class="container-fluid"-->
  <div class="row">
    <div class="col-md-12 text-left">
      <p class="lead">Privacy focused pDNS collection system must be based on the three key layers or components: sensor, shield, and collector.</p>
      <img src="{{ '/img/portfolio/comp_flow.png' | relative_url }}" alt="Component Flowchart" style="max-width: 100%; height: auto; margin: 20px 0;">
      <h4 class="section-heading">
      Sensor
      </h4>
      <p class="lead"> The sensor sits near the DNS resolver and batches up DNS responses and sends them over to privacy shield.</p>
      <h4 class="section-heading">
      Privacy Shield
      </h4>
      <p class="lead"> The Privacy Shield ensures that pDNS data is anonymized and secured to protect user privacy. It acts as a filter that prevents personally identifiable information (PII) or sensitive internal data from being exposed while still allowing the analysis of DNS responses for security purposes. This shield is essential for ensuring compliance with data privacy laws and maintaining confidentiality while using pDNS data for network monitoring and threat detection. It also serves as a mixer for several source streams making it even harder to even guess a possible source of the pDNS record.</p>
      <h4 class="section-heading">
      Collector
      </h4>
      <p class="lead"> The pDNS collector is responsible for storing and aggregating the DNS query data captured by sensors. It organizes and stores the data in a centralized database for further analysis. The collector helps maintain historical records of DNS responses, which can be used for forensics, incident response, and identifying long-term patterns or trends in network behavior.</p>
      <h3 class="section-heading">Data protocols</h3>
      <p class="lead">
       The sensor sends DNS responses to the shield via encrypted UDP packets. The data is accumulated for some time before being submitted to the pDNS Collector. The Collector receives, decrypts and validates the data integrity. The data is subsequently stored and used for analysis. Throughout the process, a heartbeat mechanism is used at all levels to ensure liveness of the system components and allowing real-time response to potential network issues or a hardware malfunction.
      </p>
    </div>
  </div>
<!--/div-->
