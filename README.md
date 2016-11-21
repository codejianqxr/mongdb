# mongdb
-----

## 安装  
1.  windows安装  
    1.1 [mongodb官网地址](http://www.mongodb.org) 下载安装包  
    1.2 将安装目录下的`bin/`目录,放到系统全局变量下面   
    1.3 将mongodb将入到windows服务 ,用一下命令


    mongod.exe --logpath d:/websoft/mongodb/logs --logappend --dbpath d:/websoft/mongodb/data --directoryperdb --serviceName MongoDB -install  
    
## 启动
1. 启动命令 `mongod --dbpath='指定文件存放的目录'`  
    **默认的端口号是`27017`** 
2. 然后继续开启命令行交互模式,输入命令 `mongo`   
   **mongo 命令给我提供了和mongodb交互的环境,他就是一个javascript解析器**  
3. 开始你的mongodb之旅
4. 如果您不想通过命令行操作,可安装可视化图形工具 `mongvue`, 1.0版本的开始收费了，[免费破解版v1.5.3](http://download.csdn.net/detail/sunboy_2050/6770483) 
      
## 常用命令
1. 选择数据库


    use dbname  
2. 创建    
  
  
 