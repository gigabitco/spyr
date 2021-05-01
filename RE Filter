# SPYR re-Filter Implementation
# 4-29-21
#
set interfaces lo0 unit 0 family inet address 127.0.0.1/32
set interfaces lo0 unit 0 family inet filter input protect-RE
set firewall filter protect-RE interface-specific
set firewall filter protect-RE term ssh from source-address 162.249.33.128/27
set firewall filter protect-RE term ssh from source-address 23.135.176.25/32
set firewall filter protect-RE term ssh from destination-port ssh
set firewall filter protect-RE term ssh from destination-port telnet
set firewall filter protect-RE term ssh then accept
set firewall filter protect-RE term SSH-DENY from destination-port ssh
set firewall filter protect-RE term SSH-DENY from destination-port telnet
set firewall filter protect-RE term SSH-DENY then discard
set firewall filter protect-RE term LDP-ALLOWED from source-address 100.0.0.0/8
set firewall filter protect-RE term LDP-ALLOWED from destination-address 224.0.0.2/32
set firewall filter protect-RE term LDP-ALLOWED from destination-address 100.0.0.0/8
set firewall filter protect-RE term LDP-ALLOWED from protocol tcp
set firewall filter protect-RE term LDP-ALLOWED from protocol udp
set firewall filter protect-RE term LDP-ALLOWED from destination-port ldp
set firewall filter protect-RE term LDP-ALLOWED then accept
set firewall filter protect-RE term LDP-DENY from protocol tcp
set firewall filter protect-RE term LDP-DENY from protocol udp
set firewall filter protect-RE term LDP-DENY from destination-port ldp
set firewall filter protect-RE term LDP-DENY then discard
set firewall filter protect-RE term BGP from protocol tcp
set firewall filter protect-RE term BGP from destination-port bgp
set firewall filter protect-RE term BGP then accept
set firewall filter protect-RE term BGP-DENY from protocol tcp
set firewall filter protect-RE term BGP-DENY from destination-port bgp
set firewall filter protect-RE term BGP-DENY then discard
set firewall filter protect-RE term SNMP-ALLOWED from source-address 162.249.33.128/27
set firewall filter protect-RE term SNMP-ALLOWED from source-address 172.16.31.0/24
set firewall filter protect-RE term SNMP-ALLOWED from source-address 23.135.176.25/32
set firewall filter protect-RE term SNMP-ALLOWED from destination-port snmp
set firewall filter protect-RE term SNMP-ALLOWED from destination-port syslog
set firewall filter protect-RE term SNMP-ALLOWED then accept
set firewall filter protect-RE term SNMP-DENY from destination-port snmp
set firewall filter protect-RE term SNMP-DENY from destination-port syslog
set firewall filter protect-RE term SNMP-DENY then reject
set firewall filter protect-RE term icmp from protocol icmp
set firewall filter protect-RE term icmp from icmp-type echo-request
set firewall filter protect-RE term icmp from icmp-type echo-reply
set firewall filter protect-RE term icmp from icmp-type unreachable
set firewall filter protect-RE term icmp from icmp-type time-exceeded
set firewall filter protect-RE term icmp then accept
set firewall filter protect-RE term RSVP from protocol tcp
set firewall filter protect-RE term RSVP from protocol udp
set firewall filter protect-RE term RSVP from port 3455
set firewall filter protect-RE term RSVP then accept
set firewall filter protect-RE term TCP-ESTABLISHED from tcp-flags "(ack | rst)"
set firewall filter protect-RE term TCP-ESTABLISHED then accept
set firewall filter protect-RE term OSPF from protocol ospf
set firewall filter protect-RE term OSPF then accept
set firewall filter protect-RE term VRRP from protocol vrrp
set firewall filter protect-RE term VRRP then accept
set firewall filter protect-RE term TRACEROUTE from protocol udp
set firewall filter protect-RE term TRACEROUTE from destination-port 33434-33523
set firewall filter protect-RE term TRACEROUTE then accept
set firewall filter protect-RE term DOMAIN from protocol udp
set firewall filter protect-RE term DOMAIN from port domain
set firewall filter protect-RE term DOMAIN then accept
set firewall filter protect-RE term OTHER then log
set firewall filter protect-RE term OTHER then syslog
set firewall filter protect-RE term OTHER then discard
####
