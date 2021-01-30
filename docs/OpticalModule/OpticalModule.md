## **光模块 Optical Module**

###1. 种类

- 光发送模块 Transmitter
- 光接收模块 Receiver
- 光收发一体模块 Transceiver （光模块一般指Transceiver）
- 光转发模块 Transponder

### 2. 组成

- 光发射器件（TOSA，含激光器）
- 光接收器件（ROSA，含光探测器）
- 功能电路
- 光（电）接口

![img](https://pic2.zhimg.com/80/v2-1f9eee060e7747932ffeb3087895f135_720w.jpg)

###3. 封装

*区分光模块的最主要方式*

![img](https://pic3.zhimg.com/80/v2-bba888f90b5aa6a0f861ae06cedef91a_720w.jpg)

![img](https://pic2.zhimg.com/80/v2-93bd5d5a055eac36739734081a60fe65_720w.jpg)

####3.1 光通信的标准化组织

- IEEE
- ITU-T（国际电联）
- MSA，Multi Source Agreement 多源协议（多供应商规范）

####3.2 常见封装类型

#####3.2.1 GBIC（Giga Bitrate Interface Converter，千兆接口转换器）

- 2000年以前最流行的光模块封装，应用最广泛的千兆模块形态

![img](https://pic1.zhimg.com/80/v2-188e986912806a364887489963d02ca4_720w.jpg)

#####3.2.2 SFP（Small Form-factor Pluggable，小型可热插拔光模块）

- SFP的体积比GBIC模块减小一半，可在相同的面板上配置多出一倍以上的端口数量
- 功能上，SFP与GBIC差别不大，均支持热插拔
- SFP支持最大带宽为4Gbps

<img src="https://pic3.zhimg.com/80/v2-4d58a26e1536c7c41fd2cc502da5439e_720w.jpg" alt="img" style="zoom:50%;" />

#####3.2.3 XFP（10-Gigabit Small Form-factor Pluggable，万兆SFP）

- XFP采用一条XFI（10Gb串行接口）连接的全速单通道串行模块

![img](https://pic2.zhimg.com/80/v2-1c0cf3463484a84055e2b1dacd8228bd_720w.jpg)

#####3.2.4 SFP+

- SFP+和XFP均为10G光模块
- SFP+尺寸与SFP一致，比XFP更紧凑（缩小了约30%），功耗更小（减小了一些信号控制功能）

![img](https://pic1.zhimg.com/80/v2-e5b984fafe52ae1ecd77a1f5a89f8e28_720w.jpg)

<img src="https://pic2.zhimg.com/80/v2-df80881f0db2a9d717370fcefb9dc1a5_720w.jpg" alt="img" style="zoom:80%;" />

##### 3.2.5 SFP28

- 速率为25Gbps的SFP（40G和100G光模块的过渡方案）

<img src="https://pic3.zhimg.com/80/v2-d3bce465a39a1afd5519bcaf96361a76_720w.jpg" alt="img" style="zoom: 67%;" />

#####3.2.6 QSFP / QSFP+ / QSFP28 / QSFP28-DD（Quad Small Form-factor Pluggable，四通道SFP接口）

- QSFP根据速度分为：4x10G QSFP+；4x25G QSFP28；8x25G QSFP28-DD等

- QSFP-DD（Double Density，双倍密度），与QSFP方案兼容，可在原有的QSFP28模块再插入一个模块

- QSFP-DD每路采用25Gbps NRZ（200Gbps）或者50Gbps PAM4信号（**400Gbps**）

<img src="https://pic4.zhimg.com/80/v2-2fa30e8924f2bb371618a6ac57cef4af_720w.jpg" alt="img" style="zoom:67%;" />

#####3.2.7 CFP / CFP2 / CFP4 /CFP8（Centum gigabits Form Pluggable，密集波分光通信模块）

- 传输速率可达100-400Gbps
- CFP在SFP基础上设计，尺寸更大，支持100Gbps数据传输，可支持单个100G信号、一个或多个40G信号
- CFP、CFP2、CFP4的区别在于体积，CFP2体积是CFP的$\frac{1}{2}$，CFP4是CFP的$\frac{1}{4}$
- CFP8针对400G信号，尺寸与CFP2相当。支持25Gbps和50Gbps速率，通过16x25G或8x50G电接口实现**400Gbps**模块速率

![img](https://pic4.zhimg.com/80/v2-43886359940cfe48da34e2185b771d63_720w.jpg)

#####3.2.8 OSFP（Octal Small Form-factor Pluggable，八通道SFP接口）

- 8个电气通道实现**400Gbps**，尺寸略大于QSFP-DD，散热性能稍好

![img](https://pic4.zhimg.com/80/v2-d1bba1796bbec51be1283e62dbc57d13_720w.jpg)

###4. 400G光模块

*QSFP-DD、CFP8、OSFP*

![img](https://pic3.zhimg.com/80/v2-34d34a630a63f43a8f427a82d8ec160a_720w.jpg)

- 早期400G光模块：16路25Gbps NRZ的方式，CDFP或CFP8封装
  - 优点：25G NRZ技术成熟
  - 缺点：16路并行传输，功耗和体积较大，不适合数据中心的应用
- 目前400G光模块：光口侧使用8路53Gbps PAM4或4路106Gbps PAM4实现400G的信号传输；电口侧使用8路53Gbps PAM4电信号，OSFP或QSFP-DD封装
  - QSFP-DD尺寸更小，适合数据中心应用
  - OSFP尺寸稍大，适合电信应用
- 400Gbps光模块价格昂贵

### 5. 光模块的具体命名

*100G为例*

<img src="https://pic1.zhimg.com/80/v2-5acb32e4a3ca84f1850497da05d58e1c_720w.jpg" alt="img" style="zoom: 80%;" />

####5.1 MSA命名

- PSM4（Parallel Single Mode 4 lanes，并行单模四通道）
- CWDM4（Coarse WDM 4 lanes，四通道粗波分复用）

####5.2 IEEE 802.3命名

<img src="https://pic2.zhimg.com/80/v2-d0b1d49ea435e054a5651484382567c1_720w.jpg" alt="img" style="zoom:50%;" />

####5.3 中心波长

![img](https://pic4.zhimg.com/80/v2-035bfaac788177e3b873935eb28a1f1f_720w.jpg)

<img src="https://pic3.zhimg.com/80/v2-244b7f89bb08a438e37a40edbf9bae26_720w.jpg" alt="img" style="zoom:50%;" />

###6. 光模块的基本指标

- 输出光功率（W，mW，dBm）

- 接收灵敏度最大值（dBm）
  - 一定速率、误码率条件下光模块的最小接收光功率
  - 速率越高，接收灵敏度越差

- 消光比
- 光饱和度（dBm）
  - 一定传输速率下，维持一定误码率时的最大输入功率

###7. 光模块的产业链

<img src="https://pic1.zhimg.com/80/v2-55075516c8e48a75b3c0bb07df0a20fc_720w.jpg" alt="img" style="zoom:67%;" />

<img src="https://pic1.zhimg.com/80/v2-98c53099f9349c6f98fad86d84ea6b88_720w.jpg" alt="img" style="zoom: 67%;" />