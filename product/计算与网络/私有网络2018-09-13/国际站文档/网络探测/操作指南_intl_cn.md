## 创建网络探测
1. 登录 [腾讯云控制台](https://console.cloud.tencent.com/)，选择 【云产品】>【私有网络】>【网络探测】。
![新建1](https://main.qcloudimg.com/raw/8dec3a9a9a1e5a64e7f77a7f0ec562a7.png)

2. 单击左上角【新建】按钮创建探测实例，需在弹出框中依次输入或确定以下参数：
 - 名称：网络探测名称
 - 所属网络及子网：系统自动选择子网内两个闲置的内网 IP 作为网络探测的源地址；
 - 探测目的 IP：网络探测最大支持两个目的 IP 地址，请为网络探测的目的主机开通 ICMP 防火墙策略；
 - 下一跳：指网络探测流量的下一跳路由，配置下一跳对象后，在子网所关联的路由表中自动添加对应 32 位路由。
 
3. 选择结束后单击【创建】按钮，即可完成探测实例的创建。
![新增3](https://main.qcloudimg.com/raw/42b8ca8c8e71dafe1095c510908debde.png)
>**注意：**
> 1. 建议您在创建网络探测前，验证探测结果，如果连接失败，请检查子网路由是否配置正确 或 目的探测对象是否放通了 PING 防火墙等。
> 2. 网络探测路由为系统路由，不可修改。
> 3. 在子网切换路由时，原子网关联路由表将删除此系统路由，子网新关联的路由表将添加此系统路由。

## 查看网络探测时延和丢包率
1. 登录 [腾讯云控制台](https://console.cloud.tencent.com/)，选择 【云产品】>【私有网络】>【网络探测】。

2. 点击网络探测实例的监控图标即可查看网络探测时延及丢包率。
![监控](https://main.qcloudimg.com/raw/ac6db68116aa7a97604b486f110a5033.png)

## 修改网络探测
1. 登录 [腾讯云控制台](https://console.cloud.tencent.com/)，选择 【云产品】>【私有网络】>【网络探测】。

2. 单击网络探测实例的 【编辑】 按钮，即可修改网络探测相关参数。
![](https://main.qcloudimg.com/raw/c1df7281db38ab378414da70a2cfd5ef.png)

## 删除网络探测
1.登录 [腾讯云控制台](https://console.cloud.tencent.com/)，选择 【云产品】>【私有网络】>【网络探测】。

2.选择需要删除的网络探测实例，单击 【删除】>【确认】 即可完成删除。
![删除](https://main.qcloudimg.com/raw/837d819b09af935ad21072c5ccfa15d4.png)
>**注意：**
>删除网络探测实例，其相关路由将一并删除。
