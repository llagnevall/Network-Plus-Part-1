# Lab – Identify IPv6 Addresses

## Objectives

- **Part 1:** Practice with Different Types of IPv6 Addresses  
- **Part 2:** Examine a Host IPv6 Network Interface and Address

---

## Background / Scenario

With IPv4 address space depletion and the transition to IPv6, networking professionals must understand IPv6 address types and configuration. This lab focuses on identifying IPv6 address types, compressing/decompressing IPv6 addresses, and examining IPv6 settings on a PC.

---

## Required Resources

- 1 PC (Windows with Internet access)

---

## Part 1: Practice with Different Types of IPv6 Addresses

### Step 1: Match the IPv6 Address to Its Type

**Answer choices:**

- a. Loopback address  
- b. Global unicast address  
- c. Link-local address  
- d. Unique-local address  
- e. Multicast address  

| IPv6 Address                          | Answer |
|--------------------------------------|--------|
| 2001:0db8:1:acad::fe55:6789:b210     |     b   |
| ::1                                  |    a    |
| fc00:22:a:2::cd4:23e4:76fa           |    d    |
| 2033:db8:1:1:22:a33d:259a:21fe       |    b    |
| fe80::3201:cc01:65b1                 |     d   |
| ff00::                               |    c    |
| ff00::db7:4322:a231:67c              |     e   |
| ff02::2                              |     c   |

---

### Step 2: Compress and Decompress IPv6 Addresses

Use IPv6 abbreviation rules to compress or decompress the following:

1. **2002:0ec0:0200:0001:0000:04eb:44ce:08a2**  
   _Compressed: 2002:ec0:200:1:0:4eb:44ce:8a2  

2. **fe80:0000:0000:0001:0000:60bb:008e:7402**  
   _Compressed: fe90::1:0:60bb:8e:7402  

3. **fe80::7042:b3d7:3dec:84b8**  
   _Decompressed: fe80:0000:0000:0000:7042:b3d7:3dec:84b8    

4. **ff00::**  
   _Decompressed: ff00:0000:0000:0000:0000:0000:0000:0000  

5. **2001:0030:0001:acad:0000:330e:10c2:32bf**  
   _Compressed: 2001:30:1:acad:0:330e:10c2:32bf 

---

## Part 2: Examine a Host IPv6 Network Interface and Address

### Step 1: Check Your PC IPv6 Network Address Settings

1. Open **Control Panel**  
2. Go to **Network and Sharing Center**  
3. Click **Change adapter settings**  
4. Right-click active network interface → **Properties**  
5. Verify **Internet Protocol Version 6 (TCP/IPv6)** is installed and active  
6. Click **Properties** to view IPv6 settings  
7. Open Command Prompt and run:  
   ```bash
   ipconfig /all
   ```


Link-local IPv6 Address . . . . . : fe80::429c:b64b:73f6:18cc%3(Preferred)
   IPv4 Address. . . . . . . . . . . : 10.4.32.153(Preferred)
   Subnet Mask . . . . . . . . . . . : 255.255.252.0
   Lease Obtained. . . . . . . . . . : Tuesday, September 9, 2025 11:22:33 AM
   Lease Expires . . . . . . . . . . : Wednesday, September 17, 2025 11:22:34 AM
   Default Gateway . . . . . . . . . : 10.4.32.1
   DHCP Server . . . . . . . . . . . : 10.4.100.25
   DHCPv6 IAID . . . . . . . . . . . : 59567179
   DHCPv6 Client DUID. . . . . . . . : 00-01-00-01-2D-D7-EF-90-6C-2B-59-CE-5A-63
   DNS Servers . . . . . . . . . . . : 10.4.100.25
                                       10.7.100.24
                                       10.3.69.16
## Questions 

- What does it indicate about the network regarding IPv6 global unicast, unique-local, or gateway address?
Answer: 
- What kind of IPv6 addresses did you find using ipconfig /all?
Answer: It is a link local address as indicated by the fe80


## Reflection Questions

1. How do you think you must support IPv6 in the future?
Answer: IPv6 will simply need to be enabled and used as the primary IP on any created networks from the point that it is viable to use

2. Do you think IPv4 networks will continue, or will everyone eventually switch to IPv6? How long do you think it will take?
Answer:
 I think IPv4 is likely to still see use in small local networks that only need a very small number of Ips to function where it would be more work to convert the network to IPv6. Generalized conversion will likely still take another 5 or so years at least.
