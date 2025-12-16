1. Large HTTP Continuation Packets
These appear abnormal because they are large, repetitive, and lack clear request context:

HTTP Continuation packets from 146.75.90.172 → 192.168.0.166 (port 80)
(Multiple frames showing Continuation segments with large payloads)

 2. Reassembled TCP Payloads
Repeated TCP reassembly entries on the same flow, indicating large or unexpected transfers:

146.75.90.172 → 192.168.0.166
(Many [TCP PDU reassembled in 431] packets)

 3. QUIC Activity With Abnormal Resets
Traffic that starts QUIC but ends abruptly with a reset:

QUIC / Protected Payload packets between 192.168.0.112 and 34.87.1.8 / 192.168.223.188

TCP RST terminating a QUIC session from 34.87.1.8 → 192.168.0.112

 4. Spurious TCP Retransmissions
Retransmissions without a clear, successful handshake:

Retransmissions from 192.168.0.112 → 192.168.223.188 

Summary of Suspicious Sources & Flows
Type	Source	Destination	Protocol
Large HTTP continuations	146.75.90.172	192.168.0.166	HTTP/TCP
Reassembled large payloads	146.75.90.172	192.168.0.166	TCP
QUIC with resets	34.87.1.8	192.168.0.112	QUIC/TCP RST
Spurious retransmissions	192.168.0.112	192.168.223.188	TCP
