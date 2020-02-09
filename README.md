# rpiawsvpn
aws vpn with a raspberry Pi

This is an example config for AWS lan-to-lan VPN, using libreswan with a VTI interface, and BGPd routing via FRR.

Tests were conducted using a rPi4 with 4gb memory, and a 300mb/s comcast/xfinity internet connection.

Total throughput seems to max out at 180mb/s, due to raspberry Pi hardware limitations (tested with iperf).

tested on rasbian linux 10 (buster)

install necessary packages

#apt-get install frr libreswan lsof

you can't terminate both tunnels on one rPi, so spend the extra $35 and get some real redundancy

