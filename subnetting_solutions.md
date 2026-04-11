# Part 2 - Section B

# Exercise 1

Original: 192.168.10.0/24
Need 4 subnets → borrow 2 bits
New prefix: /26
Addresses per subnet: 2^6 = 64
Usable hosts per subnet: 64 - 2 = 62
Subnet mask: 255.255.255.192

| Subnet | Network Address | First Usable  | Last Usable    | Broadcast      | Subnet Mask     | CIDR |
|--------|-----------------|---------------|----------------|----------------|-----------------|------|
| 1      | 192.168.10.0    | 192.168.10.1  | 192.168.10.62  | 192.168.10.63  | 255.255.255.192 | /26  |
| 2      | 192.168.10.64   | 192.168.10.65 | 192.168.10.126 | 192.168.10.127 | 255.255.255.192 | /26  |
| 3      | 192.168.10.128  | 192.168.10.129| 192.168.10.190 | 192.168.10.191 | 255.255.255.192 | /26  |
| 4      | 192.168.10.192  | 192.168.10.193| 192.168.10.254 | 192.168.10.255 | 255.255.255.192 | /26  |


# Exercise 2

Network: 172.16.0.0/16

| Department  | Network Address | First Usable | Last Usable  | Broadcast    | Subnet Mask     | CIDR |
|-------------|-----------------|--------------|--------------|--------------|-----------------|------|
| Engineering | 172.16.0.0      | 172.16.0.1   | 172.16.0.254 | 172.16.0.255 | 255.255.255.0   | /24  |
| HR          | 172.16.1.0      | 172.16.1.1   | 172.16.1.62  | 172.16.1.63  | 255.255.255.192 | /26  |
| Sales       | 172.16.1.64     | 172.16.1.65  | 172.16.1.94  | 172.16.1.95  | 255.255.255.224 | /27  |
| Management  | 172.16.1.96     | 172.16.1.97  | 172.16.1.110 | 172.16.1.111 | 255.255.255.240 | /28  |

# Exercise 3

IP Address:    192.168.1.150
Subnet Mask:   255.255.255.192
Default Gateway: 192.168.1.1

1- The computer belongs to 192.168.1.128/26

2- Valid host range: 192.168.1.129 - 192.168.1.190

3- The computer cannot communicate with the default gateway because it is in a diffrent subnet.

4- Change the subnet mask to 255.255.255.0 so that they are on the same subnet.
