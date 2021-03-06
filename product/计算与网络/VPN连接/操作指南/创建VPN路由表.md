>?当前VPN的路由表功能在灰度测试中，如有需要，请提交 [工单申请](https://console.cloud.tencent.com/workorder/category)。

## 前提条件
在配置路由表前，请确保已完成VPN网关、对端网关及VPN通道的配置。

## 操作步骤
1. 登录 [私有网络控制台](https://console.cloud.tencent.com/vpc/vpc?rid=1)。
2. 单击左导航栏中【VPN 连接】>【VPN 网关】。
3. 选择地域和私有网络，单击VPN网关ID进入详情页。
4. 单击【路由表】页签。
   ![](https://main.qcloudimg.com/raw/d261071d65c453ecf21d3980d1b3a8cd.png)
   5. 单击【新增路由】，并配置路由策略。
      ![](https://main.qcloudimg.com/raw/288637983594aa439f67c2ee00a7a12a.png)

| 配置项     | 说明                                                         |
| ---------- | ------------------------------------------------------------ |
| 目的端     | 填写要访问的对端网络的内网网段。                             |
| 下一跳类型 | VPN通道。<p>说明：如果是CCN型VPN网关，且VPN网关已关联至云联网实例时，还需要添加下一跳到【云联网】的路由策略。 |
| 下一跳     | 选择已创建的VPN通道。                                        |
| 权重       | 选择通道的权重值：<p><li>0：优先级高<li>100：优先级低        |
| 新增一行   | 可添加多条路由策略。                                         |
| 删除       | 可删除路由策略，最后一条不允许删除。                         |

6. 完成路由策略的配置后，单击【确定】。
7. 其他可执行操作。
    1. 启动、或禁用路由策略。
      ![](https://main.qcloudimg.com/raw/1d2b107d0c80bb1a0a291b6e68f7455f.png)
			
	2. 已禁用的路由策略支持删除。
		![](https://main.qcloudimg.com/raw/dfb2085c28e54597fd1d399091cd9826.png)
