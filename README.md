# Clash_for_Windows_HTA
## 使用VBScript编写的Clash控制面板<br>
服务器和规则稳定之后没必要使用那么重的工具,动辄上百M,HTA非常轻量化,记事本就可以编辑<br>
自用之余传下GitHub吧,万一有人需要呢<br>
![image](https://github.com/Amaury-GitHub/Clash_for_Windows_HTA/blob/main/README_IMG/IMG2.png)<br>
## 启动时<br>
自动读取Clash核心版本,然后循环读取Clash进程是否存在,系统代理是否打开,并给出提示,循环时间1s<br>
自动读取JMS的流量API信息并显示成柱状图,根据百分比不同变色,循环时间10m<br>
## 点击 打开 Clash 按钮<br>
按照以下步骤开启Clash<br>
1. 中断循环读取
2. 关闭 Clash
3. 关闭系统代理
4. 更新 Country.mmdb
5. 打开系统代理
6. 打开 Clash
7. taskkill调用的进程(cmd.exe,conhost.exe,reg.exe)
8. 开启循环读取
## 点击 关闭 Clash 按钮<br>
按照以下步骤关闭Clash<br>
1. 中断循环读取
2. 关闭 Clash
3. 关闭系统代理
4. taskkill调用的进程(cmd.exe,conhost.exe,reg.exe)
5. 开启循环读取
## 点击 Razord Dashboard 按钮<br>
访问 http://clash.razord.top/
## 点击 Yacd Dashboard 按钮<br>
访问 http://yacd.haishan.me/
## 点击 运行 EnableLoopback 按钮<br>
运行目录下的EnableLoopback.exe,让UWP应用可以正常上网
## 点击 更新 Clash 核心 按钮<br>
访问 https://github.com/Dreamacro/clash/releases/tag/premium<br>
自行判断是否需要更新吧
## 关闭<br>
没有任何操作,可以用完就退,没有遗留进程,只保留Clash自身<br>
## 修改提示<br>
![image](https://github.com/Amaury-GitHub/Clash_for_Windows_HTA/blob/main/README_IMG/IMG3.png)<br>
此处修改JMS的api地址<br>
<br>
![image](https://github.com/Amaury-GitHub/Clash_for_Windows_HTA/blob/main/README_IMG/IMG4.png)<br>
此处修改配置文件的名称<br>
## 广告<br>
目前在使用Just My Socks的服务,感觉还不错<br>
配置文件写成自动测速选择服务器之后都完全不用维护了,会自动换IP<br>
之前使用GCP的免费服务,三天两头IP被封,443端口直接阻塞<br>
有需要的小伙伴可以尝试一下<br>
[Just My Socks官网](https://justmysocks.net/members/aff.php?aff=15760)<br>
[Just My Socks5官网镜像,可直连](https://justmysocks5.net/members/aff.php?aff=15760)

