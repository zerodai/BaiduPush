#Welcome to use Baidu Push Service

> **云推送**（Push）是百度开放云向开发者提供的消息推送服务；通过利用云端与客户端之间建立稳定、可靠的长连接来为开发者提供向客户端应用推送实时消息服务。 <br />


百度云推送服务支持三种推送类型：***通知、消息及富媒体**；支持向所有用户、根据标签分类向特定用户群体、向单个用户和基于地理位置推送消息；支持更多自定义功能（如自定义内容、后续行为、样式模板等）；提供用户信息及通知消息统计信息，方便开发者进行后续开发及运营。

####Official Site: [http://developer.baidu.com/cloud/push](http://developer.baidu.com/cloud/push)

####Report Issue&Bug: [https://github.com/BaiduPush/BaiduPush/issues](https://github.com/BaiduPush/BaiduPush/issues)

####SDK & API: 

* #####[客户端SDK](http://developer.baidu.com/wiki/index.php?title=docs/cplat/push/sdk/clientsdk)

* #####[服务端SDK](http://developer.baidu.com/wiki/index.php?title=docs/cplat/push/sdk/serversdk)

* ####[Http API](http://developer.baidu.com/wiki/index.php?title=docs/cplat/push/api)

----------


## 开发者支持途径

	百度hi官方技术讨论群：1405944

	QQ群1：348807820（可加）

	QQ群2：242190646（已满）

	QQ群3：324533810（已满)


##云推送服务功能

云推送服务主要提供以下功能：

###推送通知
向移动端推送展现在系统通知栏的通知消息。

###推送消息
以透传的方式将开发者自定义的内容发送到客户端。开发者可以预先在客户端设定好规范，进行消息定制化。

###推送富媒体
推送图片、视频、音频、网址等形式的富媒体信息。

###基于地理位置的推送（或“LBS推送”）<font color="red">New</font>

有了LBS推送，开发者可以根据用户所在的地理位置，有针对性的推送消息，更好的契合用户的信息消费需求。比如，向全北京的用户推送一条暴雨预警通知，向上海的用户推送地铁故障信息，等。

LBS推送是在现有的三种推送模式上的增强，无论是推送通知，透传消息，还是富媒体消息，都可以加上LBS定向这个选项。目前支持省、直辖市、市、区级别的行政区域，后续会增加商圈及自定义地理围栏等功能（仅限Android平台）。

	了解详情：请下载最新的Android SDK了解客户端的设置。请参考管理控制台说明，了解如何推送LBS消息。


说明：目前LBS推送功能还处于邀请测试阶段，有意向的开发者可以通过 [dev_support@baidu.com](email://dev_support@baidu.com) 邮件与我们联系申请加入测试。请在标题中注明 “***申请加入LBS推送测试***” 字样，邮件内容请提供您的账号、应用名称、应用id以及简单说明一下应用场景，便于我们筛选和处理您的邮件。您也可以通过QQ群(242190646)和百度HI群(1405944)与我们获得联系。

###信息统计
提供推送信息和用户行为的统计。


###管理控制台
将推送功能可视化，可以直接通过控制台针对特定的用户群，完成通知、消息、富媒体的推送。详细信息，请参考《管理控制台》。


##云推送服务特点

云推送服务具有以下特点：

1. 增强用户粘性

通过云和端之间建立的长连接，可以实时的推送消息到达用户端。保持与用户的沟通，大大提升用户活跃度和留存率。

2. 节约成本

在省电省流量方面远超行业水平，基础的消息推送服务永久免费，大大节省开发者推送的成本。

3. 稳定安全的推送

强大的分布式集群长期为百度各大产品线提供推送服务，保证消息推送服务的稳定、可靠。

##重要说明

* ***目前单条消息支持最大 4K 的消息推送功能，兼容文本和二进制消息格式。***

	如果应用有超过 4K 数据推送的需求，则应用可以在推送的消息里携带资源的 URL 地址，客户端在接收到消息后，主动对这个超过 4K 的数据发起另外一次请求。

* 云推送服务提供消息暂存、转发和推送的功能，客户端无需保持在线状态及进行反复轮询，消息不会丢失。

* 云推送服务支持推送给一个人、一群人和所有人，详情可参考《REST API》。

* 单一终端多个应用共享一个服务进程和一条 TCP 长连接，从而有效降低手机的耗电量和数据流量。

* 目前接入和使用云推送服务都需要成为百度开发者；而其应用的账户登录系统则可使用“百度账户登录”，也可使用“无账户登录”。