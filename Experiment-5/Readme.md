<h1>Experiment 5</h1>

<h2>Implement error detection and correction mechanisms using block coding and CRC. Simulate a communication system that demonstrates how errors are detected and corrected during data transmission.</h2>

<h3>1. Theory:</h3>
   
<h4>a. Block Coding:</h4>
Data is divided into discrete blocks, and redundant parity bits are appended to detect and correct single-bit errors. By adding these extra bits, the receiver can verify if the data received matches the data sent.

<h4>b. CRC (Cyclic Redundancy Check):</h4>
A mathematical division process used to detect accidental changes to raw data. The sender calculates a check value based on binary division and appends it to the frame as the Frame Check Sequence (FCS).

<h3>2. Network Topology:</h3>

<h4>- Step-by-step Procedure:</h4>
  - Topology Setup: Created a new network topology using End Devices (PCs) and a central Switch.
  - IP Addressing:  Assigned static IP addresses to the PCs.
  - Documentation:  Used the "Add Note" feature in Packet Tracer to document the theoretical application of block coding and parity bits for error checking within the workspace.
  - Traffic Generation:  Generated ICMP (ping) traffic using the Add Simple PDU tool to simulate data transmission.
  - Packet Inspection:  Switched to Simulation Mode to observe the packet headers, specifically inspecting the Ethernet II frame to view the CRC/FCS trailer used for error detection.
  
<h2>4. Configuration Commands:</h2>

N/A (This experiment relies on packet inspection rather than CLI configuration).

<h2>5. Observations / Results:</h2>
   
PDU Details
- Inspected the outbound PDU details in Simulation Mode.
- While physical bit-flipping isn't manually configurable in the GUI, the simulation allowed for the visualization of the FCS trailer, confirming the implementation of CRC at the data link layer.
  
<h2>6. Conclusion:</h2>
Successfully simulated a communication system demonstrating error detection concepts. The experiment highlighted the practical application of CRC in standard Ethernet frames to ensure data integrity over a network.
