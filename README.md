# nginx 负载均衡
## nginx.conf 配置负载服务器
* weight 权重
```
http{
    upstream php_pool{
        server 192.168.1.1:80 weight=10;
        server 192.168.1.2:80 weight=20;
    }
}
```
## 端口配置文件
```
    location / {
        proxy_pass http://php_tool
    }
```