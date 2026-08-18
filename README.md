<h1>VLAN's on Fortigate and Cisco Switch</h1>

![](https://github.com/rbrianshutt/vlan_on_fortigate_and_cisco_switch/blob/main/VLAN%20on%20Fortigate%20and%20Cisco%20switch/2026-07-11%2023_34_07-Ubuntu%2064-bit%20-%20VMware%20Workstation.png)

<h2>Description</h2>
x
<br />

<h2>Techonologies Used</h2>

- <b>EVE-NG for my homelab</b>
- <b>Fortigate</b>
- <b>Cisco Core Switch</b>
- <b>Cisco Access Switches</b>
- <b>VLAN's</b>
- <b>Firewall policies</b>


<h2>Overview:</h2>

- <b>Fortigate setup and configuration of VLAN's and firewall policies</b> 
- <b>Configure Cisco Core switch and Cisco Access switches</b>
- <b>x</b>
- <b>x</b>
- <b>x</b>
- <b>x</b>
- <b>x</b>

<h2>Program Walk-Through:</h2>

<h1>Fortigate setup and configuration of VLAN's and firewall policies</h1>

Setup port 1 as our WAN connection to the internet<br/>
Click port 1<br/>

![](https://github.com/rbrianshutt/vlan_on_fortigate_and_cisco_switch/blob/main/VLAN%20on%20Fortigate%20and%20Cisco%20switch/2026-07-11%2012_39_29-Fortigate.png)
<br />

Enter alias as WAN1<br/>
Set role to WAN<br/>
Click OK<br/>

![](https://github.com/rbrianshutt/vlan_on_fortigate_and_cisco_switch/blob/main/VLAN%20on%20Fortigate%20and%20Cisco%20switch/2026-07-11%2012_40_48-.png)
<br />

You can see WAN1 is setup on port 1<br/>

![](https://github.com/rbrianshutt/vlan_on_fortigate_and_cisco_switch/blob/main/VLAN%20on%20Fortigate%20and%20Cisco%20switch/2026-07-11%2012_41_40-Fortigate.png)
<br />

<h2>Create VLAN 10 and VLAN 20</h2>

Go to Network -> Interfaces -> Create New -> Interface  <br/>

![](https://github.com/rbrianshutt/vlan_on_fortigate_and_cisco_switch/blob/main/VLAN%20on%20Fortigate%20and%20Cisco%20switch/2026-07-11%2012_43_08-Fortigate.png)
<br />

Fill in Name as VLAN10, Alias as VLAN10, Type as VLAN, Interface (port 2), VLAN ID as 10, Role as LAN <br/>
Set IP/Netmask to 10.10.10.1/24<br/>
Enable what you would like to allow in administrative access<br/>
Enable DHCP<br/>
Click OK<br/>

![](https://github.com/rbrianshutt/vlan_on_fortigate_and_cisco_switch/blob/main/VLAN%20on%20Fortigate%20and%20Cisco%20switch/2026-07-11%2012_44_33-Fortigate.png)
<br />

Create VLAN20 similar to VLAN10  <br/>
Set IP/Netmask to 20.20.20.1/24<br/>

![](https://github.com/rbrianshutt/vlan_on_fortigate_and_cisco_switch/blob/main/VLAN%20on%20Fortigate%20and%20Cisco%20switch/2026-07-11%2012_46_54-.png)
<br />

If you expand port 2 you will see both VLAN's created <br/>

![](https://github.com/rbrianshutt/vlan_on_fortigate_and_cisco_switch/blob/main/VLAN%20on%20Fortigate%20and%20Cisco%20switch/2026-07-11%2012_48_15-Fortigate.png)
<br />

<h2>Create static route</h2>

Network -> Static Routes -> Create New<br/>
Ensure destination set to 0.0.0.0/0.0.0.0<br/>
Set gateway address to 192.168.133.2 as our default gateway <br/>
Ensure interface is set to port 1 as WAN1<br/>
Click OK<br/>

![](https://github.com/rbrianshutt/vlan_on_fortigate_and_cisco_switch/blob/main/VLAN%20on%20Fortigate%20and%20Cisco%20switch/2026-07-11%2012_49_11-Fortigate.png)
<br />
![](https://github.com/rbrianshutt/vlan_on_fortigate_and_cisco_switch/blob/main/VLAN%20on%20Fortigate%20and%20Cisco%20switch/2026-07-11%2012_49_44-Fortigate.png)
<br />

<h2>Create firewalls policies</h2>

Lorem ipsum  <br/>

![]()
<br />

