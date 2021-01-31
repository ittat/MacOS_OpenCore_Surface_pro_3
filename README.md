# MacOS 10.14 for Surface pro 3 (Intel i5) 

## What's work? 
- 原生声音 (AppleHDA + AppALC + dsdt)
- GPU (dsdt + hot patch)
   关机保持亮度
   快捷键调节亮度 Fn + Del  Fn + back （4代键盘）
- BatteryManagement (dsdt) 
    实现双电池 
    状态栏电量更新误差在2%以内 
- 机身按键 (ACPIKeyboard.kext + dsdt) (偶尔可以正常使用) 
- CPU 
    原生dsdt已经实现12级变频 
- 触屏 Touchscreen 
    开机情况下 kextload VoodooI2C 1.0.4 可以实现触屏 
- 相机 

## What's not work? 
- 触控板无法驱动（4代键盘）
    I need your help!!!
- WIFI Bluetooth
    