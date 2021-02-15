## **多模干涉仪耦合器 MMI coupler**

### 1. 基本原理

自映像原理(Self-imaging)：在多模波导中，多个导模互相干涉，周期性出现输入场的一个或多个映像。

### 2. 推导

设多模干涉区宽度为$W_{MMI}$，长度为$L_{MMI}$，工作波长为$\lambda$，波导芯层、包层的有效折射率$n_r=n_{eff}$，$n_c$ 。第$\nu$个导模的纵向传播常数$\beta_{\nu}$与横向传播常数$k_{x\nu}$有如下关系：
$$
k_{x\nu}^2+\beta_{\nu}^2=k_0^2n_r^2
$$
$$
k_{x\nu}=\frac{(\nu+1)\pi}{W_{e\nu}}
$$

$W_{e\nu}$为第$\nu$个模式的有效宽度，各导模的有效宽度用基模的有效宽度来近似
$$
W_{e\nu}\approx W_e=W_m+(\frac{\lambda_0}{\pi})(\frac{n_{cl}^2}{n_{co}^2})^{2\sigma}(n_{co}^2-n_{cl}^2)^{-\frac{1}{2}}
$$
对于TE模极化，式中$\sigma=0$；对于TM模极化，式中$\sigma=1$。

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
   - 配对干涉模式(paired interference)：输入波导从多模干涉区的$\pm\frac{W}{6}$输入

<img src="G:\AresNing's Blogs\docs\OptoelectronicDevices\pics\image-20200923205008882.png" alt="image-20200923205008882" style="zoom: 50%;" />

###3. 重叠成像 Overlapping Imaging

输入场$x_0$沿某个方向移动，正像和反像移动的方向相反；所有正像（或反像）移动方向相同，且任意两个正像（或反像）移动前后间距不变。

正像之间或反像之间不可能出现重叠；正像与反像之间可以出现重叠。

<img src="G:\AresNing's Blogs\docs\OptoelectronicDevices\pics\image-20201027084138131.png" alt="image-20201027084138131" style="zoom:50%;" />

####3.1 重叠成像的条件

输入场位置$x_0$为 W/N 整数倍，出现重叠成像，输出场所得的像的个数小于N并形成新的强度分布
$$
x_0=i\frac{W}{N}\quad\quad(i=1,2...N-1)
$$

#### 3.2 成像位置和个数

##### 3.2.1 特殊重叠成像：像的强度分布相同

- N为2的倍数，且$i=N/2$（即$x_0=W/2$）
- N为3的倍数，且$i=N/3$（即$x_0=W/3$）或$i=2N/3$（即$x_0=2W/3$）

#####3.2.2 一般重叠成像：像的强度分布不同

- 除了特殊重叠成像以外的重叠成像



