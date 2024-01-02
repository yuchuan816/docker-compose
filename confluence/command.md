```shell
# confluence 授权
java -jar /Users/liuyuchuan/tom/docker-composes/confluence/build/atlassian-agent.jar -m dqzboy@xxxx -n dqzboy.com -p  conf -o https://confluence.66plat.com/ -s B6IF-QR11-DET9-R943

# confluence 插件授权
java -jar /Users/tom/Desktop/docker-composes/confluence/build/atlassian-agent.jar -m dqzboy@xxxx -n dqzboy.com -o https://confluence.66plat.com/ -s B6IF-QR11-DET9-R943 -p com.stiltsoft.confluence.smart-attachment-for-confluence

# 新建数据库
CREATE DATABASE confluence CHARACTER SET utf8 COLLATE utf8_bin;

# 修改数据库字符集
ALTER DATABASE confluence CHARACTER SET utf8mb4 COLLATE utf8mb4_bin

# 新建用户
CREATE USER 'confluence'@'%' IDENTIFIED BY 'confluence';

# 赋予用户权限
GRANT ALL PRIVILEGES ON confluence.* TO 'confluence'@'%';

flush privileges;
```
