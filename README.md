# Домашняя работа Keepalived/vrrp 10-02. Неклюдов Михаил

Задание 1.

vrrp_instance test {

state MASTER

interface enp0s8

virtual_router_id 10

priority 110

advert_int 4

authentication {

auth_type AH

auth_pass 123

}

unicast_peer {

192.168.123.20

}

virtual_ipaddress {

192.168.0.50 dev enp0s8 label enp0s8:vip

}

}

![image](https://github.com/MikhailNeklyudov/09-02-hw/assets/130427747/5503ed86-3766-4e0d-b5f4-af5cab7b695d)


vrrp_instance test {

state BACKUP

interface enp0s8

virtual_router_id 10

priority 100

advert_int 4

authentication {

auth_type AH

auth_pass 123

}

unicast_peer {

192.168.123.18

}

virtual_ipaddress {

192.168.0.50 dev enp0s8 label enp0s8:vip

}

}

![image](https://github.com/MikhailNeklyudov/09-02-hw/assets/130427747/433b479a-5c00-4cd8-80fd-9fdc57cee337)




Задание 2.



 ![VirtualBox_Debian11-master_23_07_2023_14_45_01](https://github.com/MikhailNeklyudov/09-02-hw/assets/130427747/a85a33dd-09b2-485a-a316-a0b0b7ce0c39)

