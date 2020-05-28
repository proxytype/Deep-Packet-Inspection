# Deep Packet Inspection
Using Iptables rules for redirect traffic to queues, the main function create array of threads, each thread connect to different queue, when packet arrived to the queue a callback function start to analyze the packet and drop it if it's found specific string in the payload, this mechanism can help you build IPS/IDS/WAF applications.

add libraries to the linker
pthread,netlink and libnetfilter_queue,

make sure libnetfilter_queue installed in your system:<br />
#: yum install libnetfilter_queue<br />
#: yum install libnetfilter_queue-devel
