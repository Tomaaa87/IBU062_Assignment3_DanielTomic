pc pt pc0 168.90.0.11
pc pt pc1 168.90.0.12
laptop pt laptop0 168.90.0.13
server pt server0 168.90.0.14
pc pt pc2 210.3.14.11
server pt server1 210.3.14.12
srver pt server2 210.3.14.13
pc pt pc3 168.90.0.14
pc pt pc4 210.3.14.14


Configure the router interface


ip dhcp excluded-address 168.90.0.1 168.90.0.10 ip dhcp excluded-address 210.3.14.1 210.3.14.10


ip dhcp pool FIRST_POOL network 168.90.0.0 255.255.0.0 default-router 168.90.0.1 exit ip dhcp pool SECOND_POOL network 210.3.14.0 255.255.255.0 default-router 210.3.14.1 exit


