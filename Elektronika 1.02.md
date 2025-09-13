P01

![[Elektronika_1_02_1.jpg]]

## Elektronika 1. 2. alkalom

- vizsgán 1 motoros (vagy 1 világításos) feladatból kell húzni
- Feszültség, tér munkavégző képessége

elektronos feszültség    U    volt    V    U = W / Q  
                         1 V = 1 J / 1 C = 1 Ws / 1 As

elektromos ellenállás    R resistance    ohm    Ω  
Ohm törvény: R = U / I ;  1 V / 1 A = 1 Ω

Ohm-törvény: zárt áramkörben a fogyasztók kapcsán mérhető feszültség és a rajta átfutó áram hányadosa állandó és jellemzi a fogyasztót

- elektronos vezetés, G [siemens] S  
  G = 1 / R ; 1 S = 1 / Ω = (1 Ω)⁻¹  
  (vezetés az ellenállás reciproka)

- Kirchhoff I-es törvénye  
  Áramokra vonatkozó csomóponti törvény:
	A csomópontban befolyó áramok összege megegyezik az onnan kifolyó áramok összegével
  I₁ + I₂ + I₅ = I₃ + I₄


P02
![[Elektronika_1_02_2.jpg]]

### 1️⃣ Kirchhoff’s Current Law (KCL)  
**Node (junction) rule**  

> **Statement:**  
> The algebraic sum of currents entering a node (or junction) is zero.

\[
$$
\sum_{k=1}^{n} I_k = 0
$$
\]

- **Sign convention:**  
  - Choose a reference direction (e.g. currents entering the node as **+**, leaving as **–**, or vice versa).  
  - Be consistent for all currents at that node.

- **General form:**  
$$
  I₁ + I₂ + … + I_m  –  (I_{m+1} + … + I_n) = 0
$$


or more compactly
$$
∑inI  −  ∑outI  =  0 \sum_{\text{in}} I \;-\;\sum_{\text{out}} I \;=\;0
$$
- **Example:**  
    At a 4-way junction:
    $$
    I1+I2=I3+I4⟺I1+I2−I3−I4=0 I_1 + I_2 = I_3 + I_4 \quad\Longleftrightarrow\quad I_1 + I_2 - I_3 - I_4 = 0
    $$

---

### 2️⃣ Kirchhoff’s Voltage Law (KVL)

**Loop rule**

> **Statement:**  
> The algebraic sum of all voltage rises and drops around any closed loop is zero.

$$
∑k=1mVk=0\sum_{k=1}^{m} V_k = 0
$$

- **Sign convention:**
    
    1. Pick a loop direction (clockwise or counter-clockwise).
        
    2. For each element, assign a **+** if you go from negative to positive terminal (voltage rise), **–** for positive to negative (voltage drop).
        
- **General form:**
    
$$
    +V_source – V_R1 – V_R2 – … – V_Rn = 0
$$
    
    or
    
$$
∑rises(+V)  +  ∑drops(−V)  =  0 \sum_{\text{rises}} (+V) \;+\;\sum_{\text{drops}} (-V) \;=\;0
$$

- **Example:**  
    Simple series loop with a source EE and resistors R1,R2R_1, R_2:
$$
    +E−I R1−I R2=0⟹E=I (R1+R2) +E - I\,R_1 - I\,R_2 = 0 \quad\Longrightarrow\quad E = I\,(R_1 + R_2)
$$    

---

P03
![[Elektronika_1_02_3.jpg]]

## A fogyasztók soros és párhuzamos kapcsolása

### A fogyasztók soros eredője
Ha sorba vannak kötve a fogyasztók, ellenállások, az eredőjük az összegük lesz.

Jó leírás:
https://www.electronics-tutorials.ws/resistor/res_3.html

### Series Equivalent Resistance (English)

When resistors are connected **in series**, their equivalent behaves like a single resistor whose value is the sum of the individual resistances.

1. **Current**  
    The same current III flows through each resistor:
    $$
    I=I1=I2=⋯=In. I = I_1 = I_2 = \dots = I_n.I=I1​=I2​=⋯=In​.
    $$
2. **Voltage drops**  
    The total voltage UUU across the series chain equals the sum of each voltage drop:
    $$
    U=U1+U2+⋯+Un,whereUk=I Rk. U = U_1 + U_2 + \dots + U_n, \quad\text{where}\quad U_k = I\,R_k.U=U1​+U2​+⋯+Un​,whereUk​=IRk​.
    $$
3. **Equivalent resistance**  
    Substitute the drops into Kirchhoff’s voltage law:
    $$
    U=I Req=I (R1+R2+⋯+Rn)⟹Req=∑k=1nRk. U = I\,R_\text{eq} = I\,(R_1 + R_2 + \dots + R_n) \quad\Longrightarrow\quad R_\text{eq} = \sum_{k=1}^n R_k.U=IReq​=I(R1​+R2​+⋯+Rn​)⟹Req​=k=1∑n​Rk​.
    $$
4. **Key property**  
    The equivalent resistance of series resistors is always **greater** than the largest individual resistance in the chain.
    $$
    Req>max⁡{R1,R2,…,Rn}. R_\text{eq} > \max\{R_1, R_2, \dots, R_n\}.Req​>max{R1​,R2​,…,Rn​}.
    $$
P04
![[Elektronika_1_02_4.jpg]]

## Parallel Equivalent Resistance

Nagyon jó leírás:
https://www.electronics-tutorials.ws/resistor/res_4.html

When resistive elements (or “loads”) are connected **in parallel**, they share the same voltage but carry different branch currents. The total current divides among the branches, and you can replace the whole network by a single equivalent resistor 
$$
\(R_\mathrm{eq}\).
$$

---

### 1️⃣ Voltage and Currents

- **Common voltage** across every branch:  
  $$
  U = U_1 = U_2 = \dots = U_n
  $$

- **Currents add up** at the junction (Kirchhoff’s Current Law):  
  $$
  I_\mathrm{tot} = I_1 + I_2 + \dots + I_n
  $$

  where each branch current is  
  $$
  I_k = \frac{U}{R_k}.
  $$

---

### 2️⃣ Derivation of \(R_\mathrm{eq}\)

By definition of the equivalent resistor,
$$
I_\mathrm{tot} = \frac{U}{R_\mathrm{eq}}.
$$
But also
$$
I_\mathrm{tot}
= \sum_{k=1}^n I_k
= \sum_{k=1}^n \frac{U}{R_k}
= U \sum_{k=1}^n \frac{1}{R_k}.
$$
Equate the two expressions for \(I_\mathrm{tot}\):
$$
\frac{U}{R_\mathrm{eq}}
= U \sum_{k=1}^n \frac{1}{R_k}
\quad\Longrightarrow\quad
\frac{1}{R_\mathrm{eq}} = \sum_{k=1}^n \frac{1}{R_k}.
$$

---

### 3️⃣ Special cases

- **Two resistors in parallel** \((n=2)\):
  $$
  \frac{1}{R_\mathrm{eq}}
  = \frac{1}{R_1} + \frac{1}{R_2}
  \quad\Longrightarrow\quad
  R_\mathrm{eq} = \frac{R_1 R_2}{R_1 + R_2}.
  $$

- **General \(n\)**:
  $$
  R_\mathrm{eq}
  = \frac{1}{\displaystyle\sum_{k=1}^n \frac{1}{R_k}}.
  $$

---

### 4️⃣ Key property

The equivalent resistance of parallel resistors is always **smaller** than the smallest individual resistance:

$$
R_\mathrm{eq} < \min\{R_1, R_2, \dots, R_n\}.
$$

---
## Calculating Parallel Equivalent Resistance

When $n$ resistors $R_1, R_2, \dots, R_n$ are connected in parallel:

1. **Common voltage** $U$ appears across each resistor.  
2. **Branch currents** are  
   $$
   I_k = \frac{U}{R_k},\quad k = 1, \dots, n.
   $$
3. **Total current** by KCL:  
   $$
   I_{\text{tot}} = \sum_{k=1}^n I_k = \sum_{k=1}^n \frac{U}{R_k} = U \sum_{k=1}^n \frac{1}{R_k}.
   $$
4. **Define** $R_{\text{eq}}$ by  
   $$
   I_{\text{tot}} = \frac{U}{R_{\text{eq}}}.
   $$
5. **Equate** and solve for $R_{\text{eq}}$:  
   $$
   \frac{U}{R_{\text{eq}}} = U \sum_{k=1}^n \frac{1}{R_k} \quad\Longrightarrow\quad \frac{1}{R_{\text{eq}}} = \sum_{k=1}^n \frac{1}{R_k}.
   $$

---

### Two resistors ($n = 2$)

$$
\frac{1}{R_{\text{eq}}} = \frac{1}{R_1} + \frac{1}{R_2}
\quad\Longrightarrow\quad
R_{\text{eq}} = \frac{1}{\displaystyle \frac{1}{R_1} + \frac{1}{R_2}} = \frac{R_1 R_2}{R_1 + R_2}.
$$

---

### Three or more resistors ($n \ge 3$)


$$
\frac{1}{R_{\text{eq}}} = \frac{1}{R_1} + \frac{1}{R_2} + \dots + \frac{1}{R_n}
\quad\Longrightarrow\quad
R_{\text{eq}} = \frac{1}{\displaystyle \sum_{k=1}^n \frac{1}{R_k}}.
$$


P05
![[Elektronika_1_02_5.jpg]]
P06
![[Elektronika_1_02_6.jpg]]
Ugyanez rajzolva:
https://www.circuit-diagram.org/circuits/3b2434ae06144afd83e82ccb80da2afd
![[P10_circuit.jpg]]
P07
![[Elektronika_1_02_7.jpg]]
P08
![[Elektronika_1_02_8.jpg]]
P09
![[Elektronika_1_02_9.jpg]]
P10
![[Elektronika_1_02_10.jpg]]
## vegyes (soros és párhuzamos) kapcsolás egyszerre:

Jó leírás:
https://www.electronics-tutorials.ws/resistor/res_5.html

P11
![[Elektronika_1_02_11.jpg]]
P12
![[Elektronika_1_02_12.jpg]]
P13
![[Elektronika_1_02_13.jpg]]
P14
![[Elektronika_1_02_14.jpg]]