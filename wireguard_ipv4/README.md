# wireguard_ipv4

### 此处唯一区别就是 脚本文件内的 这两行配置 （这是脚本生成客户端配置文件的部分内容）

```bash

294  AllowedIPs = ${SERVER_NETWORK_SEGMENT}, ${CLIENT_WG_IPV4}/32

295  #AllowedIPs = 0.0.0.0/0

```


#### 294行  脚本内使用这行配置，是本地连上云服务器的内外ip地址可以使用此配置，本地客户端连上vpn之后 本地可以ping通 vpn 服务端的ip地址 


#### 295行  脚本内使用这行配置，是转发所有流量，一般只有把 VPN 当做武当纵云梯来用时，才会需要转发所有流量，不多说，点到为止。