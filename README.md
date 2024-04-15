<h1>File permissions in Linux</h1>

 

<h2>Description</h2>
This repository contains scripts and documentation for managing and securing file and directory permissions within a Linux environment. The primary focus is on practical commands and strategies to adjust file permissions according to security needs, especially in environments where sensitive data is managed or multiple users access the same system resources.
<br />


<h2>Project Overview</h2>

- <b>Assessment of Current Permissions:</b> Utilizing commands like ls -l and ls -ld to list files and directories along with detailed permissions, ownership, and other attributes, which is essential for evaluating current security settings.
- <b>Understanding Permissions Strings:</b> Detailed explanation and examples of permissions strings which define access levels for different user types:
 <p> <blockquote> &#8728;File Type Indicator: (e.g., d for directory, - for file) </blockquote> </p>
 <p> <blockquote> &#8728; Owner Permissions: (e.g., rwx) </blockquote> </p>
 <p> <blockquote> &#8728; Group Permissions: (e.g., rwx) </blockquote> </p>
 <p> <blockquote> &#8728; Others Permissions: (e.g., rwx) </blockquote> </p>

- <b>Modifying File Permissions:</b> Practical usage of the chmod command to change permissions, illustrated through real-world examples:
<p> <blockquote> &#8728; Restricting and granting access using both numeric and symbolic methods.</blockquote> </p>
<p> <blockquote> &#8728; Special focus on handling hidden files and directories. </blockquote> </p>
- <b>Real-World Scenarios:</b>  Step-by-step walkthroughs on how permissions are modified to meet specific operational requirements or security policies within an organization.

<h2>Contents: </h2>

- <b> Scripts:</b> Scripts used to modify and manage file and directory permissions.
- <b> Documentation:</b> Detailed explanations of each script and command used.
- <b>Case Studies:</b> Practical applications and scenario-based examples demonstrating how to secure a Linux file system effectively.



## Usage

The organization experienced a DDoS attack that disrupted internal network services for two hours. The attack involved a flood of ICMP packets overwhelming the network. The incident management team responded by blocking incoming ICMP packets and restoring critical network services. Investigation revealed that an unconfigured firewall allowed the attack, prompting the implementation of new firewall rules, source IP address verification, network monitoring software, and an IDS/IPS system. This event underscores the need for enhanced network security measures to prevent future attacks and ensure the integrity of the company's network infrastructure.

<b>Checking File and Directory Details: </b>
bash
ls -l
ls -la

<b> Changing File Permissions: </b>
bash
chmod o-w project_k.txt
ls -la # Confirming the changes

<b> Securing Hidden Files: </b>
bash
chmod u-w .project_x.txt
chmod g-w .project_x.txt
chmod g+r .project_x.txt

<b> Modifying Directory Access: </b>
bash
chmod go-x drafts


## Summary

This project enhances the understanding and application of Linux file permissions to ensure that files and directories are secured as per the organizational requirements. By employing a combination of command-line tools and scripts, users can effectively manage and safeguard their Linux environments against unauthorized access.


