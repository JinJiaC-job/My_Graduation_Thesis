1、巴特沃斯低通滤波器与零相位数字滤波

低通滤波器：其归一化截止频率（Wn）是指信号的截止频率除以采样频率的一半（Nyquist频率）。

```c
Wn = Fc / (Fs/2)
```

其中：

- `Wn` 是归一化截止频率。
- `Fc` 是滤波器的实际截止频率。
- `Fs` 是信号的采样频率。

外骨骼机械臂运行时间runtime = 20s；

滤波器阶数n = 5；（默认）

采样频率ws = 20Hz；（控制程序修改）

截止频率wc = 3；（默认）

采样点数pnt = 400；（控制程序修改）



2、采用中值滤波和卡尔曼滤波进一步去除信号毛刺