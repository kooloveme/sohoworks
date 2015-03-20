

这个页面描述 marsx 一个delphi ria  应用程序开发平台

### 什么marsx ###

marsx 是一个delphi ria 应用程序开发平台。delphi 说明了其开发语言，ria 表示marsx 是基于internet 的富客户端应用。 开发平台是指用户可以直接使用marsx开发应用程序。marsx 在开发中借鉴了许多微软axapta 概念.  marsx有以下内容组成

  * 桌面客户端和一个ActiveX ie客户端，包括aot 二次开发环境
  * 应用程序服务器
  * 配置实用程序等扩展工具

marsx 支持pascal/vb/javascript为客户化开发语言，基础平台使用delphi开发。 利用db存储aot 元数据，目标数据库使用sql server 2000或以上版本

marsx 的最大特点是程序即开发平台，上层应用代码开源。好处是程序将是永远发展，不断积累，而且不受限于开发商.有了这样的应用，可以想象技术支持部门能快速的响应实际的需求，方便的修改或在原有功能上增加新功能。这同一般闭源，无定制能力的应用的发展前景将会有很大的不同

主要特点

  * 纯32位本机windows 应用，无程序慢慢的感觉，无较大资源占用问题
  * 使用分布式方式访问数据库 支持tcp/http连接，支持bin/json/xml消息格式
  * 拥有一个集中的元数据库。抽象了编程元素，像table,form,class,job,query,report,base enum,lookup s等，这些均保存在一个叫aot的地方，目前使用数据库保存
  * 带一个编译器，客户化环境语言目前同时支持pascal,basic,javascript（未来将支持java),代码编译后存在在数据库，登录时自动下载，更新后自动编译
  * 提供一个广泛的控件集（如网格，文本框，数字，日期等）和大量的函数和基础对象，如formrun/reportrun等
  * 用户通常只需退出应用程序重新进入就能反映变化,程序更新时无需更新客户端
  * 可使用内置的aot 进行定制开发
  * 开发流程简单，单表，master/detail之类的均在几分钟完成，通常步骤就是
    1. 创建table,目前没有数据库同步功能,需要手动创建数据库表(todo)
    1. 创建窗体form，增加数据源datasource，将表名tableName指定为创建的table，创建控件，指定datasource和field
    1. 创建menuitem ,指向刚创建的窗体
    1. 创建菜单-指向 刚创建的menuitem
    1. 重新启动或刷新导航

  * 强大的excel报表支持
  * 工作流支持，内置设计器
  * 支持多国语言
  * 基于安全键的安全模式 ，支持记录级安全
  * 内置单元测试框架 (todo )




### marsx 设计哲学 ###

marsx 借鉴了axapta 的设计哲学

  * Modify the complete system by changing ONE property 通过属性设置改变应用系统
  * Move your code away from the interface 代码应该尽量远离用户接口，即尽量少在窗体中写代码
  * Design the structure of your interface, not the layout 用户界面通过描述其结构展现，无需“画界面”

### 规范 ###

[规范](Specifications.md)

### 模式 ###

[模式](pattern.md)



### 更新日志 ###

[changelog](changelog.md)

### 开发指南 ###
[开发指南](guide.md)

[函数列表](global_function.md)

[内置控件列表](controls.md)

[服务器端脚本](server_scripts.md)

[陷阱](Trap.md)

[faq](faq.md)

### 已知问题 ###
[issue](issue.md)




### 案例 ###


[case\_earrow](case_earrow.md)