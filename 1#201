NO_1_3#sh run

Building configuration...
Current configuration : 13890 bytes

!
version RGOS 10.4(3b19)p3 Release(180891)(Mon Dec 15 12:13:56 CST 2014 -ngcf70)
hostname NO_1_3
!
!
!
!
!
!
!
sntp server 10.96.0.114
sntp enable
!
aaa new-model
!
!
!
aaa accounting update periodic 30
aaa accounting update
aaa accounting network ruijie start-stop group radius
aaa authorization ip-auth-mode supplicant
aaa authentication login ruijie local
aaa authentication dot1x ruijie group radius none
!
!
nfpp
!
!
vlan 1
!
vlan 2
 name guanli
!
vlan 11
!
vlan 12
!
vlan 13
!
vlan 14
!
vlan 15
!
vlan 21
!         
vlan 22
!
vlan 23
!
vlan 97
!
vlan 98
!
vlan 99
!
vlan 100
!
vlan 116
 name 1#407
!
vlan 119
 name 1#405
!
vlan 120
 name 1#406
!
vlan 121
 name 1#408
!         
vlan 122
 name 1#410
!
vlan 127
 name 1#409
!
vlan 179
 name 1#dianzibanpai
!
vlan 250
 name banbantong
!
!
username qhx password qhx
username wyf password heroonly1975
username wyf privilege 15
privilege exec all level 1 show 
no service password-encryption
service timestamps log datetime msec year
ip ssh version 2
!
ip dhcp snooping
!
!         
ip default-gateway 10.10.1.254
!
!
clock timezone east 8 0
radius-server host 10.96.0.12 test username ruijie idle-time 2 key ruijie
radius-server dead-criteria tries 6
radius-server key ruijie
!
logging server 10.96.14.222
http redirect direct-site 10.96.11.254 arp
http redirect direct-site 10.96.12.254 arp
http redirect direct-site 10.96.13.254 arp
http redirect homepage http://10.96.0.12/index.html
http redirect 10.96.14.243
enable secret 5 $1$7B8y$qyD6yvFCFA7EExzv 
enable service ssh-server
!
!
!
!
!
!
spanning-tree mode rstp
spanning-tree
dot1x accounting ruijie
dot1x authentication ruijie
dot1x probe-timer alive 60
dot1x client-probe enable
dot1x timeout quiet-period 5
dot1x private-supplicant-only
dot1x redirect
interface gi 1/0/1
 switchport access vlan 11
 anti-arp-spoofing ip 10.96.11.254
 rldp port loop-detect shutdown-port
 spanning-tree portfast
 shutdown
 description 1#1haomen_menwei  
!
interface gi 1/0/2
 switchport access vlan 250
 rldp port loop-detect shutdown-port
 spanning-tree portfast
 description 1#108_s108  
!
interface gi 1/0/3
 switchport access vlan 11
 anti-arp-spoofing ip 10.96.11.254
 rldp port loop-detect shutdown-port
 spanning-tree portfast
 dot1x port-control auto
!
interface gi 1/0/4
 switchport access vlan 11
 anti-arp-spoofing ip 10.96.11.254
 rldp port loop-detect shutdown-port
 spanning-tree portfast
 description 1#_xueshengchu_zhiwenji  
!
interface gi 1/0/5
 switchport access vlan 250
 rldp port loop-detect shutdown-port
 spanning-tree portfast
 description 1#110â€”â_s110
!
interface gi 1/0/6
 switchport access vlan 100
 rldp port loop-detect shutdown-port
 spanning-tree portfast
 description 1#204_jiankong  
!
interface gi 1/0/7
 switchport access vlan 250
 rldp port loop-detect shutdown-port
 spanning-tree portfast
 description 1#112_s113  
!
interface gi 1/0/8
 switchport access vlan 100
 rldp port loop-detect shutdown-port
 spanning-tree portfast
!
interface gi 1/0/9
 switchport access vlan 250
 rldp port loop-detect shutdown-port
 spanning-tree portfast
 description 1#111_s115
!
interface gi 1/0/10
 switchport access vlan 250
 rldp port loop-detect shutdown-port
 spanning-tree portfast
 description 1#109_s116  
!
interface gi 1/0/11
 switchport access vlan 11
 anti-arp-spoofing ip 10.96.11.254
 rldp port loop-detect shutdown-port
 spanning-tree portfast
 dot1x port-control auto
!
interface gi 1/0/12
 switchport access vlan 11
 anti-arp-spoofing ip 10.96.11.254
 rldp port loop-detect shutdown-port
 spanning-tree portfast
 dot1x port-control auto
!
interface gi 1/0/13
 switchport access vlan 250
 rldp port loop-detect shutdown-port
 spanning-tree portfast
 description 1#107b_s117
!
interface gi 1/0/14
 switchport access vlan 250
 anti-arp-spoofing ip 10.96.11.254
 rldp port loop-detect shutdown-port
 spanning-tree portfast
 description 1#107A_s120  
!
interface gi 1/0/15
 switchport access vlan 11
 anti-arp-spoofing ip 10.96.11.254
 rldp port loop-detect shutdown-port
 spanning-tree portfast
 dot1x port-control auto
!
interface gi 1/0/16
 switchport access vlan 250
 rldp port loop-detect shutdown-port
 spanning-tree portfast
 description 1#107a_s123
!
interface gi 1/0/17
 switchport access vlan 11
 anti-arp-spoofing ip 10.96.11.254
 rldp port loop-detect shutdown-port
 spanning-tree portfast
 dot1x port-control auto
!
interface gi 1/0/18
 switchport access vlan 11
 anti-arp-spoofing ip 10.96.11.254
 rldp port loop-detect shutdown-port
 spanning-tree portfast
 dot1x port-control auto
!
interface gi 1/0/19
 switchport access vlan 11
 rldp port loop-detect shutdown-port
 spanning-tree portfast
 dot1x port-control auto
 description 1#105
!
interface gi 1/0/20
 switchport access vlan 11
 anti-arp-spoofing ip 10.96.11.254
 rldp port loop-detect shutdown-port
 spanning-tree portfast
 dot1x port-control auto
!
interface gi 1/0/21
 switchport access vlan 12
 anti-arp-spoofing ip 10.96.12.254
 rldp port loop-detect shutdown-port
 spanning-tree portfast
 dot1x port-control auto
!
interface gi 1/0/22
 switchport access vlan 250
 rldp port loop-detect shutdown-port
 spanning-tree portfast
 description 1#205
!
interface gi 1/0/23
 switchport access vlan 250
 rldp port loop-detect shutdown-port
 spanning-tree portfast
 description 1#207_s209  
!
interface gi 1/0/24
 rldp port loop-detect shutdown-port
 spanning-tree portfast
 dot1x port-control auto
!
interface gi 2/0/1
 switchport access vlan 250
 rldp port loop-detect shutdown-port
 spanning-tree portfast
 description 1#209_s210
!         
interface gi 2/0/2
 switchport access vlan 250
 rldp port loop-detect shutdown-port
 spanning-tree portfast
 description 1#211_s212  
!
interface gi 2/0/3
 switchport access vlan 12
 anti-arp-spoofing ip 10.96.12.254
 rldp port loop-detect shutdown-port
 spanning-tree portfast
 dot1x port-control auto
!
interface gi 2/0/4
 switchport access vlan 250
 rldp port loop-detect shutdown-port
 spanning-tree portfast
 dot1x port-control auto
 description Link_to_A210  
!
interface gi 2/0/5
 switchport access vlan 250
 rldp port loop-detect shutdown-port
 spanning-tree portfast
 description 1#210_s215  
!
interface gi 2/0/6
 switchport access vlan 179
 rldp port loop-detect shutdown-port
 spanning-tree portfast
 description dianzibanpai
!
interface gi 2/0/7
 switchport access vlan 12
 anti-arp-spoofing ip 10.96.12.254
 rldp port loop-detect shutdown-port
 spanning-tree portfast
 dot1x port-control auto
 description 1#208
!
interface gi 2/0/8
 switchport access vlan 12
 anti-arp-spoofing ip 10.96.12.254
 rldp port loop-detect shutdown-port
 spanning-tree portfast
 dot1x port-control auto
 description 1#206_s218
!         
interface gi 2/0/9
 switchport access vlan 12
 anti-arp-spoofing ip 10.96.12.254
 rldp port loop-detect shutdown-port
 spanning-tree portfast
!
interface gi 2/0/10
 switchport access vlan 12
 anti-arp-spoofing ip 10.96.12.254
 rldp port loop-detect shutdown-port
 spanning-tree portfast
 dot1x port-control auto
!
interface gi 2/0/11
 switchport access vlan 12
 anti-arp-spoofing ip 10.96.12.254
 rldp port loop-detect shutdown-port
 spanning-tree portfast
 dot1x port-control auto
!
interface gi 2/0/12
 switchport access vlan 12
 anti-arp-spoofing ip 10.96.12.254
 rldp port loop-detect shutdown-port
 spanning-tree portfast
 description 1#204  
!
interface gi 2/0/13
 switchport access vlan 12
 anti-arp-spoofing ip 10.96.12.254
 rldp port loop-detect shutdown-port
 spanning-tree portfast
 dot1x port-control auto
!
interface gi 2/0/14
 switchport access vlan 12
 anti-arp-spoofing ip 10.96.12.254
 rldp port loop-detect shutdown-port
 spanning-tree portfast
 dot1x port-control auto
!
interface gi 2/0/15
 switchport access vlan 13
 anti-arp-spoofing ip 10.96.13.254
 rldp port loop-detect shutdown-port
 spanning-tree portfast
 dot1x port-control auto
!         
interface gi 2/0/16
 switchport access vlan 250
 rldp port loop-detect shutdown-port
 spanning-tree portfast
 description 1#306_s308  
!
interface gi 2/0/17
 switchport access vlan 250
 rldp port loop-detect shutdown-port
 spanning-tree portfast
 description 1#304
!
interface gi 2/0/18
 switchport access vlan 250
 rldp port loop-detect shutdown-port
 spanning-tree portfast
 description 1#308_s310  
!
interface gi 2/0/19
 switchport access vlan 13
 anti-arp-spoofing ip 10.96.13.254
 rldp port loop-detect shutdown-port
 spanning-tree portfast
 dot1x port-control auto
!
interface gi 2/0/20
 switchport access vlan 250
 rldp port loop-detect shutdown-port
 spanning-tree portfast
 description 1#310_s312  
!
interface gi 2/0/21
 switchport access vlan 99
 rldp port loop-detect shutdown-port
 spanning-tree portfast
!
interface gi 2/0/22
 switchport access vlan 13
 anti-arp-spoofing ip 10.96.13.254
 rldp port loop-detect shutdown-port
 spanning-tree portfast
 dot1x port-control auto
 description 1#309_s314
!
interface gi 2/0/23
 switchport access vlan 13
 anti-arp-spoofing ip 10.96.13.254
 rldp port loop-detect shutdown-port
 spanning-tree portfast
 dot1x port-control auto
 description 1#305_xin  
!
interface gi 2/0/24
 switchport access vlan 99
 rldp port loop-detect shutdown-port
 spanning-tree portfast
 dot1x port-control auto
!
interface gi 3/0/1
 spanning-tree portfast
!
interface gi 3/0/2
 switchport access vlan 250
 rldp port loop-detect shutdown-port
 spanning-tree portfast
 description 1#307_317  
!
interface gi 3/0/3
 rldp port loop-detect shutdown-port
 spanning-tree portfast
 dot1x port-control auto
!         
interface gi 3/0/4
 rldp port loop-detect shutdown-port
 spanning-tree portfast
 dot1x port-control auto
!
interface gi 3/0/5
 switchport access vlan 250
 rldp port loop-detect shutdown-port
 spanning-tree portfast
 description 1#106
!
interface gi 3/0/6
 rldp port loop-detect shutdown-port
 spanning-tree portfast
 dot1x port-control auto
!
interface gi 3/0/7
 switchport access vlan 13
 anti-arp-spoofing ip 10.96.13.254
 rldp port loop-detect shutdown-port
 spanning-tree portfast
 dot1x port-control auto
!
interface gi 3/0/8
 switchport access vlan 13
 anti-arp-spoofing ip 10.96.13.254
 rldp port loop-detect shutdown-port
 spanning-tree portfast
 dot1x port-control auto
!
interface gi 3/0/9
 rldp port loop-detect shutdown-port
 spanning-tree portfast
!
interface gi 3/0/10
 switchport access vlan 119
 rldp port loop-detect shutdown-port
 spanning-tree portfast
 description 1#405_s402  
!
interface gi 3/0/11
 switchport access vlan 119
 rldp port loop-detect shutdown-port
 spanning-tree portfast
 shutdown
 description 1#405_s403  
!
interface gi 3/0/12
 switchport access vlan 116
 rldp port loop-detect shutdown-port
 spanning-tree portfast
 description 1#407_s404  
!
interface gi 3/0/13
 switchport access vlan 116
 rldp port loop-detect shutdown-port
 spanning-tree portfast
 shutdown
 description 1#407_s405  
!
interface gi 3/0/14
 switchport access vlan 127
 rldp port loop-detect shutdown-port
 spanning-tree portfast
 description 1#409
!
interface gi 3/0/15
 switchport access vlan 122
 rldp port loop-detect shutdown-port
 spanning-tree portfast
 description 1#410jifang_s407  
!         
interface gi 3/0/16
 rldp port loop-detect shutdown-port
 spanning-tree portfast
 dot1x port-control auto
!
interface gi 3/0/17
 switchport access vlan 121
 rldp port loop-detect shutdown-port
 spanning-tree portfast
 description 1#408_s409  
!
interface gi 3/0/18
 rldp port loop-detect shutdown-port
 spanning-tree portfast
 dot1x port-control auto
 shutdown
!
interface gi 3/0/19
 switchport access vlan 120
 rldp port loop-detect shutdown-port
 spanning-tree portfast
 description 1#406_s411  
!
interface gi 3/0/20
 rldp port loop-detect shutdown-port
 spanning-tree portfast
 shutdown
 description 1#406_s412  
!
interface gi 3/0/21
 rldp port loop-detect shutdown-port
 spanning-tree portfast
!
interface gi 3/0/22
 rldp port loop-detect shutdown-port
 spanning-tree portfast
!
interface gi 3/0/23
 rldp port loop-detect shutdown-port
 spanning-tree portfast
!
interface gi 3/0/24
 rldp port loop-detect shutdown-port
 spanning-tree portfast
!
interface GigabitEthernet 1/0/25
 switchport mode trunk
 medium-type fiber
 ip dhcp snooping trust
 spanning-tree bpdufilter enable
 description ã€<Link_To_SW1_G0/24>
!
interface GigabitEthernet 1/0/26
!
interface GigabitEthernet 2/0/25
!
interface GigabitEthernet 2/0/26
!
interface GigabitEthernet 3/0/25
!
interface GigabitEthernet 3/0/26
!
interface VLAN 2
 ip address 10.10.1.3 255.255.255.0
 no shutdown
!
!
!
errdisable recovery interval 200
!
snmp-server host 10.96.14.222 traps version 2c ruijie
snmp-server enable traps
snmp-server community ruijie ro 
line con 0
line vty 0 4
!
!
end
NO_1_3#$                                                  sh vl              
VLAN Name                             Status    Ports     
---- -------------------------------- --------- -----------------------------------
   1 VLAN0001                         STATIC    Fa1/0/24, Gi1/0/25, Gi1/0/26, Gi2/0/25
                                                Gi2/0/26, Fa3/0/1, Fa3/0/3, Fa3/0/4   
                                                Fa3/0/6, Fa3/0/9, Fa3/0/16, Fa3/0/18  
                                                Fa3/0/20, Fa3/0/21, Fa3/0/22, Fa3/0/23
                                                Fa3/0/24, Gi3/0/25, Gi3/0/26          
   2 guanli                           STATIC    Gi1/0/25                              
  11 VLAN0011                         STATIC    Fa1/0/1, Fa1/0/3, Fa1/0/4, Fa1/0/11   
                                                Fa1/0/12, Fa1/0/15, Fa1/0/17, Fa1/0/18
                                                Fa1/0/19, Fa1/0/20, Gi1/0/25          
  12 VLAN0012                         STATIC    Fa1/0/21, Gi1/0/25, Fa2/0/3, Fa2/0/7  
                                                Fa2/0/8, Fa2/0/9, Fa2/0/10, Fa2/0/11  
                                                Fa2/0/12, Fa2/0/13, Fa2/0/14          
  13 VLAN0013                         STATIC    Gi1/0/25, Fa2/0/15, Fa2/0/19, Fa2/0/22
                                                Fa2/0/23, Fa3/0/7, Fa3/0/8            
  14 VLAN0014                         STATIC    Gi1/0/25                              
  15 VLAN0015                         STATIC    Gi1/0/25                              
  21 VLAN0021                         STATIC    Gi1/0/25                              
  22 VLAN0022                         STATIC    Gi1/0/25                              
  23 VLAN0023                         STATIC    Gi1/0/25                              
  97 VLAN0097                         STATIC    Gi1/0/25                              
  98 VLAN0098                         STATIC    Gi1/0/25                              
  99 VLAN0099                         STATIC    Gi1/0/25, Fa2/0/21, Fa2/0/24          
 100 VLAN0100                         STATIC    Fa1/0/6, Fa1/0/8, Gi1/0/25            
 116 1#407                            STATIC    Gi1/0/25, Fa3/0/12, Fa3/0/13          
 119 1#405                            STATIC    Gi1/0/25, Fa3/0/10, Fa3/0/11          
 120 1#406                            STATIC    Gi1/0/25, Fa3/0/19                    
 121 1#408                            STATIC    Gi1/0/25, Fa3/0/17                    
 122 1#410                            STATIC    Gi1/0/25, Fa3/0/15                    
 127 1#409                            STATIC    Gi1/0/25, Fa3/0/14                    
 179 1#dianzibanpai                   STATIC    Gi1/0/25, Fa2/0/6                     
 250 banbantong                       STATIC    Fa1/0/2, Fa1/0/5, Fa1/0/7, Fa1/0/9    
                                                Fa1/0/10, Fa1/0/13, Fa1/0/14, Fa1/0/16
                                                Fa1/0/22, Fa1/0/23, Gi1/0/25, Fa2/0/1 
                                                Fa2/0/2, Fa2/0/4, Fa2/0/5, Fa2/0/16   
                                                Fa2/0/17, Fa2/0/18, Fa2/0/20, Fa3/0/2 
                                                Fa3/0/5                               
NO_1_3#                    sh ver
System description      : Ruijie Gigabit Security & Intelligence Access Switch (S2628G-E) By Ruijie Networks
System start time       : 2023-02-13 22:30:54
System uptime           : 0:0:3:8
System hardware version : 1.01
System software version : RGOS 10.4(3b19)p3 Release(180891)
System BOOT version     : 10.4(2b2) Release(85787)
System CTRL version     : 10.4(2b2) Release(85787)
System serial number    : 2683DH7350460
Device information:
  Device-1
    Hardware version : 1.01
    Software version : RGOS 10.4(3b19)p3 Release(180891)
    BOOT version     : 10.4(2b2) Release(85787)
    CTRL version     : 10.4(2b2) Release(85787)
    Serial Number    : 2683DH7350460
  Device-2
    Hardware version : 1.01
    Software version : RGOS 10.4(3b19)p3 Release(180891)
    BOOT version     : 10.4(2b2) Release(85787)
    CTRL version     : 10.4(2b2) Release(85787)
    Serial Number    : 2683DH7350434
  Device-3
    Hardware version : 1.01
    Software version : RGOS 10.4(3b19)p3 Release(180891)
    BOOT version     : 10.4(2b2) Release(85787)
    CTRL version     : 10.4(2b2) Release(85787)
    Serial Number    : 2683DH7350531
