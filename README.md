# Superbi
## 引言
superbi 是达闼科技以开源项目superset为基础开发的企业级快速BI应用。
可扩展的框架设计，支持多种DBMS数据源，让数据BI更加简单。
superbi提供直观的UI，拖拽式的编辑体验，配置式的图例创建，轻松创建数据可视化dashboard的能力。

## 图例展示
[![](https://i.loli.net/2020/10/23/6jRYo2ZpOaD8yXz.png)](https://i.loli.net/2020/10/23/6jRYo2ZpOaD8yXz.png)

## superbi能做什么
- 提供丰富的可视化图例，包含基本的折线图，饼图，GL可视化图例等近60种图例
- 简单易用，无需代码，配置式创建的图例，拖拽编辑体验的dashboard。
- 先进的SQL在线编辑器，IDE式的体验，让你可以方便快捷的浏览元数据。
- 集成企业级的用户权限管理，并可以与其他身份验证系统集成（OpenID, LDAP, OAuth, REMOTE_USER）
- 自定义SQL扩展，提供对复杂情况的数据可视化能力。
- 集成echarts，3d word cloud，更加高度可配置的图表UI效果展示



## 支持的数据库
|             数据库类型           |          驱动安装        |       连接字符串          |
| ---------------------- | ------------------------ | ------------------------ |
|  clickhouse  |  pip install sqlalchemy-clickhouse  |   clickhouse://{username}:{password}@{hostname}:{port}/{database}  |
| Apache Kylin | pip install kylinpy | kylin://{username}:{password}@{hostname}:{port}/{project}?{param1}={value1}&{param2}={value2} |
|Apache Hive|pip install pyhive|hive://hive@{hostname}:{port}/{database}|
|Apache Impala|pip install impala|impala://{hostname}:{port}/{database}|
|Apache Spark SQL|pip install pyhive|hive://hive@{hostname}:{port}/{database}|
|MySQL| pip install mysqlclient| mysql://&lt;UserName>:&lt;DBPassword>@&lt;Database Host>/&lt;Database Name>|
|PostgreSQL|pip install psycopg2|postgresql:://&lt;UserName>:&lt;DBPassword>@&lt;Database Host>/&lt;Database Name>|
## 安装&运行
### 前置依赖
1. docker
2. docker-compose

### 安装步骤

    git clone https://github.com/CloudmindsRobot/superBI.git
    
    cd superbi
    
    docker-compose up
	
启动成功后在浏览器中输入地址http://localhost:8088 即可访问
- 用户名： admin
- 密码: admin



