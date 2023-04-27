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
    > nb de first bits reserves

| CIDR |   Dot-decimal   | Nb subnets | IP addr / subnet | Usable IP-addr / subnet | 
| ---- | --------------- | ---------- | ---------------- | ----------------------- | 
| /24  | 255.255.255.0   |       1    |      256         |         254             | 
| /25  | 255.255.255.128 |       2    |      128         |         126             | 
| /26  | 255.255.255.192 |       4    |       64         |          62             | 
| /27  | 255.255.255.224 |       8    |       32         |          30             | 
| /28  | 255.255.255.240 |      16    |       16         |          14             | 
| /29  | 255.255.255.248 |      32    |        8         |           6             | 
| /30  | 255.255.255.252 |      64    |        4         |           2             | 
| /31  | 255.255.255.254 |     128    |        2         |           1             | 
| /32  | 255.255.255.255 |     256    |        1         |           0             | 


| Adresse IP réservée     | Plage d'adresses IPv4             |                     | Utilisation                                 |
|-------------------------|-----------------------------------|-----------------    |---------------------------------------------|
| 0.0.0.0/8               | 0.0.0.0 - 0.255.255.255           |0,*                  | Réseau par défaut                           |
| 10.0.0.0/8              | 10.0.0.0 - 10.255.255.255         |10.*                 | Réseau privé                                |
| 100.64.0.0/10           | 100.64.0.0 - 100.127.255.255      |100.64.* - 100.127.* | Communication entre opérateurs              |
| 127.0.0.0/8             | 127.0.0.0 - 127.255.255.255       |127.*                | Boucle locale                               |
| 169.254.0.0/16          | 169.254.0.0 - 169.254.255.255     |169.254.*            | Configuration automatique d'adresse IP      |
| 172.16.0.0/12           | 172.16.0.0 - 172.31.255.255       |172.16.* - 172.31.*  | Réseau privé                                |
| 192.0.0.0/24            | 192.0.0.0 - 192.0.0.255           |192.0.0.*            | Adresses spéciales pour documentation       |
| 192.0.2.0/24            | 192.0.2.0 - 192.0.2.255           |192.0.2.*            | Adresses de test pour documentation réseau  |
| 192.88.99.0/24          | 192.88.99.0 - 192.88.99.255       |192.88.99.*          | Tunneling pour IPv6 sur IPv4                |
| 192.168.0.0/16          | 192.168.0.0 - 192.168.255.255     |192.168.*            | Réseau privé                                |
| 198.18.0.0/15           | 198.18.0.0 - 198.19.255.255       |198.18.* - 198.19.*  | Test de performance réseau                  |
| 198.51.100.0/24         | 198.51.100.0 - 198.51.100.255     |198.51.100.*         | Adresses de test pour documentation réseau  |
| 203.0.113.0/24          | 203.0.113.0 - 203.0.113.255       |203.0.113.*          | Adresses de test pour documentation réseau  |
| 224.0.0.0/4             | 224.0.0.0 - 239.255.255.255       |224.* - 239.*        | Multicast                                   |
| 240.0.0.0/4             | 240.0.0.0 - 255.255.255.254       |240.0.* - 255.*      | Réservé pour usage futur                    |
| 255.255.255.255/32      | 255.255.255.255 - 255.255.255.255 |                     | Diffusion locale                            |


Premiere adresse d'une plage = adresse reseau
    > reservee a l'identification du reseau
Derniere adresse d'une plage = adresse de diffusion (broadcast address)
    > reservee a l'envoi de paquets a toutes les interfaces du sous-reseau

