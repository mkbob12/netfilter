# netfilter


# packet to netfiler
 * sudo iptables -F
 * sudo iptables -A OUTPUT -j NFQUEUE --queue-num 0
 * sudo iptables -A INPUT -j NFQUEUE --queue-num 0

# RUN COMMAND 
 * gcc -o nfqnl_test nfqnl_test.c -lnetfilter_queue
 * sudo ./nfqnl_test


