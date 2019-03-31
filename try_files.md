# try_files 配置
```
try_files $uri $uri/ /index.php;
```
* 当www.test.com/test,先寻找test文件和目录,fallback第三个参数,请求交给index.php。
* 请求会被location ~ \.php$ { ... }接收到，转发给fpm处理。
