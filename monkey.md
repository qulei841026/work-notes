Monkey脚本

##代码
type= raw events
count= 1
speed= 1.0   
start data >>   
LaunchActivity(com.le.hsv, com.le.hsv.demo.MainActivity)

DispatchPress(KEYCODE_DPAD_LEFT)
UserWait(50)
DispatchPress(KEYCODE_DPAD_CENTER)
UserWait(50)
DispatchPress(KEYCODE_DPAD_CENTER)
UserWait(50)

##命令
安装
adb push monkey.mks /data/local/tmp/<br>
执行<br>
adb shell monkey -f /data/local/tmp/monkey.mks -v -v 1 //-v信息，1次数<br>
关闭<br>
adb shell top | grep "mokey"<br>
adb shell kill -9 "24971"

