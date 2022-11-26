# Jarkom-Modul-4-C07-2022
laporan resmi Praktikum Jaringan Komputer Modul 1 tahun 2022

Anggota Kelompok C07 :
* 5025201274 - Alif Adrian Anzary
* 5025201122 - Marsyavero Charisyah Putra
* 5025201209 - Hemakesha Ramadhani Heriqbaldi

topologi:


</br>

* Cisco packet Tracer menggunakan VLSM
* GNS3 menggunakan CIDR

## VLSM (Cisco Packet Tracer):

Subnetting yang kami gunakan:
![topologi_final](https://user-images.githubusercontent.com/78362238/204092696-3fe7cab7-c359-4f1f-a64c-f389629052da.png)

Plotting Untuk Subnettingnya adalah:

|Subnet|Jumlah Host|Netmask|
|------|-----------|-------|
|  A1  |    1001   |  /22     |
|  A2  |    501    |  /23     |
|  A3  |     271   |  /23     |
|  A4  |     251   |  /23     |
|  A5  |      211  |  /24     |
|  A6  |       121 |  /25     |
|  A7  |     121   |  /25     |
|  A8  |    71     |  /25     |
|  A9  |     51    |  /26     |
|  A10 |     2     |  /30     |
|  A11 |    2      |  /30     |
|  A12 |    2      |  /30     |
|  A13 |   2       |  /30     |
|  A14 |    2      |  /30     |
|  A15 |   2       |  /30     |
|  A16 |   2       |  /30     |
|  A17 |    2      |  /30     |
|  A18 |    2      |  /30     |


VLSM dari Subnetting:
![subnetdecisiontree](https://user-images.githubusercontent.com/78362238/204087513-dfbb7811-a96d-4f01-b9ad-a700a564673c.jpg)

Pembagian IP setiap subnet:

|Subnet|Network ID |Netmask|
|------|-----------|-------|
|  A1  |    10.13.4.0      |  255.255.252.0     |
|  A2  |    10.13.2.0      |  255.255.254.0     |
|  A3  |     10.13.10.0    |  255.255.254.0     |
|  A4  |     10.13.1.0     |  255.255.254.0     |
|  A5  |      10.13.9.0    |  255.255.255.0     |
|  A6  |     10.13.0.128   |  255.255.255.128   |
|  A7  |     10.13.8.128   |  255.255.255.128   |
|  A8  |    10.13.8.0      |  255.255.255.128   |
|  A9  |     10.13.0.64    |  255.255.255.192     |
|  A10 |     10.13.0.0     |  255.255.255.252     |
|  A11 |    10.13.0.4      |  255.255.255.252     |
|  A12 |    10.13.0.8      |  255.255.255.252     |
|  A13 |   10.13.0.12      |  255.255.255.252     |
|  A14 |    10.13.0.16     |  255.255.255.252     |
|  A15 |   10.13.0.20      |  255.255.255.252     |
|  A16 |   10.13.0.24      |  255.255.255.252     |
|  A17 |    10.13.0.28     |  255.255.255.252     |
|  A18 |    10.13.0.32     |  255.255.255.252     |


## Routing

Routing pada tiap router:


### The Resonance
| Subnet | IP | Netmask | Next Hop |
|--------|----|---------|----------|
| A9   | 10.13.0.64 | /26| 10.13.0.2|
|      | 0.0.0.0 |/0     | 10.13.0.2|
| A3   | 10.13.10.0 | /23| 10.13.0.10|


## CIDR (GNS3):