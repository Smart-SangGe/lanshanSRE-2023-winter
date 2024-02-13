# lanshanSRE-2023-winter

### 考核问题

一.git基本命令使用，git代理怎么设置

二.dockerdile里面常用字段

三.dockercompose常用字段

四.介绍一下代码注释，挑部分代码问问作用，怎么实现

## 共同改进之处

1. 可以学习测试驱动开发模式，即先编写测试代码，再实现函数功能通过测试样例。

## 胡跃敏

完成度相当不错，代码方面可以继续改进

### 改进之处

1. commit信息不够完善，不能只有update， 应该加上具体的改动描述。（可利用gpt生成）  
2. 对于python还是不够熟练，仓库里的shell文件基本上可以用os和subprocess来执行。  
3. 在编写函数的时候，添加type lint和usage document。 有助于自己debug和编写unit test。  
4. 对于git的分支不够熟练，每次更新迭代应该在dev branch里操作测试没问题后，通过pr合并到main branch中。  
5. 对于docker版本，可以考虑加入参数解析，这样不需要进入容器进行二次操作。  
6. 对于docker中安装lamp环境，由于docker内部没有systemd，所以可以
  考虑mounting docker socket或者使用docker in docker，构建容器化的lamp环境。  
7. 容器内没办法监控宿主机，可以考虑使用privilege mode  

### 提问

1.git代理如何设置？例如在clone或者pull中遇到了443情况

2.克隆，拉取更新命令，推送命令，git fetch作用

3.from，label字段大概意义，copy . .大致意思

4.docker run -p 8080:80 -d witch6/winter_test:3.11  /bin/bash -c "while true; do sleep 1;done"这部分具体意思

5.查看运行程序那里的那段代码跟这个网页版是否有点儿多余？

## 刘青青

完成度极低，非常难评

### 提问

没约时间，再说

## 徐航

完成度也相当不错，项目管理方面可以继续改进

### 改进之处

1. commit信息不够完善，一次性提交也不是不行，但是确实没看到迭代过程。  
2. 使用明文密码存储。  
3. 对于github的分支不够熟练，default分支里面是空的。  
4. 对于python不够熟练，例如数据库方面可以使用python内置的sqlite，而没必要再运行一个mysql
  （从需求分析上来讲，数据库只有单用户单程序的读写需求。或者也可以使用sqlalchemy，可以让用户自行配置存储后端）  
5. 代码中的应该避免使用print来输出日志信息，python中可以使用logging库来实现区分等级，存储到日志文件等功能。  
6. 应当使用Gunicorn 或 uWSGI作为服务器，并且在启动时关闭debug模式。
7. 对于git的应用不够熟练，例如说数据库文件不应该被track，建议学习gitignore的用法。  

### 提问

20号过后才有时间
