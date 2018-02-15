---
layout: post
title: query snmp from vbscript
---

if anyone finds a way to do more, let me know. i have not found a way to query a specific oid via vbscript without using a com object specifically for this or an external command.

this method uses the wmi snmp provider. valid values for the class variable below, as far as i know,  are currently:
SNMP_RFC1213_MIB_snmp
SNMP_RFC1213_MIB_ip
SNMP_RFC1213_MIB_ipRouteTable
SNMP_RFC1213_MIB_ipAddrTable
SNMP_RFC1213_MIB_ipNetToMediaTable
SNMP_RFC1213_MIB_interfaces
SNMP_RFC1213_MIB_ifTable
SNMP_RFC1213_MIB_icmp
SNMP_RFC1213_MIB_tcp
SNMP_RFC1213_MIB_tcpConnTable
SNMP_RFC1213_MIB_egp
SNMP_RFC1213_MIB_egpNeighTable
SNMP_RFC1213_MIB_udp
SNMP_RFC1213_MIB_udpTable
SNMP_RFC1213_MIB_system
SNMP_RFC1213_MIB_atTable

using the wmi cim studio tools available from microsoft for free download, you can find these if you browse to root/snmp/smir and look in snmpmacro/snmpobjecttype

{% gist 38259a302d604fa4db53186feaaf8237 %}