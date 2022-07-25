- 归档: [[服务器]]
---

#Azure

## 1.为什么要用云

1.传统IT基础架构的缺点

+ 价格贵
+ 服务器大部分时间处于闲置的状态
+ 维护烦

<br/>

2.云的好处

+ 没有昂贵的前期投入
+ 扩展性
+ 不再担心底层架构

<br/>

3.所有企业并不一定需要上云。根据核心需求决定是否上云。


## 2.什么是云

1.云的定义：**租用**其他公司的计算、存储、网络资源，并**按需付费**。

2.云的分类

+ 公有云
+ 私有云(政府机构、金融机构会考虑采用)
+ 混合云(公有云+私有云)

<br/>

3.全球公有云IaaS市场份额排行

+ top1：AWS
+ top2：Azure
+ top3：阿里云

<br/> 

4.技术侧重点

+ AWS：开源
+ 微软Azure：hypev | sql | .net
+ 阿里：开源

<br/>

## 3.什么是IaaS、PaaS、SaaS

1.on-prem(on-premises software)：本地部署软件

2.IaaS(Infrastructure as a service)：基础设施即服务【速冻饺子】

Azure中的VM

3.PaaS(Platform as a service)：平台即服务【外卖饺子，专注于开发网站】

Web App

4.SaaS(Software as a service)：软件即服务【去饭点随便点单】

Office365

5.其他的\*AAS

BaaS(Backend as a Service)：后端即服务【专注于前端开发】
DRaaS(Disaster Recovery as a Service)：灾难备份即服务【将灾难备份托管给服务提供商】

## 4.Azure国际版与国内版的区别

1.Azure全球基础架构包含了两个最主要的部分

+ 物理基础设施
+ 网络连接组件

<br/>

2.Azure中国和Azure全球

+ 物理上和逻辑上完全独立
+ Azure中国由世纪互联运营
+ Azure全球由微软运营
+ 有些服务国内版的Azure还未上线

<br/>

## 5.Azure上的地域/区域/可用性区域是什么

+ 地域(Geo，如中国)：一个国家或地区
+ 区域(Region)是一组数据中心，每个region内的延迟在2毫秒以下。
+ 可用性区域(Availability Zone)：保证你一个数据中心坏了，另一个数据中心上的实例还正常工作。
 + 区域对儿(Region Pair)：每次更新只更新区域对儿中的一个区域；如果中断影响多个区域，则每对中的至少一个区域将优先进行恢复。

## 6.Azure中的订阅与租户的区别

1.订阅(subscription)

+ 你<—>微软合同
+ 像你的SIM卡
+ 种类
	+ 免费试用订阅
	+ Pay as you go订阅(先用后付)
	+ EA，大企业，1-3年承诺，折扣价，微软支持
	+ Parter，灵活，折扣，帮你部署，帮你维护，省心

<br/>

2.租户(AAD)

+ 纯云，身份，访问
+ 通常代表一家公司
+ AAD≠AD

<br/>

3.

+ 登录Azure=>AAD/租户
+ 部署资源=>订阅/Subscription
+ 一个AAD(公司)有多个订阅
+ 打包订阅到一起

<br/>

## 7.Azure中的资源是怎么部署出来的

1.经典(classic)

自己按顺序部署，挨个删除，访问控制

2.ARM(Azure Resource Manager)：Azure资源管理器

+ 资源(Resource)，一个东西......如虚拟机
+ 资源组(Resource group)，文件夹，组织，访问控制
+ 资源提供程序(Resource provider)，VM—>Microsoft Compute，Storage—>Microsoft Store
+ 资源管理器模板(Resource Manager template)：脚本，建1000台VM

<br/>

好处：

+ 下方策略：只准部署资源在某地
+ 访问管理：权限会继承

<br/>

## 8.Azure Portal演示

...

## 9.创建一台Azure虚拟机

...


