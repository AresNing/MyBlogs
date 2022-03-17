# Binary / Ternary / Quaternary Material Parameters

## Vegard's law

### Ternary ($A_{1-x}B_xC$)

$$
P(A_{1-x}B_xC)=(1-x)P(AC)+xP(BC)
$$
> P for Parameters

### Quaternary ($A_{1-x}B_xC_yD_{1-y}$)

$$
P(A_{1-x}B_xC_yD_{1-y})=(1-x)yP(AC)+(1-x)(1-y)P(AD)+xyP(BC)+x(1-y)P(BD)
$$

## Binary compounds

### Lattice constant  $a_0$ ($\overset{\circ}{A}$)

- InP: 5.8688
- GaAs: 5.6533
- InAs: 6.0584
- GaP: 5.4505
- AlAs: 5.6600

### Energy band structure $E_g$ (eV, at 300K)

- InP: 1.344
- GaAs: 1.424
- InAs: 0.354
- GaP: 2.78
- AlAs: 3.03

## Ternary compounds

### Lattice constant $a_0$ ($\overset{\circ}{A}$)

According to Vegard's law, 
$$
a(A_{1-x}B_xC)=(1-x)a(AC)+xa(BC)
$$

### Energy band structure $E_g$  (eV, at 300K)

$$
\begin{aligned}
E_g(In_{1-x}Ga_xP)&=1.35+0.643x+0.786x^2\\
E_g(In_{1-x}Ga_xAs)&=0.36+0.505x+0.555x^2\\
E_g(InAs_yP_{1-y})&=1.35-1.083y+0.091y^2\\
E_g(GaAs_yP_{1-y})&=2.74-1.473y+0.146y^2
\end{aligned}
$$

$$
E_g(In_{0.53}Ga_{0.47}As)=0.75
$$

## Quaternary compounds

### Lattice constant $a_0$ ($\overset{\circ}{A}$)

- $In_{1-x}Ga_xAs_yP_{1-y}$
  $$
  \begin{aligned}
  a(In_{1-x}Ga_xAs_yP_{1-y}) &=xy\cdot a(GaAs)+x(1-y)\cdot a(GaP)+(1-x)y\cdot a(InAs)+(1-x)(1-y)\cdot a(InP)\\
  &=5.8688-0.4176x+0.1896y+0.0125xy
  \end{aligned}
  $$

- $In_{1-x}Ga_xAs_yP_{1-y}$ on InP substrate
  $$
  x=\frac{0.1894y}{0.4184-0.013y}\approx0.47y
  $$

- $In_{1-x}Ga_xAs_yP_{1-y}$ on GaAs substrate
  $$
  x=\frac{1.00+y}{2.08}
  $$

### Energy band structure $E_g$  (eV, at 300K)

- $In_{1-x}Ga_xAs_yP_{1-y}$
  $$
  E_g(In_{1-x}Ga_xAs_yP_{1-y})=1.35+0.668x-1.068y+0.758x^2+0.078y^2-0.069xy-0.322x^2y+0.03xy^2
  $$

- $In_{1-x}Ga_xAs_yP_{1-y}$ on InP substrate
  $$
  E_g=1.35-0.775y+0.149y^2
  $$

## Ref.

1. [Adachi, Sadao. Material parameters of In1-xGaxAsyP1-y and related binaries. Journal of Applied Physics, 53.12 (1982): 8775-8792.](https://aip.scitation.org/doi/abs/10.1063/1.330480)
2. Physics of Photonic Devices_Chuang, Shun Lien_2012.（光子器件物理-第二版-庄连顺）

