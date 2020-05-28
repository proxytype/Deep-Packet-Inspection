# Deep-Packet-Inspection
using iptables rules for redirect traffic to queues, the main function create array of threads, each thread connect to different queue, when packet arrived to the queue a callback function start to analyze the packet and drop it if it's found specific string in the payload, this mechanism can help you build IPS/IDS/WAF applications.
