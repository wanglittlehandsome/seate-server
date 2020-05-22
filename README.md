# seate-server 
### version 1.2.0

#### 一、配置：

##### 1.修改registry.conf
    1. registry.type = "nacos" nacos中的serverAddr和username,password根据自己的配置
    2. registry.config = "file" 指向不变，接下来就是就是file.conf文件
##### 2.file.conf
    1. mode = "db"
    2. db 配置项中 url,user,password根据自己mysql填写
    3. PS: 为什么选择db模式而不是file模式？ 是因为file适合单机测试(内存读写)，生产应用还是需要db模式，事务信息存在在mysql中天然支持
           分布式部署
#### 二、启动：

##### 1.windows启动：
     双击 seata-server.bat
 
##### 2.linux启动：
     sh ./seata-server,sh    