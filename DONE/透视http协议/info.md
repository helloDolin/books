# Hyper Text Transfer Protocol
WebSocket
wget
curl
都是基于 HTTP

# Domain Name System
DNS
可以实现基于域名的负载均衡

# SSL/TLS

# Content Delivery Network
CDN
作用：缓存、加速

# 代理
传输过程中的中转站，可以实现缓存加速、负载均衡等

# 用 Charles 查看原始（Raw）的报文
=================================================== req
POST /api/v2/transaction/coinTrade HTTP/1.1
Host: 175.178.207.169
Content-Length: 1112
Accept: application/json, text/plain, */*
compress: 1
User-Agent: Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) aicoin/2.11.10 Chrome/108.0.5359.215 Electron/22.3.27 Safari/537.36 AICoin/2.11.10
Content-Type: application/json
Accept-Encoding: gzip, deflate
Accept-Language: zh-CN
Connection: keep-alive

{"p":"sRqUto7hxLoKDzOaoOi/ZUulAN7k5VFR4FVBvp+ZST7a+pk5MG3Edtj9cVEWev4fOfioDcyEBgR1f+KYMM3e+/VJ+1KfnnbxjWjURekj6lZC5zC6W9zOgc0+TuRKv7zllQPDZoGPcCHG0OJgEqIp9OZCMFOfIBYhY6AT5+aDZN1ScpJiLAgbjKiDUYuRotppSebDc5LIU0yccILprEkI/Knqcrjz1O9zC6UGQbfYZofAmAEfnulmfmSR7844TooPIHyxruw280ut8GO6Y8fozi+KN/mKO4DaXgPguzyXz5/pByaxH4ch7Dkt08YNXLoo0aew/gr7sUOi528j2+MIERgxBd4io0YnxIT05GYkaVDUSZ5fF52Fn63T+9kPJMus1dr4jyR8CMjaZWgWrUahxLn8e8Pg6OrxrpuVX6+KJ9ZGIrxSVnnzThN0tqbwazCis0/mb9YMco5GmKCjwvPBG88u+UqK2mFwmSkpb42T+Uz+gWo6HlvGZa0aZJt+EM/TuvLmMabvwBrlrut7b+3L6YdEGgSW8h6c+K3pbe3k1o/ymNSOKzlxn9yPweuUB9eKP5/AK/cVdjsDpcqyKh3QEbfbEjgxDEKCwtzF8TGIl4s6gXPjQziE3QDuMbmYBMOqAOaWkda39qgXEEzagBAs4XvtYhyNxZVKewLd0m+NyHwoKkpJa50dYt9NTnxC2TawhYdLBhhh4S0JyLLLkQGw6A==","k":"KalwQ3v2CWfxN0cYbvyxS+S5LlHrCz107ReTfLjmJqjd6rgTrNAJXzawmTwIP3f43cqtNJBDKnotHSAcieJ2+eht2F0SaH64r2av2WOsdsO0eax8U0Ld+AM5K0qJxecRMV1+6igNj7z3AQvzpCwhuLgX3IAPNX5JFwSMpt6WeOI=","v":"1535898394","iv":"BiZC1INsg2V0jat8HFZz+5dwpFRglw2W0B5tbbj6yjkVWj++xN2DV6bdo3tF8IwjugKg/AgvrQ4KK5o4NR8SwNMYW5fuFIXIdLPI5J8uoy9Hlq4dq2NS29x0wGcWcsCPLh5MsB+C6lZjJqjlE0qN908gBbfHWf69rkTX0Xl55ZI="}

=================================================== res
HTTP/1.1 200 OK
Date: Mon, 16 Dec 2024 15:52:05 GMT
Content-Type: application/json; charset=UTF-8
Content-Length: 295
Decompress: 1
X-Upgrade: true
Proxy-Connection: keep-alive

{"success":true,"message":"success","status":200,"data":"5gR+CGA4GRNDtkikPoeDGhF5s8FIhF5PD1B7RnabFPX1WJYdoykJ2U2Mep+g6v4EJNRPEp+QxCZXJOqDKwHnkiXDj98M1kYK2k3HA9whQXMtdIq3OlAuiA7nLGYYuD0T44rw3O/abJR/3n7Vp5YR22PoDr762nJHgZzx9TjnsBQFxgePhXjfCBekOihzbfyu4jspuCtJhAM1IxKS05xja199jV0QLZCq0B5Sce+tjA0="}

# 1
* HTTP/1.1 是目前互联网上使用最广泛的协议，功能也非常完善
* HTTP/2 基于 Google 的 SPDY 协议，注重性能改善，但还未普及
   压缩头部使之更少的字节数
   服务端可以推送消息到客户端
* HTTP/3 基于 Google 的 QUIC 协议，是将来的发展方向

# URI
只有 ASCII 
如果有 @&? 关键字需要 url 编码

# method
get post
head：
