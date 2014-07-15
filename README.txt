Name: Gateway Administration

Description: You've been given the awesome responsibility of running a gateway
node between two large networks. Everything flows through this node.
Naturally, you've set up a packet caputuring tool. [Here's] today's traffic.
See if there's anything juicy?

How to Solve: Open the packet capture with Wireshark. Use the VoIP functionality
to look for SIP conversations. There should be two. Both are calls to the
`Temperance Bank' helpdesk. One references Phillip J. Fry's (Futurama) 
bank pin (1077) and the other references the place where Zeno of Citium taught
(the Painted Porch, or Stoa Poikile).

Additionally, there is a PNG file transmitted in the packet capture. It 
contains a hexadecimal pin pad (as to an ATM). This will give the hint that
the flag is a hex string composed of two pin numbers. These are 1077 and 570A
(stoa) respectively. When put together with MCA-, they give a flag.

What to distribute:
dist/challenge.pcap

Flag: MCA-1077570A
