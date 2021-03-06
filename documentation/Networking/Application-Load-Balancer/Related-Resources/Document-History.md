# 文档历史记录


本文档介绍应用负载均衡产品文档的重要更新历史，包括新增产品的重大特性和按照用户的反馈进行内容的更新等。

|发布日期|特性|描述|
|-|-|-|
|2020年2月|开放OpenAPI和SDK|应用负载均衡OpenAPI和SDK对外开放|
|2020年1月|应用负载均衡列表页支持搜索|应用负载均衡列表页支持基于ID、名称等搜索|
|2020年1月|修改计费类型|应用负载均衡计费类型从按配置改为按用量，但仍暂时免费|
|2019年12月|对接云安全-SSL数字证书|应用负载均衡使用的SSL证书都迁移至云安全-SSL数字证书，应用负载均衡-证书模块不再提供SSL证书管理功能，由云安全-SSL数字证书进行统一管理|
|2019年8月|支持转发规则组|支持基于URL请求的主机名和路径将流量转发给不同的后端服务处理|
|2019年7月|七层访问日志|应用负载均衡支持通过日志服务收集七层访问日志|
|2019年3月|功能迭代|支持删除保护、虚拟服务器组添加实例时支持按指定字段搜索|
|2018年11月|支持TLS协议|应用负载均衡支持监听TLS协议|
|2018年7月|支持高可用组|支持通过高可用组提供后端服务|
|2018年7月|支持原生容器|应用负载均衡支持绑定容器为后端服务进行流量分发|
|2018年7月|架构优化|分拆监听规则为监听器与后端服务|
|2018年2月|支持绑定安全组|应用负载均衡支持绑定安全组功能|
|2017年11月|支持四层源IP透传|四层协议支持proxy protocol|
|2017年9月|计费模式调整|计费模式修改为后付费|
|2017年9月|支持HTTPS协议| 应用负载均衡支持监听HTTPS协议 |
|2017年1月|公测|应用负载均衡公测版上线|


## 相关参考

- [产品概述](../Introduction/Product-Overview.md)
- [核心概念](../Introduction/Core-Concepts.md)
- [产品优势](../Introduction/Benefits.md)
- [产品功能](../Introduction/Features.md)
- [价格总览](../Pricing/Price-Overview.md)
- [计费规则](../Pricing/Billing-Rules.md)
- [创建负载均衡实例](../Getting-Started/Create-Instance.md)
- [创建高可用组](../Getting-Started/Create-AvailabilityGroup.md)
- [创建虚拟服务器组](../Operation-Guide/TargetGroup-Management.md)
- [配置侦听策略](../Operation-Guide/Listener-Management.md)
- [管理后端服务与查看服务实例健康状态](../Operation-Guide/Backend-Management.md)
- [查看监控信息](../Operation-Guide/Monitoring.md)
