# 数据源管理

> 此处以MySQL为例介绍数据源登记流程，具体步骤如下。

#### 步骤一：在系统头部导航选择【数据集成】然后左侧选择【数据源管理】，进入数据源登记页面。

![进入数据源登记页面](http://api.junereed.online:8100/file_center/file/1741167156382/dataSource1.png)

#### 步骤二：在【数据集成】-【数据源管理】页面，点击“登记数据源”按钮打开登记弹窗。

![打开登记弹窗](http://api.junereed.online:8100/file_center/file/1741167500418/dataSource2.png)

#### 步骤三：在弹窗中，需要填写项目组、数据源类型、数据源名称、库名称等内容，具体如下。

![登记弹窗信息](http://api.junereed.online:8100/file_center/file/1741167549898/dataSource3.png)

|配置项|内容|
|-|-|
|项目组|数据源的项目归属|
|数据源类型|MySQL,Oracle,MongoDB,DM,FTP,TxtFile,Hive,SqlServer,ClickHouse|
|数据源名称|用户自定义|
|库名称|用户自定义|
|IP|根据实际环境填写|
|Port|根据实际环境填写|
|用户名|根据实际环境填写|
|密码|根据实际环境填写|

#### 步骤四：对登记完成的数据源进行【测试连接】，测试通过后即可使用。

![测试连接](http://api.junereed.online:8100/file_center/file/1741167569289/dataSource4.png)

> 连接失败时，可以选择暂存此数据源。

![测试连接失败](http://api.junereed.online:8100/file_center/file/1741167581011/dataSource5.png)