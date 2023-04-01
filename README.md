# Clash_for_Windows_HTA
## 使用VBScript编写的Clash控制面板<br>
一个工控人的摸鱼作品,欢迎指正<br>
Clash for Windows的软件都太大了,动辄上百M,很多功能我也不需要<br>
HTA非常轻量化,记事本就可以编辑,可以按照自己的需求进行打造<br>
自用之余传下GitHub吧,万一有人需要呢<br>
![image](https://github.com/Amaury-GitHub/Clash_for_Windows_HTA/blob/main/README_IMG/IMG1.png)<br>
## 启动时<br>
启动步骤<br>
1. 调整窗口尺寸
2. 调整窗口位置
3. 启动RBTray,实现右键最小化按钮缩到托盘区,(实在不知道如何使用程序实现,调用外部程序)
4. 读取 Clash 版本
5. 获取 Clash & 系统代理 是否开启
7. 建立读状态的循环,循环时间 10s
## 关闭时<br>
清除所有调用的进程,保留Clash核心<br>
## 点击 打开 Clash 按钮<br>
开启Clash步骤<br>
1. 中断循环读取
2. 关闭 Clash
3. 读取 Clash 版本
4. 打开 Clash
5. 打开系统代理
6. 修改dns指向127.0.0.1,::1
7. 清除调用的进程
8. 开启循环读取
## 点击 关闭 Clash 按钮<br>
关闭Clash步骤<br>
1. 中断循环读取
2. 关闭 Clash
3. 关闭系统代理
4. 恢复dns的设置
5. 清除调用的进程
6. 开启循环读取
## 点击 Razord Dashboard 按钮<br>
yaml需要配置ui的路径,external-ui: /dashboard<br>
访问 http://127.0.0.1:9090/ui/razord
## 点击 Yacd Dashboard 按钮<br>
yaml需要配置ui的路径,external-ui: /dashboard<br>
访问 http://127.0.0.1:9090/ui/yacd
## 点击 运行 EnableLoopback 按钮<br>
运行目录下的EnableLoopback.exe,让UWP应用可以正常上网
## 点击 Github Clash 按钮<br>
访问 https://github.com/Dreamacro/clash/releases/tag/premium<br>
两个版本不一致可以去更新,自动更新就算了,感觉超出能力范畴了
## 修改提示<br>
![image](https://github.com/Amaury-GitHub/Clash_for_Windows_HTA/blob/main/README_IMG/IMG2.png)<br>
