![2](https://github.com/user-attachments/assets/6fd8b863-0811-4f21-a1f8-406e51621a79)# Jarkom-Modul-4-IT18-2024

**KELOMPOK IT18**
| Nama | NRP |
|---------------------------|------------|
|Hazwan Adhikara Nasution | 5027231017 |
|Farand Febriansyah | 5027231084 |

<hr>

## Topology

**Cisco Packet Tracer**
<img src="./public/image.png">


# CIDR

## Topology

![topologi-modul-4](https://github.com/user-attachments/assets/a0acf502-d0a9-4932-b1b9-4b47ef6dfb8d)

## **Pembagian IP**

![image](https://github.com/user-attachments/assets/091317c2-5f34-4163-90fa-da4afb347645)

## Pennggabungann

### Langkah 1

![1](https://github.com/user-attachments/assets/53b5b894-88af-4f51-b077-643dbbe4d93b)


### Langkah 2

![2](https://github.com/user-attachments/assets/d35f1359-a6bf-44bf-a7b0-6edcc0b1c754)


### Langkah 3

![3](https://github.com/user-attachments/assets/770b7600-7f86-4840-be37-ccc2a1f25a5b)


### Langkah 4

![4](https://github.com/user-attachments/assets/c2e84d57-9ef2-4119-b439-38822f62d57a)


### Langkah 5

![5](https://github.com/user-attachments/assets/dfc9c89c-d6b4-4b3c-b5ea-910669d22190)

### Langkah 6

![6](https://github.com/user-attachments/assets/a3941c8f-804e-4557-899c-2a9b8c5d9fb4)


### Langkah 7

![7](https://github.com/user-attachments/assets/a3193667-3125-4fe5-92da-45747c6ef228)


### Langkah 8

![8](https://github.com/user-attachments/assets/1a7d61e2-d24e-4571-b440-7d6658f92003)

### Langkah 9

![image](https://github.com/user-attachments/assets/b13a1c24-50a6-4839-86a2-ee09641bb972)

### Langkah 10

![10](https://github.com/user-attachments/assets/66f0b7fb-e229-44cc-8cce-ba25c0a50d2d)

### Langkah 11

![11](https://github.com/user-attachments/assets/686998f2-297a-4d71-b86e-51f37690e617)

## **Tree**

![Untitled Diagram](https://github.com/user-attachments/assets/55d4c2ad-3ea8-409c-99de-792988c7f0d8)

## **Network Configuration**

### Hololive (Gateway)
```
#A15
bash
auto eth1
iface eth1 inet static
    address 192.242.66.5
    netmask 255.255.255.252

#A1
auto eth2
iface eth2 inet static
    address 192.242.4.5
    netmask 255.255.255.252

#A8
auto eth3
iface eth3 inet static
    address 192.242.10.25
    netmask 255.255.255.252
```

### Holo-EN (Gateway)
```
#A15
auto eth0
iface eth0 inet static
    address 192.242.66.6
    netmask 255.255.255.252
    gateway 192.242.66.5

#A16
auto eth1
iface eth1 inet static
    address 192.242.66.1
    netmask 255.255.255.252

#A21
auto eth2
iface eth2 inet static
    address 192.242.16.33
    netmask 255.255.255.252
```

### Holo-Myth (Gateway)
```
#A16
auto eth0
iface eth0 inet static
    address 192.242.66.2
    netmask 255.255.255.252
    gateway 192.242.66.1

#A17
auto eth1
iface eth1 inet static
    address 192.242.64.1
    netmask 255.255.254.0

#A19
auto eth2
iface eth2 inet static
    address 192.242.32.65
    netmask 255.255.255.248
```

### Gura_Ame_Ina (Client)
```
#A17
auto eth0
iface eth0 inet static
    address 192.242.64.2
    netmask 255.255.254.0
    gateway 192.242.64.1
```

### Kiara_Calli (Client)
```
#A17
auto eth0
iface eth0 inet static
    address 192.242.64.3
    netmask 255.255.254.0
    gateway 192.242.64.1
```

### Holo Advent (Gateway)
```
#A21
auto eth0
iface eth0 inet static
    address 192.242.16.34
    netmask 255.255.255.252
    gateway 192.242.16.33

#A22
auto eth1
iface eth1 inet static
    address 192.242.16.1
    netmask 255.255.255.224
```

### FuwaMoco (Client)
```
#A22
auto eth0
iface eth0 inet static
    address 192.242.16.2
    netmask 255.255.255.224
    gateway 192.242.16.1
```

### Shiori_Nerissa (Client)
```
#A22
auto eth0
iface eth0 inet static
    address 192.242.16.3
    netmask 255.255.255.224
    gateway 192.242.16.1
```

### Biboo (Client)
```
#A22
auto eth0
iface eth0 inet static
    address 192.242.16.4
    netmask 255.255.255.224
    gateway 192.242.16.1
```

### Project-Hope (Gateway)
```
#A19
auto eth0
iface eth0 inet static
    address 192.242.32.66
    netmask 255.255.255.248
    gateway 192.242.32.65

#A18
auto eth1
iface eth1 inet static
    address 192.242.32.73
    netmask 255.255.255.248
```

### Irys (Client)
```
#A18
auto eth0
iface eth0 inet static
    address 192.242.32.74
    netmask 255.255.255.248
    gateway 192.242.32.73
```

### Holo-Council (Gateway)
```
#A19
auto eth0
iface eth0 inet static
    address 192.242.32.67
    netmask 255.255.255.248
    gateway 192.242.32.65

#A20
auto eth1
iface eth1 inet static
    address 192.242.32.1
    netmask 255.255.255.192
```

### Kronii_Mumei (Client)
```
#A20
auto eth0
iface eth0 inet static
    address 192.242.32.2
    netmask 255.255.255.192
    gateway 192.242.32.1
```

### Bae_Fauna (Client)
```
#A20
auto eth0
iface eth0 inet static
    address 192.242.32.3
    netmask 255.255.255.192
    gateway 192.242.32.1
```

### Holo-ID (Gateway)
```
#A1
auto eth0
iface eth0 inet static
    address 192.242.4.6
    netmask 255.255.255.252

#A2
auto eth1
iface eth1 inet static
    address 192.242.4.1
    netmask 255.255.255.252

#A4
auto eth2
iface eth2 inet static
    address 192.242.16.65
    netmask 255.255.255.252

#A6
auto eth3
iface eth3 inet static
    address 192.242.34.1
    netmask 255.255.255.252
```
### AREA15 (Gateway)
```
#A2
auto eth0
iface eth0 inet static
    address 192.242.4.2
    netmask 255.255.255.252
    gateway 192.242.4.1

#A3
auto eth1
iface eth1 inet static
    address 192.242.0.1
    netmask 255.255.252.0
```

### lofi (Client)
```
#A3
auto eth0
iface eth0 inet static
    address 192.242.0.2
    netmask 255.255.252.0
    gateway 192.242.0.1
```

### Moona (Client)
```
#A3
auto eth0
iface eth0 inet static
    address 192.242.0.3
    netmask 255.255.252.0
    gateway 192.242.0.1
```

### Risu (Client)
```
#A3
auto eth0
iface eth0 inet static
    address 192.242.0.4
    netmask 255.255.252.0
    gateway 192.242.0.1
```

### holoro (Gateway)
```
#A4
auto eth0
iface eth0 inet static
    address 192.242.16.66
    netmask 255.255.255.252
    gateway 192.242.16.65

### A5
auto eth1
iface eth1 inet static
    address 192.242.16.1
    netmask 255.255.252.192
```

### Ollie (Client)
```
#A5
auto eth0
iface eth0 inet static
    address 192.242.16.2
    netmask 255.255.252.192
    gateway 192.242.16.1
```

### Anya (Client)
```
#A5
auto eth0
iface eth0 inet static
    address 192.242.16.3
    netmask 255.255.252.192
    gateway 192.242.16.1
```

### Reine (Client)
```
#A5
auto eth0
iface eth0 inet static
    address 192.242.16.4
    netmask 255.255.252.192
    gateway 192.242.16.1
```

### holoh3ro (Gateway)
```
#A6
auto eth0
iface eth0 inet static
    address 192.242.34.2
    netmask 255.255.255.252
    gateway 192.242.34.1
```
