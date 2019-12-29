# YDArk
免责声明: 这只是一个免费的辅助软件, 如果您使用本软件, 给您直接或者间接造成损失、损害, 本人概不负责. 从您使用本软件的一刻起, 将视为您已经接受了本免责声明.

// 本软件加了VMProtect壳, 可能有些杀毒软件会报毒...请大家放心使用, 这属于杀毒软件误报.

// 本软件免费, 但未获得作者书面授权, 禁止用于商业用途; 另外禁止本软件用于恶意用途(比如作为病毒木马的一部分、破解网吧收费系统等等).

// 本软件仅限于学习交流，如侵权请在24小时进行删除.

////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////

// 本驱动加了VMProtect壳, 不支持启用内核隔离.

// 驱动未进行驱动签名, 请自行对驱动文件签名或开启调试模式, (已签名但还加载驱动失败)请禁用Secure Boot或微软Ev签名或虚拟机使用.

// 欢迎大家在使用中若是发现BUG, 请及时联系反馈, 将会尽快修复, 如果大家有好的建议或意见, 也可以联系以下QQ或QQ群.
// QQ: 3269334485; QQ群: 399309204

////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////


// Tool screenshot
![image](https://github.com/ClownQq/YDArk/blob/master/screenshots/Process.png)
![image](https://github.com/ClownQq/YDArk/blob/master/screenshots/SystemNotify.png)

// Process
Threads                     View/Kill/Suspend/Resume
Modules                     View/Unload/Dump
Handles                     View/Close/Modify Granted Access
Windows                     View/Show/Hide/Maximized/Minimized/Enable/Disable/Close/Attack
Memorys                     View/Dump/Modify Protection
Timers                      View/Remove
HotKeys                     View/Remove

// Driver Module
Driver                      View/Unload/Dump/View Hide Driver

// Kernel
System Notify               View/Remove/Disassembling
Filter Driver               View/Remove/Disassembling
DPC Timer                   View/Remove/Disassembling
Hal Call                    View/Restore/Disassembling
Wdf Call                    View/Restore/Disassembling
File System                 View/Remove/Disassembling
Object Hijack               View/Restore (Disk)
Global Descriptor Table     View

// Kernel Hook
SSDT                        View/Restore/Disassembling
ShadowSSDT                  View/Restore/Disassembling
FSD                         View/Restore/Disassembling
Keyboard                    View/Restore/Disassembling
I8042prt                    View/Restore/Disassembling
Mouse                       View/Restore/Disassembling
Partmgr                     View/Restore/Disassembling
Disk                        View/Restore/Disassembling
Atapi                       View/Restore/Disassembling
Acpi                        View/Restore/Disassembling
Scsi                        View/Restore/Disassembling
Kernel Hook                 Scan/Restore/Disassembling
Object Type                 View/Restore/Disassembling
Interrupt Descriptor Table  View

// User Hook
Message Hook                View/Remove
User Hook                   Scan/Restore
Kernel Hook Table           Scan/Restore

// Net Work
Port                        View/Remove
Tcpip                       View/Restore/Disassembling
Nsiproxy                    View/Restore/Disassembling
Tdx                         View/Restore/Disassembling
Wfp WfpFilter               View/Remove
Wfp Callout                 View
Ndis                        View
IE Plugin                   View/Remove
IE Shell                    View/Remove
SPI                         View/Repair
Hosts                       View/Edit

// Registry
Create/Enumerate/Delete/Rename/Export/View Watch

// File
Create/Enumerate/Delete/Rename/View Lock/View File Pending/Delay Delete/Copy To/Copy In/Drag In

// Startup Info
Startup                     View/Remove
Services                    View/Start/Stop/Pause/Resume/Restart/Delete
Schedule Task               View/Disable/Enable/Delete

// Monitor
Create Exit Process/Create Thread/Load Image/Load Driver/Remote Thread Injection

// About


////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////


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

1.0.0.17:
1.新增支持7600
2.新增网络 IE插件/右键菜单/SPI/Host

1.0.0.18:
1.新增系统杂项Tab
2.修复扫描内核钩子不显示BUG