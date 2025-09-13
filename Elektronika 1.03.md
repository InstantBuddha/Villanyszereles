A végén hibáztunk:

1. **Kilowatt-hour (kW·h)**  
   - This is a unit of **energy**, defined as the work done by a constant power of 1 kW acting for 1 hour.  
   - Since 1 W·s = 1 J (joule), you can convert kW·h to watt-seconds (Ws) like so:  
     
     \[
   $$
     1~\text{kW·h} = 1000~\text{W} \times 3600~\text{s}
                  = 3\,600\,000~\text{W·s}
                  = 3.6\times10^{6}~\text{J}.
                  $$
     \]
   
### Quick Reference

| Unit   | Physical quantity | Conversion to watt-seconds (energy) |
| ------ | ----------------- | ----------------------------------- |
| 1 kW·h | Energy            | 3 600 000 W·s (3.6 MJ)              |
| 1 W·s  | Energy            | 1 J                                 |
|        |                   |                                     |

- **Key point:** Use **kW·h** when you mean “kilowatts for hours” (an energy). 
Quick formulas to memorize
$$
    EkWh=EW ⁣⋅ ⁣s3 600 000
    EkWh=3600000EW⋅s
     
    EW ⁣⋅ ⁣s=EkWh×3 600 000
    EW⋅s=EkWh×3600000
$$



---
I have 2 resistors in series. I know R1=300ohm, R2=600ohm and I know the input voltage which is 180V. How can I calculate the voltage on each resistor only using ohms law? 
## 1. Total resistance in series

Two resistors $R_1$ and $R_2$ in series simply add:


$$
R_{\rm total} = R_1 + R_2
= 300\ \Omega + 600\ \Omega
= 900\ \Omega
$$

![[Elektronika_1_03_2.jpg]]
P02
Uki magyarázata: ez a feszültség esés az ellenálláson

---

## 2. Circuit current via Ohm’s law

The same current $I$ flows through both resistors. By Ohm’s law,


$$
I = \frac{V_{\rm in}}{R_{\rm total}}
= \frac{180\ \text{V}}{900\ \Omega}
= 0.2\ \text{A}
$$


---

## 3. Voltage drop on each resistor

Each drop is $V = I\,R$:

1. **Across $R_1$:**

   
   $$
   V_1 = I\,R_1
       = 0.2\ \text{A}\times 300\ \Omega
       = 60\ \text{V}
   $$
   

2. **Across $R_2$:**

   
   $$
   V_2 = I\,R_2
       = 0.2\ \text{A}\times 600\ \Omega
       = 120\ \text{V}
   $$
   

---

## 4. Quick check

Since they’re in series, $V_1 + V_2$ should equal the input:


$$
V_1 + V_2 = 60\ \text{V} + 120\ \text{V} = 180\ \text{V}
$$


---

Just copy the above into your Obsidian note, and the math blocks will render cleanly.
