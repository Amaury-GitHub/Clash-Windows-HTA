# Clash_for_Windows_HTA
## 使用VBScript编写的Clash控制面板<br>
服务器和规则稳定之后没必要使用那么重的工具,动辄上百M,HTA非常轻量化,记事本就可以编辑<br>
自用之余传下GitHub吧,万一有人需要呢<br>
![image](https://github.com/Amaury-GitHub/Clash_for_Windows_HTA/blob/main/README_IMG/IMG1.png)<br>
## 启动时<br>
启动步骤<br>
1. 调整窗口尺寸
2. 调整窗口位置
3. 启动RBTray,实现右键最小化按钮缩到托盘区,(实在不知道如何使用程序实现,调用外部程序)
4. 获取Clash核心的版本
5. 获取Clash与系统代理是否开启
6. 读取JMS的流量API信息
7. 建立读状态的循环,循环时间1m
8. 建立读流量的循环,循环时间10m
## 关闭时<br>
清除所有调用的进程,保留Clash核心<br>
## 点击 打开 Clash 按钮<br>
开启Clash步骤<br>
1. 中断循环读取
2. 关闭 Clash
3. 关闭系统代理
4. 更新 Country.mmdb
5. 打开系统代理
6. 打开 Clash
7. 清除调用的进程
8. 开启循环读取
## 点击 关闭 Clash 按钮<br>
关闭Clash步骤<br>
1. 中断循环读取
2. 关闭 Clash
3. 关闭系统代理
4. 清除调用的进程
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
## 修改提示<br>
![image](https://github.com/Amaury-GitHub/Clash_for_Windows_HTA/blob/main/README_IMG/IMG2.png)<br>
## 广告<br>
目前在使用Just My Socks的服务,感觉还不错<br>
配置文件写成自动测速选择服务器之后都完全不用维护了,会自动换IP<br>
之前使用GCP的免费服务,三天两头IP被封,443端口直接阻塞<br>
有需要的小伙伴可以尝试一下<br>
[Just My Socks官网](https://justmysocks.net/members/aff.php?aff=15760)<br>
[Just My Socks5官网镜像,可直连](https://justmysocks5.net/members/aff.php?aff=15760)

