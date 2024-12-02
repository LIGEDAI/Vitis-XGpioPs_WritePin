# XGpioPs_WritePin函数的用法
## 1.1定义
函数原型为`void XGpioPs_WritePin(const XGpioPs *InstancePtr, u32 Pin, u32 Data)
{......}`作用是向对应的MIO接口（`u32 Pin`）写入相应的数据（`u32 Data`）
-`const XGpioPs *InstancePtr`为GPIO设备的驱动程序实例
-`u32 Pin`是对应的MIO接口
-`u32 Data`是要写入`u32 Pin`的数据
## 1.2实例
-`#define MIO_LED             0;`           //led连接到 MIO0
-`XGpioPs Gpio;`                //GPIO设备的驱动程序实例
-`XGpioPs_WritePin(&Gpio, MIO_LED, 0);`  //写入数据0
