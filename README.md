# Laporan Praktikum Modul 4

## Kelompok 12

## VLSM Menggunakan CPT
### Topologi

### Konfigurasi
### Hololive
**Interfaces**
```
Fast Ethernet0/1 (A1)
- IPv4 Address : 192.239.19.73
- Subnet Mask : 255.255.255.252

Fast Ethernet1/1 (A2)
- IPv4 Address : 192.239.19.77
- Subnet Mask : 255.255.255.252

Fast Ethernet0/0 (A3)
- IPv4 Address : 192.239.19.81
- Subnet Mask : 255.255.255.252
```

**Static Routes**
```
192.239.19.84/30 via 192.239.19.82 (A4)

    Network: 192.239.19.84
    Mask: 255.255.255.252
    Next Hop: 192.239.19.82

192.239.19.88/30 via 192.239.19.82 (A5)

    Network: 192.239.19.88
    Mask: 255.255.255.252
    Next Hop: 192.239.19.82

192.239.19.92/30 via 192.239.19.82 (A6)

    Network: 192.239.19.92
    Mask: 255.255.255.252
    Next Hop: 192.239.19.82

192.239.16.0/23 via 192.239.19.82 (A7)

    Network: 192.239.16.0
    Mask: 255.255.254.0
    Next Hop: 192.239.19.82

192.239.18.192/26 via 192.239.19.82 (A8)

    Network: 192.239.18.192
    Mask: 255.255.255.192
    Next Hop: 192.239.19.82

192.239.8.0/22 via 192.239.19.82 (A9)

    Network: 192.239.8.0
    Mask: 255.255.252.0
    Next Hop: 192.239.19.82

192.239.19.48/29 via 192.239.19.78 (A10)

    Network: 192.239.19.48
    Mask: 255.255.255.248
    Next Hop: 192.239.19.78

192.239.19.96/30 via 192.239.19.74 (A11)

    Network: 192.239.19.48
    Mask: 255.255.255.252
    Next Hop: 192.239.19.74

192.239.19.100/30 via 192.239.19.74 (A12)

    Network: 192.239.19.100
    Mask: 255.255.255.252
    Next Hop: 192.239.19.74

192.239.12.0/23 via 192.239.19.74 (A13)

    Network: 192.239.12.0
    Mask: 255.255.254.0
    Next Hop: 192.239.19.74

192.239.19.32/28 via 192.239.19.78 (A14)

    Network: 192.239.19.32
    Mask: 255.255.255.240
    Next Hop: 192.239.19.78

192.239.0.0/21 via 192.239.19.78 (A15)

    Network: 192.239.0.0
    Mask: 255.255.248.0
    Next Hop: 192.239.19.78

192.239.19.56/29 via 192.239.19.74 (A16)

    Network: 192.239.19.56
    Mask: 255.255.255.248
    Next Hop: 192.239.19.74

192.239.19.64/29 via 192.239.19.74 (A17)

    Network: 192.239.19.64
    Mask: 255.255.255.248
    Next Hop: 192.239.19.74

192.239.18.128/26 via 192.239.19.74 (A18)

    Network: 192.239.18.128
    Mask: 255.255.255.192
    Next Hop: 192.239.19.74

192.239.19.0/28 via 192.239.19.74 (A19)

    Network: 192.239.19.0
    Mask: 255.255.255.240
    Next Hop: 192.239.19.74

192.239.18.0/25 via 192.239.19.78 (A20)

    Network: 192.239.18.0
    Mask: 255.255.255.128
    Next Hop: 192.239.19.78

192.239.19.72/30 via 192.239.19.78 (A21)

    Network: 192.239.19.72
    Mask: 255.255.255.252
    Next Hop: 192.239.19.78

192.239.14.0/23 via 192.239.19.78 (A22)

    Network: 192.239.14.0
    Mask: 255.255.254.0
    Next Hop: 192.239.19.78
```
### Holo-EN
**Interfaces**
```
Fast Ethernet0/0 (A1)
- IPv4 Address : 192.239.19.73
- Subnet Mask : 255.255.255.252

Fast Ethernet1/0 (A11)
- IPv4 Address : 192.239.19.97
- Subnet Mask : 255.255.255.252

Fast Ethernet0/1 (A12)
- IPv4 Address : 192.239.19.101
- Subnet Mask : 255.255.255.252
```

**Static Routes**
```
0.0.0.0/0 via 192.239.19.73 (Default to Hololive)

	Network: 0.0.0.0
	Mask: 0.0.0.0
	Next Hop: 192.239.19.73

192.239.12.0/23 via [next hope] (A13)

	Network: 192.239.12.0
	Mask: 255.255.254.0
	Next Hop: [next hope]

192.239.19.56/29 via [next hope] (A16)

	Network: 192.239.19.56
	Mask: 255.255.255.248
	Next Hop: [next hope]

192.239.19.64/29 via [next hope] (A17)

	Network: 192.239.19.64
	Mask: 255.255.255.248
	Next Hop: [next hope]

192.239.18.128/26 via [next hope] (A18)

	Network: 192.239.18.128
	Mask: 255.255.255.192
	Next Hop: [next hope]

192.239.19.0/28 via [next hope] (A19)

	Network: 192.239.19.0
	Mask: 255.255.255.240
	Next Hop: [next hope]
```




### CIDR ( GNS)

![WhatsApp Image 2024-11-16 at 00 35 03_bf0b6042](https://github.com/user-attachments/assets/a463e70f-4017-4752-9fc7-ec44e773d6c7)

#### Penggabungan Subnet

1. Pertama
   ![WhatsApp Image 2024-11-16 at 00 35 02_2f52a9c0](https://github.com/user-attachments/assets/a1f06998-9859-46cd-b564-52d20d7f70ec)
   ![image](https://github.com/user-attachments/assets/c6f73739-2608-4de3-a5c2-babafb8c106c)

3. Kedua
   ![WhatsApp Image 2024-11-16 at 00 35 02_80652a4d](https://github.com/user-attachments/assets/89caeb04-878c-4fa0-9d77-33eb73d08f01)
   ![image](https://github.com/user-attachments/assets/e4ca1372-577a-49a3-a20e-74fc4a9e454b)

5. Ketiga
   ![WhatsApp Image 2024-11-16 at 00 35 02_6d3f8120](https://github.com/user-attachments/assets/ee712bbd-3394-4dca-93c2-dfb5dd071d84)
   ![image](https://github.com/user-attachments/assets/0de80726-40c1-401c-80b2-6bd6471105bc)

7. Keempat
   ![WhatsApp Image 2024-11-16 at 00 35 01_3207b062](https://github.com/user-attachments/assets/43d817e1-999a-4f87-ad96-40d869d33b44)
   ![image](https://github.com/user-attachments/assets/c522619d-00f8-4f24-a727-c0844481ded4)

9. Kelima
   ![WhatsApp Image 2024-11-16 at 00 35 01_89598f75](https://github.com/user-attachments/assets/1b0dba5a-ba8c-4ce8-9e97-49673afeb4d3)
   ![image](https://github.com/user-attachments/assets/478cc92b-1258-4ca1-93b3-7f717be6b1b7)

11. Keenam
   ![WhatsApp Image 2024-11-16 at 00 35 00_a73fbe84](https://github.com/user-attachments/assets/79e503e8-1f22-42d7-973f-e6304bada4cd)
   ![image](https://github.com/user-attachments/assets/90a5e8cf-1344-418d-b4c3-b1c99bdd737c)

13. Ketujuh
   ![WhatsApp Image 2024-11-16 at 00 35 00_f81c26d1](https://github.com/user-attachments/assets/f4b30de5-7c69-4e0c-9605-bec6392a9ee9)
   ![image](https://github.com/user-attachments/assets/182228dc-7ffd-4739-af0e-84a5e12ad2ff)

15. Kedelapan
   ![WhatsApp Image 2024-11-16 at 00 35 00_975e5d85](https://github.com/user-attachments/assets/e37b5951-f90f-4013-a1b3-6c91cae96f30)
   ![image](https://github.com/user-attachments/assets/6b58fd1e-7c5a-4653-9c56-ca89043e1985)

17. Kesembilan
   ![WhatsApp Image 2024-11-16 at 00 34 59_0c0d83cb](https://github.com/user-attachments/assets/18daab6c-2ece-4f04-9c0d-06593df1cd0a)
   ![image](https://github.com/user-attachments/assets/fdf7d797-e6f4-4be4-b557-688347e7527f)


### TREE CIDR

![Tanpa judul (4)](https://github.com/user-attachments/assets/2388e260-5feb-4aae-9da4-3711eaab908f)

### PEMBAGIAN IP

![image](https://github.com/user-attachments/assets/4fb135ce-e1ca-489d-b379-18d97567e207)

### KONFIGURASI NETWORK

•	Hololive (Gateway)
```
auto lo
iface lo inet loopback

auto eth0
iface eth0  inet dhcp

#A1
auto eth1
iface eth1 inet static
    address 192.240.16.1
    netmask 255.255.255.252

#A3
auto eth2
iface eth2 inet static
    address 192.239.160.1
    netmask 255.255.255.252

#A2
auto eth3
iface eth3 inet static
    address 192.239.64.1
    netmask 255.255.255.252
```

•	Holo-EN (Gateway)
```
auto lo
iface lo inet loopback

#A1
auto eth0
iface eth0 inet static
    address 192.240.16.2
    netmask 255.255.255.252
    gateway 192.240.16.1

#A12
auto eth1
iface eth1 inet static
    address 192.240.4.1
    netmask 255.255.255.252

#A11
auto eth2
iface eth2 inet static
    address 192.240.8.33
    netmask 255.255.255.252
```

•	Holo-Myth (Gateway)
```
auto lo
iface lo inet loopback

#A12
auto eth0
iface eth0 inet static
    address 192.240.4.2
    netmask 255.255.255.252
    gateway 192.240.4.1

#A13
auto eth1
iface eth1 inet static
    address 192.240.0.1
    netmask 255.255.254.0

#A16
auto eth2
iface eth2 inet static
    address 192.240.2.1
    netmask 255.255.224.0
```

•	Gura_Ame_Ina (Client)
```
#A13
auto eth0
iface eth0 inet static
    address 192.240.1.254
    netmask 255.255.254.0
    gateway 192.240.0.1
```

•	Kiara_Calli (Client)
```
#A13
auto eth0
iface eth0 inet static
    address 192.240.1.255
    netmask 255.255.254.0
    gateway 192.240.0.1
```

•	Holo Advent (Gateway)
```
auto lo
iface lo inet loopback

#A11
auto eth0
iface eth0 inet static
    address 192.240.8.34
    netmask 255.255.255.252
    gateway 192.240.8.33

#A19
auto eth1
iface eth1 inet static
    address 192.240.8.1
    netmask 255.255.255.224
```

•	FuwaMoco (Client)
```
#A19
auto eth0
iface eth0 inet static
    address 192.240.8.30
    netmask 255.255.255.224
    gateway 192.240.8.1
```

•	Shiori_Nerissa (Client)
```
#A19
auto eth0
iface eth0 inet static
    address 192.240.8.31
    netmask 255.255.255.224
    gateway 192.240.8.1
```
•	Biboo (Client)
```
#A19
auto eth0
iface eth0 inet static
    address 192.240.8.32
    netmask 255.255.255.224
    gateway 192.240.8.1
```

•	Project-Hope (Gateway)
```
auto lo
iface lo inet loopback

#A16
auto eth0
iface eth0 inet static
    address 192.240.33.254
    netmask 255.255.224.0
    gateway 192.240.2.1

#A17
auto eth1
iface eth1 inet static
    address 192.240.34.65
    netmask 255.255.255.248
```

•	Irys (Client)
```
#A17
auto eth0
iface eth0 inet static
    address 192.240.34.70
    netmask 255.255.255.248
    gateway 192.240.34.65
```

•	Holo-Council (Gateway)
```
auto lo
iface lo inet loopback

#A16
auto eth0
iface eth0 inet static
    address 192.240.33.254
    netmask 255.255.224.0
    gateway 192.240.2.1

#A18
auto eth1
iface eth1 inet static
    address 192.240.34.1
    netmask 255.255.255.192
```


•	Kronii_Mumei (Client)
```
#A18
auto eth0
iface eth0 inet static
    address 192.240.34.62
    netmask 255.255.255.192
    gateway 192.240.34.1
```
•	Bae_Fauna (Client)
```
#A18
auto eth0
iface eth0 inet static
    address 192.240.34.63
    netmask 255.255.255.192
    gateway 192.240.34.1
```

•	Holo-ID (Gateway)
```
auto lo
iface lo inet loopback

#A3
auto eth0
iface eth0 inet static
    address 192.239.160.2
    netmask 255.255.255.252
    gateway 192.239.160.1

#A4
auto eth1
iface eth1 inet static
    address 192.239.132.1
    netmask 255.255.255.252

#A5
auto eth2
iface eth2 inet static
    address 192.239.144.65
    netmask 255.255.255.252

#A6
auto eth3
iface eth3 inet static
    address 192.239.138.1
    netmask 255.255.255.252
```

•	AREA15 (Gateway)
```
auto lo
iface lo inet loopback

#A4
auto eth0
iface eth0 inet static
    address 192.239.132.2
    netmask 255.255.255.252
    gateway 192.239.132.1

#A9
auto eth1
iface eth1 inet static
    address 192.239.128.1
    netmask 255.255.252.0
```

•	Risu (Client)
```
#A9
auto eth0
iface eth0 inet static
    address 192.239.131.254
    netmask 255.255.252.0
    gateway 192.239.128.1
```

•	Moona (Client)
```
#A9
auto eth0
iface eth0 inet static
    address 192.239.131.255
    netmask 255.255.252.0
    gateway 192.239.128.1
```

•	Iofi (Client)
```
#A9
auto eth0
iface eth0 inet static
    address 192.239.131.256
    netmask 255.255.252.0
    gateway 192.239.128.1
```

•	Holoro (Gateway)
```
auto lo
iface lo inet loopback

#A5
auto eth0
iface eth0 inet static
    address 192.239.144.66
    netmask 255.255.255.252
    gateway 192.239.144.65

#A8
auto eth1
iface eth1 inet static
    address 192.239.144.1
    netmask 255.255.252.192
```

•	Ollie (Client)
```
#A8
auto eth0
iface eth0 inet static
    address 192.239.144.62
    netmask 255.255.252.192
    gateway 192.239.144.1
```

•	Anya (Client)
```
#A8
auto eth0
iface eth0 inet static
    address 192.239.144.63
    netmask 255.255.252.192
    gateway 192.239.144.1
```

•	Reine (Client)
```
#A8
auto eth0
iface eth0 inet static
    address 192.239.144.64
    netmask 255.255.252.192
    gateway 192.239.144.1
```

•	Holoh3ro (Gateway)
```
auto lo
iface lo inet loopback

#A6
auto eth0
iface eth0 inet static
    address 192.239.138.2
    netmask 255.255.255.252
    gateway 192.239.138.1

#A7
auto eth1
iface eth1 inet static
    address 192.239.136.1
    netmask 255.255.254.0
```

•	Zeta (Client)
```
#A7
auto eth0
iface eth0 inet static
    address 192.239.137.254
    netmask 255.255.254.0
    gateway 192.239.136.1
```

•	Kaela (Client)
```
#A7
auto eth0
iface eth0 inet static
    address 192.239.137.255
    netmask 255.255.254.0
    gateway 192.239.136.1
```

•	Kobo(Client)
```
#A7
auto eth0
iface eth0 inet static
    address 192.239.137.256
    netmask 255.255.254.0
    gateway 192.239.136.1
```

•	Holo-JP (Gateway)
```
auto lo
iface lo inet loopback

#A2
auto eth0
iface eth0 inet static
    address 192.239.64.2
    netmask 255.255.255.252
   gateway 192.239.64.1

#A10
auto eth1
iface eth1 inet static
    address 192.239.32.1
    255.255.252.248
```

•	DEV_IS (Gateway)
```
auto lo
iface lo inet loopback

#A10
auto eth0
iface eth0 inet static
    address 192.239.32.6
    netmask 255.255.252.248
    gateway 192.239.32.1

#A14
auto eth1
iface eth1 inet static
    address 192.239.16.1
    netmask 255.255.255.240
```

•	Ririka_Raden (Client)
```
#A14
auto eth1
iface eth1 inet static
    address 192.239.16.14
    netmask 255.255.255.240
    gateway 192.239.16.1
```

•	Ao (Client)
```
#A14
auto eth1
iface eth1 inet static
    address 192.239.16.15
    netmask 255.255.255.240
    gateway 192.239.16.1
```

•	Hajime_Kanade (Client)
```
#A14
auto eth1
iface eth1 inet static
    address 192.239.16.16
    netmask 255.255.255.240
    gateway 192.239.16.1
```

•	GEN:0 (Gateway)
```
auto lo
iface lo inet loopback

#A10
auto eth0
iface eth0 inet static
    address 192.239.32.6
    netmask 255.255.252.248
    gateway 192.239.32.1

#A15
auto eth1
iface eth1 inet static
    address 192.239.0.1
    netmask 255.255.248.0
```

•	MiComet (Client)
```
#A15
auto eth0
iface eth0 inet static
    address 192.239.7.254
    netmask 255.255.248.0
    gateway 192.239.0.1
```

•	Sora_Robo_AZKi (Client)
```
#A15
auto eth0
iface eth0 inet static
    address 192.239.7.255
    netmask 255.255.248.0
    gateway 192.239.0.1
```

•	GEN:1 (Gateway)
```
auto lo
iface lo inet loopback

#A15
auto eth0
iface eth0 inet static
    address 192.239.7.254
    netmask 255.255.248.0
    gateway 192.239.0.1

#A22
auto eth1
iface eth1 inet static
    address 192.239.8.1
    netmask 255.255.254.0

#A21
auto eth2
iface eth2 inet static
    address 192.239.10.129
    netmask 255.255.255.252
```

•	FBK_Matsuri (Client)
```
#A22
auto eth0
iface eth0 inet static
    address 192.239.9.254
    netmask 255.255.254.0
    gateway 192.239.8.1
```

•	Aki_Hachama (Client)
```
#A22
auto eth0
iface eth0 inet static
    address 192.239.9.255
    netmask 255.255.254.0
    gateway 192.239.8.1
```

•	Gamers (Gateway)
```
auto lo
iface lo inet loopback

#A21
auto eth0
iface eth0 inet static
    address 192.239.10.130
    netmask 255.255.255.252
    gateway 192.239.10.129

#A20
auto eth1
iface eth1 inet static
    address 192.239.10.1
    netmask 255.255.255.128
```

•	Korone (Client)
```
#A20
auto eth0
iface eth0 inet static
    address 192.239.10.126
    netmask 255.255.255.128
    gateway 192.239.10.1
```

•	Okayu (Client)
```
#A20
auto eth0
iface eth0 inet static
    address 192.239.10.127
    netmask 255.255.255.128
    gateway 192.239.10.1
```

•	Mio (Client)
```
#A20
auto eth0
iface eth0 inet static
    address 192.239.10.128
    netmask 255.255.255.128
    gateway 192.239.10.1
```




















