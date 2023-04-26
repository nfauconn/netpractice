# IPV4

Masks: after 1 bit set to 0, there cant be '1' bits anymore
--> only available numbers =
- 255 (11111111)
- 254 (11111110)
- 252 (11111100)
- 248 (11111000)
- 240 (11110000)
- 224 (11100000)
- 192 (11000000)
- 128 (10000000)
- 0   (00000000)

*--> 255.255.255.128 is a valid mask*
*--> 255.255.128.128 is not a valid mask*
*--> 255.255.128.0 is a valid mask*


## SPECIAL IP RANGE

Reserved for private networks :
- 10.0.0.0 until 10.255.255.255         10.*
- 172.16.0.0 until 172.31.255.255       172.16.* --> 172.32.* (not include)
- 192.168.0.0 until 192.168.255.255     192.168.*

Reserved for so called loop back addresses:
- 127.0.0.0 until 127.255.255.255       127.*


## MASKS

Dot decimal notation : 255.255.255.0
Class Inter Domain Routine (CIDR): /24

| CIDR |   Dot-decimal   | IP addr / subnet | Usable IP-addr / subnet | Nb subnets |
| ---- | --------------- | ---------------- | ----------------------- | ---------- |
| /32  | 255.255.255.255 |        1         |           0             |     256    |
| /31  | 255.255.255.254 |        2         |           1             |     128    |
| /30  | 255.255.255.252 |        4         |           2             |      64    |
| /29  | 255.255.255.248 |        8         |           6             |      32    |
| /28  | 255.255.255.240 |       16         |          14             |      16    |
| /27  | 255.255.255.224 |       32         |          30             |       8    |
| /26  | 255.255.255.192 |       64         |          62             |       4    |
| /25  | 255.255.255.128 |      128         |         126             |       2    |
| /24  | 255.255.255.0   |      256         |         254             |       1    |
