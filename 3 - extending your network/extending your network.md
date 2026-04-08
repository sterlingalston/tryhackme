### Introduction to Port Forwarding

- Port forwarding is an essential component in connecting applications and services to the Internet. Without port forwarding, applications and services such as web servers are only available to devices within the same direct network.
- ![image](.attachments/d9fbaf21bc6cc1288878e143871954f739be378b.png)
- If the administrator wanted the website to be accessible to the public (using the Internet), they would have to implement port forwarding, like in the diagram below:
- ![image](.attachments/8da92e87b8951afb080dd32e6f81e64500eb7213.png)
- port forwarding is configured at the router of a network

### Firewalls 101

- **firewall** is a device within a network responsible for determining what traffic is allowed to enter and exit
- it can **permit** and **deny** traffic from entering or exiting based on factors:
  - Where the traffic is coming from? (has the firewall been told to accept/deny traffic from a specific network?)
  - Where is the traffic going to? (has the firewall been told to accept/deny traffic destined for a specific network?)
  - What port is the traffic for? (has the firewall been told to accept/deny traffic destined for port 80 only?)
  - What protocol is the traffic using? (has the firewall been told to accept/deny traffic that is UDP, TCP or both?)

- can be a device of software (i.e.g _Snort_)
  - ![image](.attachments/05f09c505fdf7c3782b4786679a25915c88eab1f.png)

Categories of Firewalls

|     |     |
| --- | --- |
| **Firewall Category** | **Description** |
| Stateful | This type of firewall uses the entire information from a connection; rather than inspecting an individual packet, this firewall determines the behaviour of a device **based upon the entire connection**.<br><br>This firewall type consumes many resources in comparison to stateless firewalls as the decision making is dynamic. For example, a firewall could allow the first parts of a TCP handshake that would later fail.<br><br>If a connection from a host is bad, it will block the entire device. |
| Stateless | This firewall type uses a static set of rules to determine whether or not **individual packets** are acceptable or not. For example, a device sending a bad packet will not necessarily mean that the entire device is then blocked.<br><br>Whilst these firewalls use much fewer resources than alternatives, they are much dumber. For example, these firewalls are only effective as the rules that are defined within them. If a rule is not exactly matched, it is effectively useless.<br><br>However, these firewalls are great when receiving large amounts of traffic from a set of hosts (such as a Distributed Denial-of-Service attack) |