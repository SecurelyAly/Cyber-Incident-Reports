<h1>File permissions in Linux</h1>

 

<h2>Description</h2>
This repository contains scripts and documentation for managing and securing file and directory permissions within a Linux environment. The primary focus is on practical commands and strategies to adjust file permissions according to security needs, especially in environments where sensitive data is managed or multiple users access the same system resources.
<br />


<h2>Project Overview</h2>

- <b>Assessment of Current Permissions:</b> Utilizing commands like ls -l and ls -ld to list files and directories along with detailed permissions, ownership, and other attributes, which is essential for evaluating current security settings.
- <b>Understanding Permissions Strings:</b> Detailed explanation and examples of permissions strings which define access levels for different user types:

File Type Indicator: (e.g., d for directory, - for file)
Owner Permissions: (e.g., rwx)
Group Permissions: (e.g., rwx)
Others Permissions: (e.g., rwx)
- <b>Modifying File Permissions:</b> Practical usage of the chmod command to change permissions, illustrated through real-world examples:
Restricting and granting access using both numeric and symbolic methods.
Special focus on handling hidden files and directories.
- <b>Real-World Scenarios:</b>  Step-by-step walkthroughs on how permissions are modified to meet specific operational requirements or security policies within an organization.
- 
<h2>Learning Outcomes: </h2>

- <b>Framework Application:</b> Application of the NIST cybersecurity framework in a real-life context, with detailed notes on how each phase—Identify, Protect, Detect, Respond, and Recover—was addressed during the incident.  
- <b>Technical Documentation:</b> In-depth analysis and technical documentation of the attack, response actions, and recovery processes, providing a blueprint for handling similar security incidents in the future.
- <b>Security Improvements:</b> Post-incident enhancements to our cybersecurity posture, including the implementation of new firewall rules, source IP address verification, deployment of network monitoring software, and integration of an IDS/IPS system.


# Incident Report Analysis


## Summary

The organization experienced a DDoS attack that disrupted internal network services for two hours. The attack involved a flood of ICMP packets overwhelming the network. The incident management team responded by blocking incoming ICMP packets and restoring critical network services. Investigation revealed that an unconfigured firewall allowed the attack, prompting the implementation of new firewall rules, source IP address verification, network monitoring software, and an IDS/IPS system. This event underscores the need for enhanced network security measures to prevent future attacks and ensure the integrity of the company's network infrastructure.

## Incident Phases

| Phase     | Description |
|-----------|-------------|
| Identify  | The identification process following the DDoS attack involved a comprehensive audit of our internal networks, systems, devices, and access privileges. Every aspect of our network infrastructure was meticulously examined to identify potential vulnerabilities and gaps in security. Through this thorough investigation, we discovered that the attack was facilitated by an unconfigured firewall, which allowed a flood of ICMP packets to overwhelm our network. This critical insight provided the foundation for our subsequent efforts to bolster our defenses and prevent future security breaches|
| Protect   | To protect the organization following the DDoS attack, several measures were implemented to mitigate cybersecurity threats. First, a new firewall rule was established to limit the rate of incoming ICMP packets, preventing similar attacks from overwhelming our network infrastructure. Additionally, source IP address verification was enforced on the firewall to detect and block spoofed IP addresses associated with incoming ICMP packets, enhancing our defense mechanisms against malicious actors. Furthermore, network monitoring software was deployed to detect abnormal traffic patterns, enabling us to swiftly identify and respond to potential security incidents in real-time. Lastly, an IDS/IPS system was integrated to filter out suspicious ICMP traffic, providing an additional layer of protection against DDoS attacks and other cybersecurity threats. These proactive measures collectively fortified our organization's security posture and bolstered our resilience against future attacks. |
| Detect    | The attack was detected through the implementation of network monitoring software, which enabled us to observe and analyze traffic patterns in real-time. The abnormal influx of ICMP packets into our network, causing a sudden surge in traffic, was flagged as suspicious activity by the monitoring system. Additionally, the IDS/IPS system played a crucial role in identifying and filtering out ICMP traffic exhibiting characteristics indicative of a DDoS attack. By continuously monitoring network traffic and employing advanced threat detection mechanisms, we were able to swiftly detect the attack and initiate appropriate response measures to mitigate its impact on our organization. |
| Respond   | In response to the attack, several immediate measures were taken to contain and neutralize the threat. The incident management team promptly blocked incoming ICMP packets to halt the ongoing DDoS attack and prevent further disruption to our network services. Non-critical network services were temporarily taken offline to mitigate the impact of the attack, while critical services were restored to ensure essential business operations continued uninterrupted. Additionally, the cybersecurity team implemented a new firewall rule to limit the rate of incoming ICMP packets and conducted source IP address verification to identify and block spoofed IP addresses associated with the attack. Furthermore, an IDS/IPS system was deployed to filter out suspicious ICMP traffic and enhance our network defenses against similar threats in the future. These response measures effectively mitigated the immediate impact of the attack and reinforced our network security posture against potential future incidents. |
| Recover   | Following the attack, efforts were directed towards the recovery and restoration of affected systems to ensure normal operations resumed swiftly. The incident management team initiated the recovery process by conducting a thorough assessment of the damage caused by the DDoS attack. Affected systems and network infrastructure were meticulously inspected to identify any compromised or disrupted components. Subsequently, a comprehensive plan for system restoration was devised, prioritizing critical systems and data for recovery. Systems were restored to their pre-attack state using backup data and configurations, with a focus on minimizing downtime and restoring normal operations as quickly as possible. Continuous monitoring and testing were conducted to verify the effectiveness of the recovery efforts and ensure the integrity of restored systems. Additionally, measures were implemented to strengthen the resilience of our network infrastructure against similar attacks in the future, including updates to firewall configurations, network monitoring protocols, and incident response procedures. Through these concerted recovery efforts, the organization successfully mitigated the impact of the DDoS attack and restored business continuity. |




## Learning Outcomes

This project applies the NIST cybersecurity framework in a practical scenario, providing insights into real-world challenges in cybersecurity incident response. It serves as a valuable educational tool for cybersecurity professionals and students, illustrating effective strategies for incident management and recovery.





<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
