
# ACPI-S0-S5&G0-G3

S0(G0): 正常工作状态: 计算机正式工作，CPU、DIM,PCH 、硬盘均开始工作。

G1 （睡眠）状态：里面包括S1-S4四个状态，睡眠的模式不同对应的功耗也是不同的。具体如下：
  - S1: 最耗电的睡眠模式。CPU所有寄存器刷新，并且CPU停止执行指令。但是CPU、DIM电源没有掉。
  - S2: CPU电关闭，通常不用。
  - S3：在任务挂到内存中，当唤醒后（S3->S0）状态，用户刚刚的工作可以恢复到睡眠前的相同状态。但是在这个状态下如果突然AC掉电，这样用户此前处理的数据将会丢失。
  - S4：在任务挂到硬盘上，当唤醒后（S4->S0）状态，用户刚刚的工作可以恢复到睡眠前的相同状态。但是在这个状态下如果突然AC掉电，这样用户此前处理的数据将不会丢失，再次重启后依然能够恢复进入睡眠模式前的工作状态。

S5: soft off ，软件关机——包括POWER BUTTON或上位机触发（用户界面）。

G3 状态是：AC掉电，主板上只有RTC电源。
