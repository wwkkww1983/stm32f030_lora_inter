# stm32f030_lora_inter

改版本改动比较多。
相对于上一个版本stm32f030_lora,本版本中在电机启动控制超时定时器时，将原来的tim6更改为rtc，
rtc唤醒目前只能支持整秒唤醒，短时间（1s以内）的延时还是使用tim6进行控制。
目前能够实现控制指令的执行，在电机启动后也能够对接收到的新命令作出重复判断。

