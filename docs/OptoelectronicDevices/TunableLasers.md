## **可调谐激光器 Tunable Lasers**

### 1. 分布式布拉格反射（DBR）激光器

![image-20200918095101032](G:\AresNing's Blogs\docs\OptoelectronicDevices\pics\image-20200918095101032.png)

1. 原理
  
   - $2\Lambda n=\lambda_b$，其中$\Lambda$为光栅周期，$n$为折射率，$\lambda_b$为光栅的中心波长
   
2. 可调谐性

   DBR可分为三个区：有源区、相移区、光栅区

   - 相移区：使谐振波长$\lambda_m$与布拉格波长$\lambda_b$一致，即$\Phi_1=\Phi_2+2m\pi$，其中$\Phi_1$为光栅区的相位变化，$\Phi_2$为有源区和相位区的相位变化

   - 光栅区：单纵模选择，改变光栅的中心波长

   - 仅改变$\lambda_m$，只能在$\lambda_b$附近极小范围得到周期性连续调谐，可避免跳模

   - 仅改变$\lambda_b$，只能得到不连续调谐并出现跳模

   - 同时改变$\lambda_m$和$\lambda_b$，可能在较大范围内得到准连续调谐

<img src="G:\AresNing's Blogs\docs\OptoelectronicDevices\pics\image-20200918110701518.png" alt="image-20200918110701518" style="zoom: 67%;" />

3. 优点

   - 损耗减小，发光效率提高：有源区与光栅区分开
   - 阈值电流较低，可实现室温连续工作

4. 缺点

   - 光栅区内注入电流能引起的有效折射率最大变化范围限制了波长的调谐范围


### 2. 分布式反馈布拉格（DFB）激光器

![image-20200918095049104](G:\AresNing's Blogs\docs\OptoelectronicDevices\pics\image-20200918095049104.png)

1. 原理

   - $2\Lambda\eta sin\theta=m\lambda$，其中$\Lambda$为光栅周期，$\eta$为材料等效折射率，$\theta$为衍射角

   - $2\Lambda n=m\lambda$，介质内前后向传播的光波可视为衍射角$\theta=90^{\circ}$，其中$n$为半导体介质的折射率
2. 优点

   - 发射频率选择范围宽，完全由光栅周期$\Lambda$决定
3. 缺点
   - 光损耗较大，器件发光效率较低：光栅直接刻在有源区上
   - 工作寿命短，通常以脉冲方式工作

###3. 耦合腔激光器（两个长度不同的谐振腔的耦合）（游标效应）

1. 具有刻蚀槽的解理F-P激光器
 	2. 解理耦合腔（两个串联的耦合腔、干涉效应）
  3. 级联耦合腔

###4. Y型耦合腔（干涉效应）

<img src="G:\AresNing's Blogs\docs\OptoelectronicDevices\pics\image-20200917112403037.png" alt="image-20200917112403037" style="zoom: 67%;" />

### 5. V型耦合腔（固定增益腔+波长选择腔）（游标效应）

<img src="G:\AresNing's Blogs\docs\OptoelectronicDevices\pics\image-20200913114408192.png" alt="image-20200913114408192" style="zoom: 33%;" />

1. 原理
   - 固定增益腔的谐振频率$f=\dfrac{mc}{2n_gL}$，频率间隔$\Delta f=\dfrac{c}{2n_gL}$
   - 波长选择腔的谐振频率$f'=\dfrac{mc}{2n_g'L'}$，频率间隔$\Delta f'=\dfrac{c}{2n_g'L'}=\dfrac{c}{2(n_aL_a+n_bL_b)}$
   - 组合腔的自由光谱范围（FSR）$\Delta f_c=\dfrac{\Delta f\Delta f'}{|\Delta f-\Delta f'|}=\dfrac{c}{2|n_g'L'-n_gL|}$
   - 为了避免两个波长同时被泵浦，$\Delta f_c$一般必须大于激光器增益谱宽度。
   <img src="G:\AresNing's Blogs\docs\OptoelectronicDevices\pics\image-20200701204119498.png" alt="image-20200701204119498" style="zoom:50%;" />
   - 激光器工作频率的改变量$\delta f=\dfrac{\Delta f}{|\Delta f-\Delta f'|}\delta f'$ （游标效应）

2. 阈值条件分析

   <img src="G:\AresNing's Blogs\docs\OptoelectronicDevices\pics\image-20200913114853850.png" alt="image-20200913114853850" style="zoom:50%;" />

   - $r_1\eta r_2e^{2(g+ik)L}=1$ 或 $r_1\eta’ r_2e^{2(g'+ik’)L}=1$

   - 代入$\eta$或$\eta'$后，均可简化为下式：

     $C_{11}r_1r_2e^{2(g+ik)L}+C_{22}r_1r_2e^{2(g'+ik')}-(C_{11}C_{22}-C_{21}C_{12})r_1^2r_2^2e^{2(g+ik)L}e^{2(g'+ik')L}=1$

3. 模式选择性（边模抑制比）

   - 定量分析：主模（阈值最低的模）和边模（阈值次低模）之间的阈值差来衡量。阈值差越大，选模特性越好

   - 可通过选择合适的两个谐振腔之间的交叉耦合系数$C_{12}$和$C_{21}$来优化

   - 交叉耦合系数减小，反射率修正因子（有效反射率）$|\eta|^2$的谐振峰变窄（模式选择性变好），但是对比度（阈值差）降低

     <img src="G:\AresNing's Blogs\docs\OptoelectronicDevices\pics\image-20200702135408030.png" alt="image-20200702135408030" style="zoom: 50%;" />

     <img src="G:\AresNing's Blogs\docs\OptoelectronicDevices\pics\image-20200702142837586.png" alt="image-20200702142837586" style="zoom:50%;" />

   - 增加固定增益腔和波长选择腔的长度差，可增加阈值差，但同时降低$\Delta f_c$；当两个谐振腔中的回路增益相等，即$gL=g'L'$，阈值差达到最大，模式选择性最高，故应尽量避免回路增益的波动

     <img src="G:\AresNing's Blogs\docs\OptoelectronicDevices\pics\image-20200916214857363.png" alt="image-20200916214857363" style="zoom: 67%;" />
     
     <img src="G:\AresNing's Blogs\docs\OptoelectronicDevices\pics\image-20200702191313894.png" alt="image-20200702191313894" style="zoom: 50%;" />
   
4. 半波耦合器的设计（重要组成部分）

   <img src="G:\AresNing's Blogs\docs\OptoelectronicDevices\pics\image-20200916202022663.png" alt="image-20200916202022663" style="zoom: 80%;" />

   - 目的：实现两个端口有同步的输出，即在某谐振波长下两个端口输出能量同时达到最大

   - 满足条件：$|C_{11}|+|C_{21}|=1$和$|C_{12}|+|C_{22}|=1$

   <img src="G:\AresNing's Blogs\docs\OptoelectronicDevices\pics\image-20200916203554360.png" alt="image-20200916203554360" style="zoom:50%;" />

   两个输入电场的相位相反，即$\varphi=\pi$，两个输出电场同时达到最大；

   两个输入电场的相位相同，两个输出电场达到最小

   - 结构：三个平行波导形成两个$\frac{1}{4}$波耦合器（定向耦合器），整体形成半波耦合器，实际操作中把中间的波导与两个相邻波导合并连接

     ![image-20200916204536930](G:\AresNing's Blogs\docs\OptoelectronicDevices\pics\image-20200916204536930.png)
     
     

5. 优点

   - 无需较大的器件尺寸和复杂的光栅结构即可实现宽的调谐范围（利用深刻蚀槽作为反射镜）
   
   - Y型耦合腔的交叉耦合系数不能小于自耦合系数；V型耦合腔的交叉耦合系数可以小于自耦合系数，从而达到更大的边模抑制比和单模选择性
   
6. （补充）多模干涉仪耦合器(MMI coupler)

   1. 基本原理 - 自映像原理(Self-imaging)：在多模波导中，多个导模互相干涉，周期性出现输入场的一个或多个映像。

   2. 推导

   设多模干涉区宽度为$W_{MMI}$，长度为$L_{MMI}$，工作波长为$\lambda$，波导芯层、包层的有效折射率$n_r=n_{eff}$，$n_c$ 。第$\nu$个导模的纵向传播常数$\beta_{\nu}$与横向传播常数$k_{x\nu}$有如下关系：
   $$
   k_{x\nu}^2+\beta_{\nu}^2=k_0^2n_r^2
   $$
   $$
   k_{x\nu}=\frac{(\nu+1)\pi}{W_{e\nu}}
   $$

   $W_{e\nu}$为第$\nu$个模式的有效宽度，各导模的有效宽度用基模的有效宽度来近似
   $$
   W_{e\nu}\approx W_e
   $$
   推导可得(旁轴近似)
   $$
   \beta_{\nu}\approx k_0n_r-\frac{(\nu+1)^2\pi\lambda}{4n_rW_e^2}
   $$
   定义$L_\pi$为基模和一阶导模的拍长
   $$
   L_\pi=\frac{\pi}{\beta_0-\beta_1}=\frac{\lambda
   }{2(n_{eff0}-n_{eff1})}\approx\frac{4n_rW_e^2}{3\lambda}
   $$
   各阶导模的传播常数差为
   $$
   \Delta\beta_{0\nu}=\beta_0-\beta_\nu\approx\frac{\nu(\nu+2)\pi}{3L_\pi}
$$
   
- 普通干涉模式(general interference)：输入波导的输入位置无任何限制
  
  <img src="G:\AresNing's Blogs\docs\OptoelectronicDevices\pics\image-20200923205225846.png" alt="image-20200923205225846" style="zoom: 67%;" />
  
- 限制干涉模式(restricted interference)：输入波导的输入位置相对于多模干涉区的中心偏移$\pm\frac{W_{MMI}}{6}$时
  
   - 对称干涉模式(symmetric interference)：输入波导从多模干涉区的中心输入

<img src="G:\AresNing's Blogs\docs\OptoelectronicDevices\pics\image-20200923205008882.png" alt="image-20200923205008882" style="zoom: 50%;" />