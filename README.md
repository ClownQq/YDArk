# YDArk
免责声明: 这只是一个免费的辅助软件, 如果您使用本软件, 给您直接或者间接造成损失、损害, 本人概不负责. 从您使用本软件的一刻起, 将视为您已经接受了本免责声明.

// 本软件加了VMProtect壳, 可能有些杀毒软件会报毒...请大家放心使用, 这属于杀毒软件误报.

// 本软件免费, 但未获得作者书面授权, 禁止用于商业用途; 另外禁止本软件用于恶意用途(比如作为病毒木马的一部分、破解网吧收费系统等等).

// 本软件仅限于学习交流，如侵权请在24小时进行删除.

////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////

// 本驱动加了VMProtect壳, 不支持启用内核隔离.

// 驱动未进行驱动签名, 请自行对驱动文件签名或开启测试模式, (已签名但还加载驱动失败)请禁用Secure Boot或微软Ev签名或虚拟机使用.

// 欢迎大家在使用中若是发现BUG, 请及时联系反馈, 将会尽快修复, 如果大家有好的建议或意见, 也可以联系以下QQ或QQ群.
// QQ: 3269334485; QQ群: 399309204

////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////

工具截图
![image](https://github.com/ClownQq/YDArk/blob/master/screenshots/Process.png)
![image](https://github.com/ClownQq/YDArk/blob/master/screenshots/SystemNotify.png)

已实现的功能:
01.支持F5刷新
// 进程
02.进程(Del键普通杀进程)/模块/模块/线程/句柄(F2编辑句柄权限)/窗口/内存/定时器/热键

// 驱动模块
03.驱动模块查看

// 内核
04.查看/移除系统回调
05.查看/移除过滤驱动
06.查看/移除DPC定时器
07.查看/恢复Hal回调
08.查看/恢复Wdf回调
09.查看/移除文件系统(MiniFilter/文件系统/SFilter/ClassInitData/Npfs/Msfs/UsbPort)
10.查看Disk对象劫持
11.查看全局描述符表

// 内核钩子
12.SSDT/ShadowSSDT/FSD/键盘/I8042Prt/鼠标/Partmgr/Disk/Atapi/Acpi/Scsi检测和恢复Hook和InlineHook
13.扫描/恢复内核钩子
14.查看/恢复Object钩子
15.查看中断描述符表

// 应用层钩子
16.查看/移除消息钩子
17.查看/恢复内核回调表

// 网络
18.查看/移除网络端口
19.Tcpip/Nsiproxy/Tdx检测和恢复Hook和InlineHook
20.查看/移除WfpFilter
21.查看WfpCallout函数
22.查看Ndis函数

// 注册表
23.枚举注册表/删除/新建/重命名注册表键(KEY)和注册表值(VALUE)/监控修改回调

// 文件
24.枚举文件/新建/解锁/删除/重启删除/重启替换/重命名/拷入拷出/拖入文件列表框

// 启动项
25.枚举/删除/修复启动项
26.枚举/启动/停止/暂停/恢复/重启服务
27.枚举/禁用/启用/删除任务计划

// 监控
28.监控进程/驱动加载/远线程注入

1.0.0.6:
1.新增枚举/恢复Disk对象劫持

1.0.0.7:
1.优化枚举驱动模块
2.修复17763-18362系统设置注册表值蓝屏
3.修复界面最小化一段时间控件消失, 支持界面窗口最大化
4.新增枚举/删除/修复启动项
5.修复进程窗口功能

1.0.0.8:
1.修复恢复SSDT/SSSDT导致蓝屏
2.新增恢复内核InlineHook

1.0.0.9:
1.新增检测更新
2.新增对进程svchost.exe显示服务模块
3.枚举枚举/启动/停止/暂停/恢复/重启服务
4.新增枚举/禁用/启用/删除任务计划

1.0.0.10:
1.修复枚举线程模块BUG
2.优化检测更新
3.新增枚举/移除注册表监控修改回调(注册表窗口右键TREE控件)

1.0.0.11:
1.修复Win7-Win8系统回调中Thread类型显示为Process类型
2.新增Ctrl+C复制一行
3.新增监控进程/驱动加载/远线程注入(Stack加载符号比较慢, 取消加载符号将symsrv.dll重命名其他文件名即可)

1.0.0.12:
1.新增支持Windows10 18363
2.新增监控创建退出线程/模块加载
3.修复若干BUG

1.0.0.13:
1.新增支持繁体中文和英文

1.0.0.14:
1.新增进程创建Dump
2.新增扫描Pte Hook

1.0.0.15:
1.修复导致文件路径异常BUG
2.新增注册表导出.reg文件
3.新增应用层扫描Inline钩子

1.0.0.16:
1.优化枚举驱动模块
2.优化扫描内核钩子
3.新增应用层扫描EAT钩子
4.新增检测Infinity钩子(SSDT Tab弹框)