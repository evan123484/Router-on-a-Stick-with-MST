# Router-on-a-Stick-with-MST
Laboratoire CML pour pratiquer routage inter-VLAN (ROAS), trois VLAN, trunking 802.1Q, le protocole MST avec 3 instances  et un pont racine pour chaque instance. 


Topologie: 3 commutateurs, 1 routeur, 3 VLAN (10,20,30)


routage inter-VLAN: VLAN 10: 192.168.10.0/24, VLAN 20: 192.168.20.0/24, VLAN 30: 192.168.30.0/24 via 802.1Q.


MST: MST1: VLAN 10 commutateur racine S1, MST2: VLAN 20 commutateur racine S2, MST3: VLAN 30 commutateur S3


Vérification: show spanning-tree mst, show interfaces trunk, show ip int br sur R1 (montre les subinterface sur R1). 


Explication: le routeur utilise des sous-interfaces pour effectuer le routage entre trois VLAN. le protocole MST permet de créer plusieurs instances. Dans ce cas, chaque instance possède un pont racine different et chaque instance possède un VLAN. Cela permet l'utilisation de différents chemins pour chaque VLAN et pour chaque instance.  


