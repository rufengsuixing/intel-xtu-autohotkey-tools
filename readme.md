##原理
提取了最后一个版本允许进行命令行控制xtu的可执行文件，通过autohotkey监听系统电源事件，进行休眠后唤醒的自动应用offset电压。
##缺点
缺点来源于xtu，使用命令行读取到的offset电压可能并没有应用到设备，所以本软件只能进行电压设置，读取的offset值没有意义。xtu也有同样offset应用是切换开关或者无效这个问题，于是应用两次不同电压解决这个问题。
##用法
安装autohotkey，和xtu（官网最新即可）<br>
复制本项目所有文件<br>
修改cpuvoltageoffset.bat 和 apply_ome.ahk 101和107行 电压offset设置（两行电压要求不同，应用的是最后一行）<br>
双击ahk，给管理员权限，电脑休眠后唤醒时会自动应用offset设置