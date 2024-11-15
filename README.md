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













