# Laporan Praktikum Modul 4

## Kelompok IT12

## VLSM Menggunakan CPT
### Topologi

![image](https://github.com/user-attachments/assets/8c75c8e2-f6bd-48eb-8bcd-40c05d4dd4f8)

### Pembagian IP - VLSM

![image](https://github.com/user-attachments/assets/f1d8bdac-8444-43c9-8d7b-e12ffa83077d)

### Tree IP - VLSM

[IMAGE TREE]

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

    Network: 192.239.19.96
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
- IPv4 Address : 192.239.19.74
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

192.239.12.0/23 via 192.239.19.102 (A13)

	Network: 192.239.12.0
	Mask: 255.255.254.0
	Next Hop: 192.239.19.102

192.239.19.56/29 via 192.239.19.102 (A16)

	Network: 192.239.19.56
	Mask: 255.255.255.248
	Next Hop: 192.239.19.102

192.239.19.64/29 via 192.239.19.102 (A17)

	Network: 192.239.19.64
	Mask: 255.255.255.248
	Next Hop: 192.239.19.102

192.239.18.128/26 via 192.239.19.102 (A18)

	Network: 192.239.18.128
	Mask: 255.255.255.192
	Next Hop: 192.239.19.102

192.239.19.0/27 via 192.239.19.98 (A19)

	Network: 192.239.19.0
	Mask: 255.255.255.224
	Next Hop: 192.239.19.98
```
### Holo-Myth
**Interfaces**
```
Fast Ethernet0/0 (A12)
- IPv4 Address : 192.239.19.102
- Subnet Mask : 255.255.255.252

Fast Ethernet1/0 (A16)
- IPv4 Address : 192.239.19.57
- Subnet Mask : 255.255.255.248

Fast Ethernet0/1 (A13)
- IPv4 Address : 192.239.12.1
- Subnet Mask : 255.255.254.0
```

**Static Routes**
```
0.0.0.0/0 via 192.239.19.101 (Default to Holo-EN)

	Network: 0.0.0.0
	Mask: 0.0.0.0
	Next Hop: 192.239.19.101

192.239.19.64/29 via 192.239.19.58 (A17)

	Network: 192.239.19.64
	Mask: 255.255.255.248
	Next Hop: 192.239.19.58

192.239.18.128/26 via 192.239.19.58 (A18)

	Network: 192.239.18.128
	Mask: 255.255.255.192
	Next Hop: 192.239.19.58

```

#### Gura-Ame-Ina (PC)
```
Fast Ethernet0/0 (A13)
- IPv4 Address : 192.239.12.3
- Subnet Mask : 255.255.254.0
- Default Gateway : 192.239.12.1
```

#### Kiara-Calli (PC)
```
Fast Ethernet0/0 (A13)
- IPv4 Address : 192.239.12.4
- Subnet Mask : 255.255.254.0
- Default Gateway : 192.239.12.1
```

### Holo-Council
**Interfaces**
```
Fast Ethernet0/1 (A18)
- IPv4 Address : 192.239.18.129
- Subnet Mask : 255.255.255.192

Fast Ethernet0/0 (A16)
- IPv4 Address : 192.239.19.59
- Subnet Mask : 255.255.255.248

```

**Static Routes**
```
0.0.0.0/0 via 192.239.19.57 (Default to Holo-Myth)

	Network: 0.0.0.0
	Mask: 0.0.0.0
	Next Hop: 192.239.19.57

192.239.19.64/29 via 192.239.19.60 (A17)

	Network: 192.239.19.64
	Mask: 255.255.255.248
	Next Hop: 192.239.19.58

```
#### Kronii_Mumei (PC)
```
Fast Ethernet0/0 (A18)
- IPv4 Address : 192.239.18.130
- Subnet Mask : 255.255.255.192
- Default Gateway : 192.239.18.129
```

#### Bae_Fauna (PC)
```
Fast Ethernet0/0 (A18)
- IPv4 Address : 192.239.18.131
- Subnet Mask : 255.255.255.192
- Default Gateway : 192.239.18.129
```

### Project-Hope
**Interfaces**
```
Fast Ethernet0/1 (A17)
- IPv4 Address : 192.239.19.65
- Subnet Mask : 255.255.255.248

Fast Ethernet0/0 (A16)
- IPv4 Address : 192.239.19.58
- Subnet Mask : 255.255.255.248

```
**Static Routes**
```
0.0.0.0/0 via 192.239.19.57 (Default to Holo-Myth)

	Network: 0.0.0.0
	Mask: 0.0.0.0
	Next Hop: 192.239.19.57

192.239.18.128/26 via 192.239.19.58 (A18)

	Network: 192.239.18.128
	Mask: 255.255.255.192
	Next Hop: 192.239.19.59

```
#### Irys (PC)
```
Fast Ethernet0/0 (A17)
- IPv4 Address : 192.239.19.66
- Subnet Mask : 255.255.255.248
- Default Gateway : 192.239.19.65
```

### Holo-Advent
**Interfaces**
```
Fast Ethernet0/0 (A11)
- IPv4 Address : 192.239.19.98
- Subnet Mask : 255.255.255.252

Fast Ethernet0/1 (A19)
- IPv4 Address : 192.239.19.1
- Subnet Mask : 255.255.255.224

```

**Static Routes**
```
0.0.0.0/0 via 192.239.19.97 (Default to Holo-EN)

	Network: 0.0.0.0
	Mask: 0.0.0.0
	Next Hop: 192.239.19.97

```
#### FuwaMoco (PC)
```
Fast Ethernet0/0 (A19)
- IPv4 Address : 192.239.19.2
- Subnet Mask : 255.255.255.224
- Default Gateway : 192.239.19.1
```
#### Shiori_Nerissa (PC)
```
Fast Ethernet0/0 (A19)
- IPv4 Address : 192.239.19.3
- Subnet Mask : 255.255.255.224
- Default Gateway : 192.239.19.1
```
#### Biboo (PC)
```
Fast Ethernet0/0 (A19)
- IPv4 Address : 192.239.19.4
- Subnet Mask : 255.255.255.224
- Default Gateway : 192.239.19.1
```

### Holo-ID
**Interfaces**
```
Fast Ethernet0/0 (A3)
- IPv4 Address : 192.239.19.82
- Subnet Mask : 255.255.255.252

Fast Ethernet0/1 (A4)
- IPv4 Address : 192.239.19.85
- Subnet Mask : 255.255.255.252

Fast Ethernet1/0 (A5)
- IPv4 Address : 192.239.19.89
- Subnet Mask : 255.255.255.252

Fast Ethernet1/1 (A6)
- IPv4 Address : 192.239.19.93
- Subnet Mask : 255.255.255.252

```

**Static Routes**
```
0.0.0.0/0 via 192.239.19.81 (Default to Hololive)

	Network: 0.0.0.0
	Mask: 0.0.0.0
	Next Hop: 192.239.19.81

192.239.8.0/22 via 192.239.19.86 (A9)

	Network: 192.239.8.0
	Mask: 255.255.252.0
	Next Hop: 192.239.19.86

192.239.18.192/26 via 192.239.19.90 (A8)

	Network: 192.239.18.192
	Mask: 255.255.255.192
	Next Hop: 192.239.19.90

192.239.16.0/23 via 192.239.19.94 (A7)

	Network: 192.239.16.0
	Mask: 255.255.254.0
	Next Hop: 192.239.19.94

```
### AREA-15
**Interfaces**
```
Fast Ethernet0/1 (A9)
- IPv4 Address : 192.239.8.1
- Subnet Mask : 255.255.252.0

Fast Ethernet0/0 (A4)
- IPv4 Address : 192.239.19.86
- Subnet Mask : 255.255.255.252
```
**Static Routes**
```
0.0.0.0/0 via 192.239.19.85 (Default to Holo-ID)

	Network: 0.0.0.0
	Mask: 0.0.0.0
	Next Hop: 192.239.19.85

```
#### Risu (PC)
```
Fast Ethernet0/0 (A9)
- IPv4 Address : 192.239.8.2
- Subnet Mask : 255.255.252.0
- Default Gateway : 192.239.8.1
```
#### Moona (PC)
```
Fast Ethernet0/0 (A9)
- IPv4 Address : 192.239.8.3
- Subnet Mask : 255.255.252.0
- Default Gateway : 192.239.8.1
```
#### Lofi (PC)
```
Fast Ethernet0/0 (A9)
- IPv4 Address : 192.239.8.4
- Subnet Mask : 255.255.252.0
- Default Gateway : 192.239.8.1
```

### holoro
**Interfaces**
```
Fast Ethernet0/1 (A8)
- IPv4 Address : 192.239.18.193
- Subnet Mask : 255.255.255.192

Fast Ethernet0/0 (A5)
- IPv4 Address : 192.239.19.90
- Subnet Mask : 255.255.255.252
```
**Static Routes**
```
0.0.0.0/0 via 192.239.19.89 (Default to Holo-ID)

	Network: 0.0.0.0
	Mask: 0.0.0.0
	Next Hop: 192.239.19.89

```
#### Ollie (PC)
```
Fast Ethernet0/0 (A8)
- IPv4 Address : 192.239.18.194
- Subnet Mask : 255.255.255.192
- Default Gateway : 192.239.18.193
```
#### Anya (PC)
```
Fast Ethernet0/0 (A8)
- IPv4 Address : 192.239.18.195
- Subnet Mask : 255.255.255.192
- Default Gateway : 192.239.18.193
```
#### Reine (PC)
```
Fast Ethernet0/0 (A8)
- IPv4 Address : 192.239.18.196
- Subnet Mask : 255.255.255.192
- Default Gateway : 192.239.18.193
```

### holoh3ro
**Interfaces**
```
Fast Ethernet0/1 (A7)
- IPv4 Address : 192.239.16.1
- Subnet Mask : 255.255.254.0

Fast Ethernet0/0 (A6)
- IPv4 Address : 192.239.19.94
- Subnet Mask : 255.255.255.252
```
**Static Routes**
```
0.0.0.0/0 via 192.239.19.93 (Default to Holo-ID)

	Network: 0.0.0.0
	Mask: 0.0.0.0
	Next Hop: 192.239.19.93

```
#### Zeta (PC)
```
Fast Ethernet0/0 (A7)
- IPv4 Address : 192.239.16.2
- Subnet Mask : 255.255.254.0
- Default Gateway : 192.239.16.1
```
#### Kaela (PC)
```
Fast Ethernet0/0 (A7)
- IPv4 Address : 192.239.16.3
- Subnet Mask : 255.255.254.0
- Default Gateway : 192.239.16.1
```
#### Kobo (PC)
```
Fast Ethernet0/0 (A7)
- IPv4 Address : 192.239.16.4
- Subnet Mask : 255.255.254.0
- Default Gateway : 192.239.16.1
```

### Holo-JP
**Interfaces**
```
Fast Ethernet0/0 (A2)
- IPv4 Address : 192.239.19.78
- Subnet Mask : 255.255.255.252

Fast Ethernet0/1 (A10)
- IPv4 Address : 192.239.19.49 -> (1) sisa 50 (fa0 dev_is)dan 51 (fa0 gen:0)
- Subnet Mask : 255.255.255.248
```
**Static Routes**
```
0.0.0.0/0 via 192.239.19.77 (Default to Hololive)

	Network: 0.0.0.0
	Mask: 0.0.0.0
	Next Hop: 192.239.19.77

192.239.19.32/28 via 192.239.19.50 (A14)

	Network: 192.239.19.32
	Mask: 255.255.255.240
	Next Hop: 192.239.19.50

192.239.0.0/21 via 192.239.19.51 (A15)

	Network: 192.239.0.0
	Mask: 255.255.248.0
	Next Hop: 192.239.19.51

192.239.18.0/25 via 192.239.19.51 (A20)

	Network: 192.239.18.0
	Mask: 255.255.255.128
	Next Hop: 192.239.19.51

192.239.19.104/30 via 192.239.19.51 (A21)

	Network: 192.239.19.104
	Mask: 255.255.255.252
	Next Hop: 192.239.19.51

192.239.14.0/23 via 192.239.19.51 (A22)

	Network: 192.239.14.0
	Mask: 255.255.254.0
	Next Hop: 192.239.19.51
```

### DEV_IS
**Interfaces**
```
Fast Ethernet0/0 (A10)
- IPv4 Address : 192.239.19.50 -> (2) sisa 51 (fa0 gen:0)
- Subnet Mask : 255.255.255.248

Fast Ethernet0/1 (A14)
- IPv4 Address : 192.239.19.33
- Subnet Mask : 255.255.255.240
```
**Static Routes**
```
0.0.0.0/0 via 192.239.19.49 (Default to Holo-JP)

	Network: 0.0.0.0
	Mask: 0.0.0.0
	Next Hop: 192.239.19.49

192.239.0.0/21 via 192.239.19.51 (A15)

	Network: 192.239.0.0
	Mask: 255.255.248.0
	Next Hop: 192.239.19.51

192.239.18.0/25 via 192.239.19.51 (A20)

	Network: 192.239.18.0
	Mask: 255.255.255.128
	Next Hop: 192.239.19.51

192.239.19.104/30 via 192.239.19.51 (A21)

	Network: 192.239.19.104
	Mask: 255.255.255.252
	Next Hop: 192.239.19.51

192.239.14.0/23 via 192.239.19.51 (A22)

	Network: 192.239.14.0
	Mask: 255.255.254.0
	Next Hop: 192.239.19.51
```
#### Ririka_Raden (PC)
```
Fast Ethernet0/0 (A14)
- IPv4 Address : 192.239.19.34
- Subnet Mask : 255.255.255.240
- Default Gateway : 192.239.19.33
```
#### Ao (PC)
```
Fast Ethernet0/0 (A14)
- IPv4 Address : 192.239.19.35
- Subnet Mask : 255.255.255.240
- Default Gateway : 192.239.19.33
```
#### Hajime_Kanade (PC)
```
Fast Ethernet0/0 (A14)
- IPv4 Address : 192.239.19.36
- Subnet Mask : 255.255.255.240
- Default Gateway : 192.239.19.33
```

### GEN:0
**Interfaces**
```
Fast Ethernet0/0 (A10)
- IPv4 Address : 192.239.19.51
- Subnet Mask : 255.255.255.248

Fast Ethernet0/1 (A15)
- IPv4 Address : 192.239.0.1
- Subnet Mask : 255.255.248.0
```
**Static Routes**
```
0.0.0.0/0 via 192.239.19.49 (Default to Holo-JP)

	Network: 0.0.0.0
	Mask: 0.0.0.0
	Next Hop: 192.239.19.49

192.239.19.32/28 via 192.239.19.50 (A14)

	Network: 192.239.19.32
	Mask: 255.255.255.240
	Next Hop: 192.239.19.50

192.239.18.0/25 via 192.239.19.52 (A20)

	Network: 192.239.18.0
	Mask: 255.255.255.128
	Next Hop: 192.239.0.2

192.239.19.104/30 via 192.239.19.52 (A21)

	Network: 192.239.19.104
	Mask: 255.255.255.252
	Next Hop: 192.239.0.2

192.239.14.0/23 via 192.239.19.52 (A22)

	Network: 192.239.14.0
	Mask: 255.255.254.0
	Next Hop: 192.239.0.2

```
#### MiComet (PC)
```
Fast Ethernet0/0 (A15)
- IPv4 Address : 192.239.0.3
- Subnet Mask : 255.255.248.0
- Default Gateway : 192.239.0.1
```
#### Sora_Robo_AZKI (PC)
```
Fast Ethernet0/0 (A15)
- IPv4 Address : 192.239.0.4
- Subnet Mask : 255.255.248.0
- Default Gateway : 192.239.0.1
```

### GEN:1
**Interfaces**
```
Fast Ethernet0/0 (A15)
- IPv4 Address : 192.239.0.2
- Subnet Mask : 255.255.248.0

Fast Ethernet0/1 (A22)
- IPv4 Address : 192.239.14.1
- Subnet Mask : 255.255.254.0

Fast Ethernet1/0 (A21)
- IPv4 Address : 192.239.19.105
- Subnet Mask : 255.255.255.252
```
**Static Routes**
```
0.0.0.0/0 via 192.239.0.1 (Default to GEN:0)

	Network: 0.0.0.0
	Mask: 0.0.0.0
	Next Hop: 192.239.0.1

192.239.18.0/25 via 192.239.19.50 (A20)

	Network: 192.239.18.0
	Mask: 255.255.255.128
	Next Hop: 192.239.19.106

```
#### FBK_Matsuri (PC)
```
Fast Ethernet0/0 (A22)
- IPv4 Address : 192.239.14.2
- Subnet Mask : 255.255.254.0
- Default Gateway : 192.239.14.1
```
#### Aki_Hachama (PC)
```
Fast Ethernet0/0 (A22)
- IPv4 Address : 192.239.14.3
- Subnet Mask : 255.255.254.0
- Default Gateway : 192.239.14.1
```

### GAMERS
**Interfaces**
```
Fast Ethernet0/0 (A21)
- IPv4 Address : 192.239.19.106
- Subnet Mask : 255.255.255.252

Fast Ethernet0/1 (A20)
- IPv4 Address : 192.239.18.1
- Subnet Mask : 255.255.255.128

```
**Static Routes**
```
0.0.0.0/0 via 192.239.19.105 (Default to GEN:1)

	Network: 0.0.0.0
	Mask: 0.0.0.0
	Next Hop: 192.239.19.105
```
#### Korone (PC)
```
Fast Ethernet0/0 (A20)
- IPv4 Address : 192.239.18.2
- Subnet Mask : 255.255.255.128
- Default Gateway : 192.239.18.1
```
#### Okayu (PC)
```
Fast Ethernet0/0 (A20)
- IPv4 Address : 192.239.18.3
- Subnet Mask : 255.255.255.128
- Default Gateway : 192.239.18.1
```
#### Mio (PC)
```
Fast Ethernet0/0 (A20)
- IPv4 Address : 192.239.18.4
- Subnet Mask : 255.255.255.128
- Default Gateway : 192.239.18.1
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

![Tanpa judul (7)](https://github.com/user-attachments/assets/5b53495f-44ae-4cd9-8c08-2b7d9f36608a)

### PEMBAGIAN IP

![Screenshot 2024-11-19 232439](https://github.com/user-attachments/assets/a4ef0d91-34a3-4965-982c-4182dc4b6e2e)

### KONFIGURASI NETWORK

•	Hololive (Gateway)

```
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
    gateway 192.240.16.1

#A11
auto eth2
iface eth2 inet static
    address 192.240.40.1
    netmask 255.255.255.252
```

•	Holo-Myth (Gateway)

```
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
    address 192.240.2.129
    netmask 255.255.255.248
```

•	Gura_Ame_Ina (Client)

```
#A13
auto eth0
iface eth0 inet static
    address 192.240.0.2
    netmask 255.255.254.0
    gateway 192.240.0.1
```

•	Kiara_Calli (Client)

```
#A13
auto eth0
iface eth0 inet static
    address 192.240.0.3
    netmask 255.255.254.0
    gateway 192.240.0.1
```

•	Holo Advent (Gateway)

```
#A11
auto eth0
iface eth0 inet static
    address 192.240.40.2
    netmask 255.255.255.252
    gateway 192.240.40.1

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
    address 192.240.8.2
    netmask 255.255.255.224
    gateway 192.240.8.1
```

•	Shiori_Nerissa (Client)

```
#A19
auto eth0
iface eth0 inet static
    address 192.240.8.3
    netmask 255.255.255.224
    gateway 192.240.8.1
```

•	Biboo (Client)

```
#A19
auto eth0
iface eth0 inet static
    address 192.240.8.4
    netmask 255.255.255.224
    gateway 192.240.8.1
```

•	Project-Hope (Gateway)

```
#A16
auto eth0
iface eth0 inet static
    address 192.240.2.130   
    netmask 255.255.255.248
    gateway 192.240.2.129

#A17
auto eth1
iface eth1 inet static
    address 192.240.2.65
    netmask 255.255.255.248
```

•	Irys (Client)

```
#A17
auto eth0
iface eth0 inet static
    address 192.240.2.66
    netmask 255.255.255.248
    gateway 192.240.2.65
```

•	Holo-Council (Gateway)

```
#A16
auto eth0
iface eth0 inet static
    address 192.240.2.131
    netmask 255.255.255.248
    gateway 192.240.2.129

#A18
auto eth1
iface eth1 inet static
    address 192.240.2.1
    netmask 255.255.255.192
```

•	Kronii_Mumei (Client)

```
#A18
auto eth0
iface eth0 inet static
    address 192.240.2.2
    netmask 255.255.255.192
    gateway 192.240.2.1
```

•	Bae_Fauna (Client)

```
#A18
auto eth0
iface eth0 inet static
    address 192.240.2.3
    netmask 255.255.255.192
    gateway 192.240.2.1
```

•	Holo-ID (Gateway)

```
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
    address 192.239.208.1
    netmask 255.255.255.252

#A6
auto eth3
iface eth3 inet static
    address 192.239.138.1
    netmask 255.255.255.252
```

•	AREA15 (Gateway)

```
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
    address 192.239.128.2
    netmask 255.255.252.0
    gateway 192.239.128.1
```

•	Moona (Client)

```
#A9
auto eth0
iface eth0 inet static
    address 192.239.128.3
    netmask 255.255.252.0
    gateway 192.239.128.1
```

•	Iofi (Client)

```
#A9
auto eth0
iface eth0 inet static
    address 192.239.128.4
    netmask 255.255.252.0
    gateway 192.239.128.1
```

•	Holoro (Gateway)

```
#A5
auto eth0
iface eth0 inet static
    address 192.239.208.2
    netmask 255.255.255.252
    gateway 192.239.208.1

#A8
auto eth1
iface eth1 inet static
    address 192.239.144.1
    netmask 255.255.255.192
```

•	Ollie (Client)

```
#A8
auto eth0
iface eth0 inet static
    address 192.239.144.2
    netmask 255.255.252.192
    gateway 192.239.144.1
```

•	Anya (Client)

```
#A8
auto eth0
iface eth0 inet static
    address 192.239.144.3
    netmask 255.255.252.192
    gateway 192.239.144.1
```

•	Reine (Client)

```
#A8
auto eth0
iface eth0 inet static
    address 192.239.144.4
    netmask 255.255.252.192
    gateway 192.239.144.1
```

•	Holoh3ro (Gateway)

```
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
    address 192.239.136.2
    netmask 255.255.254.0
    gateway 192.239.136.1
```

•	Kaela (Client)

```
#A7
auto eth0
iface eth0 inet static
    address 192.239.136.3
    netmask 255.255.254.0
    gateway 192.239.136.1
```

•	Kobo(Client)

```
#A7
auto eth0
iface eth0 inet static
    address 192.239.136.4
    netmask 255.255.254.0
    gateway 192.239.136.1
```

•	Holo-JP (Gateway)

```
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
    netmask 255.255.255.248
```

•	DEV_IS (Gateway)

```
auto lo
iface lo inet loopback

#A10
auto eth0
iface eth0 inet static
    address 192.239.32.2
    netmask 255.255.255.248
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
    address 192.239.16.2
    netmask 255.255.255.240
    gateway 192.239.16.1
```

•	Ao (Client)

```
#A14
auto eth1
iface eth1 inet static
    address 192.239.16.3
    netmask 255.255.255.240
    gateway 192.239.16.1
```

•	Hajime_Kanade (Client)

```
#A14
auto eth1
iface eth1 inet static
    address 192.239.16.4
    netmask 255.255.255.240
    gateway 192.239.16.1
```

•	GEN:0 (Gateway)

```
#A10
auto eth0
iface eth0 inet static
    address 192.239.32.3
    netmask 255.255.255.248
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
    address 192.239.0.2
    netmask 255.255.248.0
    gateway 192.239.0.1
```

•	Sora_Robo_AZKi (Client)

```
#A15
auto eth0
iface eth0 inet static
    address 192.239.0.3
    netmask 255.255.248.0
    gateway 192.239.0.1
```

•	GEN:1 (Gateway)

```
#A15
auto eth0
iface eth0 inet static
    address 192.239.0.4
    netmask 255.255.248.0
    gateway 192.239.0.1

#A21
auto eth1
iface eth1 inet static
    address 192.239.10.129
    netmask 255.255.255.252

#A22
auto eth2
iface eth2 inet static
    address 192.239.8.1
    netmask 255.255.254.0
```

•	FBK_Matsuri (Client)

```
#A22
auto eth0
iface eth0 inet static
    address 192.239.8.2
    netmask 255.255.254.0
    gateway 192.239.8.1
```

•	Aki_Hachama (Client)

```
#A22
auto eth0
iface eth0 inet static
    address 192.239.8.3
    netmask 255.255.254.0
    gateway 192.239.8.1
```


•	Gamers (Gateway)

```
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
    address 192.239.10.2
    netmask 255.255.255.128
    gateway 192.239.10.1
```

•	Okayu (Client)

```
#A20
auto eth0
iface eth0 inet static
    address 192.239.10.3
    netmask 255.255.255.128
    gateway 192.239.10.1
```


•	Mio (Client)

```
#A20
auto eth0
iface eth0 inet static
    address 192.239.10.4
    netmask 255.255.255.128
    gateway 192.239.10.1
```

### ROUTING

•	Hololive

```
#hololiveA1holomythA12
post-up route add -net 192.240.4.0 netmask 255.255.255.252 gw 192.240.16.2

#A13Gurame
post-up route add -net 192.240.0.0 netmask 255.255.254.0 gw 192.240.16.2

#A16ProjectHope
post-up route add -net 192.240.2.128 netmask 255.255.255.248 gw 192.240.16.2

#A17ClientIrys
post-up route add -net 192.240.2.64 netmask 255.255.255.248 gw 192.240.16.2

#A18ClientKroniBae
post-up route add -net 192.240.2.0 netmask 255.255.255.192 gw 192.240.16.2

#A11HoloAdvent
post-up route add -net 192.240.40.0  netmask 255.255.255.252 gw 192.240.16.2

#A19ClientFuwadll
post-up route add -net 192.240.8.0  netmask 255.255.255.224 gw 192.240.16.2

#A3Holoro
post-up route add -net 192.239.208.0 netmask 255.255.255.252 gw 192.239.160.2

#A4Area15
post-up route add -net 192.239.132.0 netmask 255.255.255.252 gw 192.239.160.2

#A9ClientMoonadll
post-up route add -net 192.239.128.0 netmask 255.255.252.0 gw 192.239.160.2

#A8ClientAnya
post-up route add -net 192.239.144.0 netmask 255.255.255.192 gw 192.239.160.2

#A6Holoh3ro
post-up route add -net 192.239.138.0 netmask 255.255.255.252 gw 192.239.160.2

#A7ClientZetadll
post-up route add -net 192.239.136.0 netmask 255.255.254.0 gw 192.239.160.2

#A10GEN&DEV
post-up route add -net 192.239.32.0 netmask 255.255.255.248 gw 192.239.64.2

#A14ClientRirikadll
post-up route add -net 192.239.16.0 netmask 255.255.255.240 gw 192.239.64.2

#A15ClientMiComet
post-up route add -net 192.239.0.0 netmask 255.255.248.0 gw 192.239.64.2

#A21Gamers
post-up route add -net 192.239.10.128 netmask 255.255.255.252 gw 192.239.64.2

#A22ClientFBKdll
post-up route add -net 192.239.8.0 netmask 255.255.254.0 gw 192.239.64.2

#A20ClientKoronedll
post-up route add -net 192.239.10.0 netmask 255.255.255.128 gw 192.239.64.2
```

•	Holo-EN

```
#HoloENA12-A13Client
post-up route add -net 192.240.0.0 netmask 255.255.254.0 gw 192.240.4.2

#A16ProjectHope
post-up route add -net 192.240.2.128 netmask 255.255.255.248 gw 192.240.4.2

#A17ClientIrys
post-up route add -net 192.240.2.64 netmask 255.255.255.248 gw 192.240.4.2

#A18ClientKroniBae
post-up route add -net 192.240.2.0 netmask 255.255.255.192 gw 192.240.4.2

#A19ClientFuwadll
post-up route add -net 192.240.8.0 netmask 255.255.255.224 gw 192.240.40.2
```

•	HoloMyth

```
#MythA12HololiveA1
post-up route add -net 192.240.16.0 netmask 255.255.255.252 gw 192.240.4.1

#A17ClientIrys
post-up route add -net 192.240.2.64 netmask 255.255.255.248 gw 192.240.2.130

#A18ClientKroniBae
post-up route add -net 192.240.2.0 netmask 255.255.255.192 gw  192.240.2.131
```

•	HoloAdvent

```
#A1Hololive
post-up route add -net 192.240.40.0  netmask 255.255.255.252 gw 192.240.40.1
```

•	Holo-ID

```
#A9ClientMoonadll
post-up route add -net 192.239.128.0 netmask 255.255.252.0 gw 192.239.132.2

#A8ClientAnyadll
post-up route add -net 192.239.144.0 netmask 255.255.255.192 gw 192.239.208.2

#A7ClientZetadll
post-up route add -net 192.239.136.0 netmask 255.255.254.0 gw 192.239.138.2
```

•	AREA15

```
#A3Hololive
post-up route add -net 192.239.160.0 netmask 255.255.255.252 gw 192.239.132.1
```

•	Holoro

```
#A3Holoro
post-up route add -net 192.239.160.0  netmask 255.255.255.252 gw 192.239.208.1
```

•	Holoh3ro

```
#A3Hololive
post-up route add -net 192.239.160.0 netmask 255.255.255.252 gw 192.239.138.1
```

•	Holo-Jp

```
#A14ClientRirikadll
post-up route add -net 192.239.16.0 netmask 255.255.255.240 gw 192.239.32.2

#A15ClientMicometdll
post-up route add -net 192.239.0.0 netmask 255.255.248.0 gw 192.239.32.3

#A21Gamers
post-up route add -net 192.239.10.128 netmask 255.255.255.252 gw 192.239.32.3

#A22ClientFBKdll
post-up route add -net 192.239.8.0 netmask 255.255.254.0 gw 192.239.32.3

#A20ClientKoronedll
post-up route add -net 192.239.10.0 netmask 255.255.255.128 gw 192.239.32.3
```

•	GEN-0

```
#A2Hololive
post-up route add -net 192.239.64.0 netmask 255.255.255.252 gw 192.239.32.1

#A21Gamers
post-up route add -net 192.239.10.128 netmask 255.255.255.252 gw 192.239.0.4

#A22ClientFBKdll
post-up route add -net 192.239.8.0 netmask 255.255.254.0 gw 192.239.0.4

#A20ClientKoronedll
post-up route add -net 192.239.10.0 netmask 255.255.255.128 gw 192.239.0.4
```

•	DEV-IS

```
#A2Hololive
post-up route add -net 192.239.64.0 netmask 255.255.255.252 gw 192.239.32.1
```

•	GEN:1

```
#A2Hololive
post-up route add -net 192.239.64.0 netmask 255.255.255.252 gw 192.239.32.1

#A21Gamers
post-up route add -net 192.239.10.128 netmask 255.255.255.252 gw 192.239.0.4

#A22ClientFBKdll
post-up route add -net 192.239.8.0 netmask 255.255.254.0 gw 192.239.0.4

#A20ClientKoronedll
post-up route add -net 192.239.10.0 netmask 255.255.255.128 gw 192.239.10.130
```

•	GAMERS

```
#A2Hololive
post-up route add -net 192.239.64.0 netmask 255.255.255.252 gw 192.239.10.129

#A10HoloJP
post-up route add -net 192.239.32.0 netmask 255.255.255.248 gw 192.239.32.1
```
