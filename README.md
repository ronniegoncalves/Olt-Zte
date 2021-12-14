# Direcionando Vlan para porta de Uplink


#PORTALNETFSA-POP1-OLT1c300#conf t

#PORTALNETFSA-POP1-OLT1c300(config)#interface xgei_1/19/2
 
#PORTALNETFSA-POP1-OLT1c300(config-if)#show this  
#interface xgei_1/19/2
  #phy-attribute lan
  #no shutdown
  #hybrid-attribute fiber
  #no negotiation auto
  #speed 10000
  #duplex full
  #flowcontrol disable
  #linktrap enable
  #switchport mode trunk
  #switchport vlan 1,1038,1045-1046 tag
  #switchport vlan 2012 tag
  #port-protect disable
  #uplink-isolate disable
#!

#PORTALNETFSA-POP1-OLT1c300(config-if)#switchport vlan 1024 tag
#PORTALNETFSA-POP1-OLT1c300(config-if)#

#PORTALNETFSA-POP1-OLT1c300(config-if)#exit
#PORTALNETFSA-POP1-OLT1c300(config)#exit
#PORTALNETFSA-POP1-OLT1c300#wr
#Backuping old configuration into flash...
#Collecting configuration into memory....
#Writing configuration into flash....[OK]
