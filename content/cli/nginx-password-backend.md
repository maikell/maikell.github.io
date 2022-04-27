---
title: "Nginx backend password protected"
date: 2022-04-27
menu: "CLI"
weight: 1 
---
### Nginx backend password protected
Nginx as a proxy allow to access backend (Apache) content which is password protected

**Nginx server configuration**
```
proxy_set_header Authorization $http_authorization;
```


##### source
* https://serverfault.com/questions/390157/nginx-as-a-proxy-doesnt-allow-to-access-backend-apache-content-which-is-passw
* https://stackoverflow.com/a/65308098