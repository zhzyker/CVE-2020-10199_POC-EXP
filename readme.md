影响版本 <= 3.21.1
需要用户登录后提供csrf和sessionid（登录成功后从浏览器复制），代码执行目前无法回显
# POC
```
+----------------------------------------------------------------------------------------------------------+
+ DES: by zhzyker as https://github.com/zhzyker/exphub                                                     +
+      CVE-2020-10199 need username & password                                                             +
+----------------------------------------------------------------------------------------------------------+
+ USE: python3 <filename> <ip> <port> <csrf> <sessionid>                                                   +
+ EXP: python3 cve-2020-10199_poc.py 1.1.1.1 8081 0.9567822851573897 edfca15e-c721-45e2-bdef-e8b3c6364ddb  +
+ VER: Nexus Repository Manager OSS/Pro version <= 3.21.1                                                  +
+----------------------------------------------------------------------------------------------------------+
```
# EXP
```
+----------------------------------------------------------------------+
+ DES: by zhzyker as https://github.com/zhzyker/exphub                 +
+      CVE-2020-10199 Nexus 3 remote command execution                 +
+----------------------------------------------------------------------+
+ USE: python3 <filename> <url> <username> <password>                  +
+ EXP: python3 cve-2020-10199_cmd.py http://127.0.0.1:8081 admin admin +
+ VER: Nexus Repository Manager 3.x OSS / Pro <= 3.21.1                +
+----------------------------------------------------------------------+
```

更多EXP参考 https://github.com/zhzyker/exphub
