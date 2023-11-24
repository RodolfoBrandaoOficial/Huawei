# Huawei NE20/NE40/NE80 Router Commands 🌐

This repository contains a comprehensive list of commands for configuring and managing Huawei NE20, NE40, and NE80 routers. These commands are valuable for network administrators and engineers working with Huawei router equipment. 💼

## Version and Patch Information 📌

- Display current software version: `display version` 📋
- Display all patches: `display patch all` 🛠️

## Configuration ⚙️

- Display current configuration: `display current-configuration` 📄
- Save configuration: `save` 💾
- Display specific configuration sections:
  - Interface configuration: `display current-configuration | section interface` ⚙️
  - Routing configuration: `display current-configuration | section route` 🌐
  - Security configuration: `display current-configuration | section security` 🔒
  - QoS configuration: `display current-configuration | section qos` 📶
  - NAT configuration: `display current-configuration | section nat` 🌍
  - BGP configuration: `display current-configuration | section bgp` 📡
  - OSPF configuration: `display current-configuration | section ospf` 🌐
  - SNMP configuration: `display current-configuration | section snmp` 📜
  - Global configuration: `display current-configuration | section global` 🌍

## Search Configuration 🔍

- Search for specific text in the configuration: `display current-configuration | include <text>` 🧐

## Interface Configuration ⚙️

- Display interface status: `display interface brief` ⚙️
- Configure interface description: `interface <interface>`, `description <description>` ⚙️
- Configure interface IP address: `interface <interface>`, `ip address <ip-address> <subnet-mask>` 🌐
- Configure interface shutdown: `interface <interface>`, `shutdown` ⚙️
- Configure interface port mode: `interface <interface>`, `port link-type <access/trunk/hybrid>` ⚙️
- Configure VLAN assignment on an interface: `interface <interface>`, `port default vlan <vlan-id>` 📶

## Routing Configuration 🌐

- Display IP routing table: `display ip routing-table` 🌐
- Configure static route: `ip route-static <destination> <mask> <next-hop>` 🌍
- Configure BGP routing: `bgp <as-number>` 📡
- Configure OSPF routing: `ospf <process-id>` 🌐
- Configure RIP routing: `rip` 🌍

## Security 🔒

- Configure ACL (Access Control List): `acl number <acl-number>`, `rule <rule-id> permit/deny <protocol> <source-ip> <source-mask> <destination-ip> <destination-mask> [match-order <match-order>]` 🔒
- Apply ACL to an interface: `interface <interface>`, `packet-filter <acl-number> inbound/outbound` 🔒
- Configure AAA (Authentication, Authorization, Accounting): `aaa` 🔒
- Configure Port Security: `interface <interface>`, `port-security enable`, `port-security max-mac-num <max-mac-num>` 🔒
- Configure NAT (Network Address Translation): `nat outbound <interface> <acl-number>` 🔒
- Configure VPN (Virtual Private Network): `vpn-instance <vpn-instance-name>` 🔒
- Configure Firewall: `firewall` 🔒

## QoS 📶

- Configure QoS policy: `qos policy <policy-name>` 📶
- Configure traffic behavior: `qos behavior <behavior-name>` 📶
- Apply QoS policy to an interface: `interface <interface>`, `qos apply policy <policy-name>` 📶
- Configure CAR (Committed Access Rate): `car <car-name> cir <cir-value> cbs <cbs-value>` 📶
- Configure WRED (Weighted Random Early Detection): `wred <wred-name>` 📶

## SNMP Configuration 📡

- Configure SNMP version: `snmp-agent sys-info version <v1/v2c/v3>` 📡
- Configure SNMP community: `snmp-agent community read <community-name> acl <acl-number>` 📡
- Configure SNMP trap receiver: `snmp-agent target-host trap address udp-domain <ip-address> params securityname <security-name> v1v2c` 📡

## Logs and Monitoring 📜

- Display logs: `display logbuffer` 📜
- Display CPU usage: `display cpu-usage` 💻
- Monitor traffic on an interface: `display interface <interface> traffic` 📈
- Display MAC address table: `display mac-address` 📜

## Miscellaneous 🛠️

- Other useful commands like `display arp`, `display interface description`, `display vlan`, `display dhcp server`, `display dhcp client`, etc.

Feel free to explore and use these commands as needed for managing Huawei NE20, NE40, and NE80 routers. 🚀

---

## All Commands 📜

Here is a comprehensive list of all Huawei NE20, NE40, and NE80 router commands mentioned in this repository:

### Version and Patch Information 📌

- `display version`
- `display patch all`

### Configuration ⚙️

- `display current-configuration`
- `save`
- `display current-configuration | section interface`
- `display current-configuration | section route`
- `display current-configuration | section security`
- `display current-configuration | section qos`
- `display current-configuration | section nat`
- `display current-configuration | section bgp`
- `display current-configuration | section ospf`
- `display current-configuration | section snmp`
- `display current-configuration | section global`

### Search Configuration 🔍

- `display current-configuration | include <text>`

### Interface Configuration ⚙️

- `display interface brief`
- `interface <interface>`, `description <description>`
- `interface <interface>`, `ip address <ip-address> <subnet-mask>`
- `interface <interface>`, `shutdown`
- `interface <interface>`, `port link-type <access/trunk/hybrid>`
- `interface <interface>`, `port default vlan <vlan-id>`

### Routing Configuration 🌐

- `display ip routing-table`
- `ip route-static <destination> <mask> <next-hop>`
- `bgp <as-number>`
- `ospf <process-id>`
- `rip`

### Security 🔒

- `acl number <acl-number>`, `rule <rule-id> permit/deny <protocol> <source-ip> <source-mask> <destination-ip> <destination-mask> [match-order <match-order>]`
- `interface <interface>`, `packet-filter <acl-number> inbound/outbound`
- `aaa`
- `interface <interface>`, `port-security enable`, `port-security max-mac-num <max-mac-num>`
- `nat outbound <interface> <acl-number>`
- `vpn-instance <vpn-instance-name>`
- `firewall`

### QoS 📶

- `qos policy <policy-name>`
- `qos behavior <behavior-name>`
- `interface <interface>`, `qos apply policy <policy-name>`
- `car <car-name> cir <cir-value> cbs <cbs-value>`
- `wred <wred-name>`

### SNMP Configuration 📡

- `snmp-agent sys-info version <v1/v2c/v3>`
- `snmp-agent community read <community-name> acl <acl-number>`
- `snmp-agent target-host trap address udp-domain <ip-address> params securityname <security-name> v1v2c`

### Logs and Monitoring 📜

- `display logbuffer`
- `display cpu-usage`
- `display interface <interface> traffic`
- `display mac-address`

### Miscellaneous 🛠️

- Other useful commands like `display arp`, `display interface description`, `display vlan`, `display dhcp server`, `display dhcp client`, etc.

Feel free to explore and use these commands as needed for managing Huawei NE20, NE40, and NE80 routers. 🚀
