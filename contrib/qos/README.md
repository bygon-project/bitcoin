### Qos ###

This is a Linux bash script that will set up tc to limit the outgoing bandwidth for connections to the Bygon network. It limits outbound TCP traffic with a source or destination port of 9333, but not if the destination IP is within a LAN (defined as 192.168.x.x).

This means one can have an always-on bygond instance running, and another local bygond/bygon-qt instance which connects to this node and receives blocks from it.
