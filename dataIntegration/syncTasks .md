# 数据同步

## 创建数据同步任务

> 此处以MySQL至Hive为例介绍同步任务创建流程，具体步骤如下。

#### 步骤一：在系统头部导航选择【数据集成】然后左侧选择【数据同步】，进入数据同步页面。

![进入数据同步页面](http://api.junereed.online:8100/file_center/file/1742176199505/syncTasks1.png)

#### 步骤二：在【数据集成】-【数据同步】页面，点击“新建传输任务”按钮打开任务弹窗。

![进入数据同步页面](http://api.junereed.online:8100/file_center/file/1742176529760/syncTasks2.png)

#### 步骤三：在任务弹窗中，配置【基本信息】，根据实际情况配置任务名称、项目组等。

![配置基本信息](http://api.junereed.online:8100/file_center/file/1742177564268/syncTasks3.png)

|配置项|内容|
|-|-|
|项目组|数据同步任务的项目归属|
|任务名称|用户自定义|
|描述|用户自定义|

#### 步骤四：配置数据来源和数据去向。

- 数据来源

![数据来源](http://api.junereed.online:8100/file_center/file/1742178089159/syncTasks4.png)

 |配置项|内容|
 |-|-|
 |类型|MySQL,Oracle,MongoDB,DM,FTP,Hive,SqlServer,ClickHouse|
 |数据源|用户自定义|
 |库|用户自定义|
 |表|用户自定义|
 |where|参考对应数据源SQL语法，填写where条件后面的内容（不包括where条件）|

- 数据去向

![数据去向](http://api.junereed.online:8100/file_center/file/1742178539765/syncTasks5.png)

 |配置项|内容|
 |-|-|
 |类型|MySQL,Oracle,MongoDB,DM,Hive,SqlServer,ClickHouse|
 |数据源|用户自定义|
 |库|用户自定义|
 |表|用户自定义|
 |分区|动态分区的值可以为来源字段的值或来源数据库的系统函数| 
 | writeMode|写入前数据清理处理模式| 
 | fieldDelimiter|写入时的字段分隔符,需要用户保证与创建的Hive表的字段分隔符一致| 

#### 步骤五：配置字段映射。

![字段映射](http://api.junereed.online:8100/file_center/file/1742179313620/syncTasks6.png)

> 此处系统会默认进行【同名映射】，如果发现映射有问题，也可以通过【同行映射】或者手动调节。

#### 步骤六：任务保存，点击保存按钮即可完成该任务的保存。

![任务保存](http://api.junereed.online:8100/file_center/file/1742179922375/syncTasks7.png)

## 试运行

#### 在数据传输任务记录中点击右侧运行按钮，可试运行该数据传输任务。

![运行任务](http://api.junereed.online:8100/file_center/file/1742193792211/syncTasks8.png)

#### 在数据传输任务记录中点击右侧运行结果按钮，可查看运行结果历史记录，点击历史记录中右侧日志按钮可查看该运行记录的日志。

![运行结果](http://api.junereed.online:8100/file_center/file/1742194097159/syncTasks9.png)

![运行结果](http://api.junereed.online:8100/file_center/file/1742194273069/syncTasks10.png)

## 提交上线

#### 在数据传输任务记录中点击右侧提交上线按钮，可把该传输任务提交用于任务管理进行调度。

![提交上线](http://api.junereed.online:8100/file_center/file/1742196108333/syncTasks11.png)

#### 在线上数据传输任务记录中点击右侧引用详情按钮，可查看该传输任务的引用详情。

![引用详情](http://api.junereed.online:8100/file_center/file/1742196283659/syncTasks12.png)

![引用详情](http://api.junereed.online:8100/file_center/file/1742196301225/syncTasks13.png)
