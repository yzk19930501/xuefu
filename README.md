# 基于pyalgotrade的回测框架
>- Too Long to refresh.很久没有更新。开放共享，共同进步。
>- 技术问题需要讨论的请直接加群QQ群： 300349971，策略研究实践不吝赐教、讨论或需要技术支持的请加QQ：657959571
>- 建议学习pyalotrade回测的用户先运行完所有demo后再进行策略编写，demo基本包含编写策略的绝大多数坑了
>- 快速开始请阅读<QuickStart.md>
## 新上传文件功能 ##
- 单独封装上期所ctp接口，不同于vnpy和海风版，将原版ctp字段和方法全部移植到python版，只需将方法和字段首字母改成小写即可，最大限度“原汁原味”.
  cmake_ctp文件夹为独立模块，相关编译脚本已写好，可自己编译最新版ctp。*目前已有针对python2.7，python3.X，含win32,win64,linux的各类编译版本*
- 对响应速度有较高要求的人员可在ctpdemo基础上进行二次开发，不敏感的见ctpTickDemo。
- 添加docker环境配置，docker文件夹为独立的模块，作者为洒家同学liqi.
- 支持tushare实时行情进行模拟或实盘测试，且支持预先加载一部分历史数据，然后再读取实时行情，方便预计算各指标
- 准备测试多因子，开发中
