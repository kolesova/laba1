laba1
====
ip net a h2

ip net a h3

ip net a h4

ip l a eth_h2 type veth peer name eth1

ip l s eth1 netns h2

ip net e h2 ip l s eth1 up

ip l a eth_h3 type veth peer name eth1

ip l s eth1 netns h3

ip net e h3 ip l s eth1 up


ip l a eth_h4 type veth peer name eth1

ip l s eth1 netns h4

ip net e h4 ip l s eth1 up

