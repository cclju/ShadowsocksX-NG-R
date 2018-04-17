Remove due to regulation

ShadowSocks-NG中使用白名单模式，只针对用户指定的规则生效，只需要按照如下步骤进行设置

 

{ 1. 在自动模式下配置并成功使用 }

配置正确服务器信息，同时在"Proxy Auto Configure Mode"可以正常访问Google.com 和Youtube.com即可

 

{ 2. 启用白名单模式 }

默认ShadowSocks-NG并没有白名单模式，在自动模式下访问规则为PAC＋用户自定义规则，如果能够使PAC失效(为空)，剩下用户自定义即为白名单模式，操作如下

A. 打开 Finder->Go->Go To Folder... (Command+Shift+G)

B. 输入 ~/.ShadowsocksX-NG/

C. 打开后看到3个文件 gfwlist.js, gfwlist.txt, user-rule.txt, 打开gfwlist.txt清空后保存

D. 通过程序菜单使用"Edit User Rules For PAC..." 随意添加或者删除一条url，保存后规则会自动更新规则，不要运行"Update PAC from GFW list"就会一直为白名单模式

 

{ ref. }

https://github.com/shadowsocks/ShadowsocksX-NG/issues/496
