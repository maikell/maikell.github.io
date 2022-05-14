---
title: "Haproxy cheat sheet"
date: 2022-05-12
menu: "CLI"
weight: 1
---

#### Check syntax 
```
haproxy -f /etc/haproxy/haproxy.cfg -c
```

### ip acl on backend 
```
backend wordpress
        http-request deny if ! { src,map_ip(/etc/haproxy/list.lst) -m found }
        server wordpress 172.5.0.1:8080 check
```

### ip acl with path on backend 
```
backend wordpress
        http-request deny if { path -i -m beg /wp-admin/ } ! { src,map_ip(/etc/haproxy/list.lst) -m found }
        server wordpress 172.5.0.1:8080 check
```

### Correct order of TLS pem file
1. Intermediate
2. domain cert
3. domain key
