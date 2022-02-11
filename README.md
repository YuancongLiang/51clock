# 51clock
是一个摆烂的项目，只是摆着当存档，具体内容可以见知乎
https://zhuanlan.zhihu.com/p/465914774
目前存在的BUG：
1、温湿度数据不能够实时变化，需要切换模式0.8秒以上返回主菜单界面才可刷新，BUG初步确定在RH函数中，不可频繁调用该函数，一般需要间隔0.8s后再重新使用才可正常刷新温湿度
2、蓝牙功能无法使用，初步推测是串口初始化不成功
3、部分按键同时按下时会卡死

AD工程中的注意事项：
1、由于3d打印件的空间限制，排针排母统一使用了弯排针
2、TP5400及其配套元件可以不进行焊接，采用具有充放电口的电池
3、电池需要一个电源转接板或定制插口，能够保证最终直接或通过杜邦线间接插在J4的两根电源排针上（VCC,GND）
4、J4初始为程序烧录口
5、晶振频率为22.1184MHz
6、J1,J2,J4,J5均为弯排针，而并非3d预览图所示的排母或直排针

current bugs:
1.Temperature and humidity data cannot be changed in real time.To solve this problem,you need to switch to another mode holding for at least 0.8 seconds.The bug is located in the function RH.This function cannot be called frequently.You can normally refresh temperature and humidity data if you call function RH with an interval.
2.Bluetooth function does not work.The reason may be the serial port initialization failed.
3.Some keys get stuck when pressed at the same time.

attentions in the AD project:
1.Due to space constraints of 3d prints,pins unified use curved pins.
2.TP5400 and its kit are no welding required.
3.Battery requires a power adapter board or custom socket.You need to ensure that the battery can be connected to J4(VCC,GND)
4.J4 is the program burning port at first.
5.The crystal frequency is 22.1184MHz.
6.J1,J2,J4,J5 are curved pins,instead of the 3d preview.
