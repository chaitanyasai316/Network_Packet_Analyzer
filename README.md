# Packet Capture Program README

## Overview  
This program captures and analyzes network packets using the `pcap` library. It is designed to display source and destination IP addresses, protocol types (TCP or UDP), and the corresponding port numbers. Additionally, it provides the payload data of the captured packets in hexadecimal format.

## Features  
- Captures packets on the selected network interface.  
- Displays source and destination IP addresses.  
- Identifies and prints the protocol type (TCP/UDP).  
- Outputs source and destination port numbers for TCP and UDP packets.  
- Displays the payload of captured packets in hexadecimal format.

## Requirements  
- C compiler (GCC, Clang, etc.)  
- `libpcap` library installed on your system.  
- Access to a network interface for capturing packets.

## Installation  
1. Ensure you have a C compiler installed on your system.  
2. Install the `libpcap` library:  
   - For **Ubuntu/Debian**: 
    ### sudo apt-get install libpcap-dev
   - For **Fedora**: 
    ### sudo dnf install libpcap-devel
   - For **Windows**: Download and install WinPcap or Npcap.  
3. Compile the program:  
  ### gcc -o packet_capture packet_capture.c -lpcap

## Usage  
1. Run the compiled executable:  
 ### ./packet_capture
2. The program will automatically find and start capturing packets on the default network device.  
3. The captured packet information will be displayed in the console.

## Output  
- The program outputs the following information for each captured packet:  
  - **Source IP**: The IP address of the packet sender.  
  - **Destination IP**: The IP address of the packet receiver.  
  - **Protocol**: Indicates whether the packet is TCP or UDP.  
  - **Source Port**: The port number used by the sender.  
  - **Destination Port**: The port number used by the receiver.  
  - **Payload**: The data carried by the packet, displayed in hexadecimal format.

## Important Notes  
- Running this program may require elevated privileges (administrator or root access) depending on your operating system and network configuration.  
- Be aware of privacy and legal considerations when capturing network traffic. Ensure you have permission to capture packets on the network you are monitoring.

## License  
This program is released under the MIT License. You are free to use, modify, and distribute it, provided that proper credit is given.

## Contact  
For questions or feedback, please contact the author at [your email address].
