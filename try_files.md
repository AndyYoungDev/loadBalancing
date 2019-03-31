# try_files 配置
```
try_files $uri $uri/ /index.php;
```
* 当www.test.com/test,先寻找test文件和目录,fallback第三个参数,请求交给index.php。
* 请求会被location ~ \.php$ { ... }接收到，转发给fpm处理。


# 正则表达式
* ^ 匹配输入字符串的开始位置
* $ 匹配输入字符串的结束位置
* \.php$ 匹配.php结尾的文件
