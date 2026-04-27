<h1>Experiment 8</h1>

<h2>Objective</h2>

Create a simulation to demonstrate logical addressing using IPv4 and IPv6 and 33IPv6. Implement address mapping techniques such as ARP, RARP, BOOTP and DHCP to show how devices acquire and resolve addresses.

<h2>Theory</h2>

- <h3>DHCP (Dynamic Host Configuration Protocol)</h3>: Automatically assigns IP addresses and network configuration (such as subnet masks and default gateways) to client devices.

- <h3>ARP (Address Resolution Protocol):</h3> Resolves a known logical IP address to an unknown physical MAC address to facilitate local network communication.

- <h3>IPv6:</h3> The next-generation protocol providing a massively expanded 128-bit address space, designed to replace IPv4.

<h2>Network Topology</h2>

![Topology](Topology.jpeg)

(Above: A network topology including a DHCP Server, a Router, a Switch, and client PCs).

<h3>Step-by-step Procedure</h3>

1. <h4>Topology Design:</h4> Designed a network topology including PCs, a Router, a Switch, and a Server.
2. <h4>Static Configuration:</h4> Assigned static IPv4 and IPv6 addresses to the Server and Router interfaces.
3. <h4>DHCP Setup:</h4> Accessed the Server's Services tab, enabled DHCP, and configured a pool with a range of IP addresses, subnet mask, and default gateway.
4. <h4>Client Configuration:</h4> Configured the PCs to acquire their IP addresses via DHCP instead of static entry.
5. <h4>ARP Simulation:</h4> Opened the Command Prompt on PC0 and pinged PC1 to initiate an ARP request. Switched to Simulation Mode to observe the ARP broadcast and the resulting MAC address resolution.
6. <h4>Verification:</h4> Verified communication using both IPv4 and IPv6 ping commands to ensure end-to-end connectivity.

<h2>Configuration Commands</h2>
N/A (Configurations handled via GUI menus for PC interfaces and Server services).

<h2>Observations / Results</h2>

- The client PCs successfully acquired dynamic IPv4 configurations from the DHCP server via the DORA (Discover, Offer, Request, Acknowledge) process.
  
- The simulation visually captured the ARP Request broadcasting to all switch ports, followed by the unicast ARP Reply returning the target MAC address.
  
<h2>Conclusion</h2>

Successfully demonstrated IPv4 and IPv6 logical addressing. The implementation of DHCP streamlined address allocation, while the simulation mode provided clear visualization of the ARP mapping techniques required for packet delivery.
