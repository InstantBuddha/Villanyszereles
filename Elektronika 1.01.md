
![[20250416_103553.jpg]] Some text
![[Adobe Scan 2025. ápr. 21._1.jpg]]
text
Átváltások:
![[Adobe Scan 2025. ápr. 21._2 1.jpg]]
Gyakorlás:

---

### **Átváltás (Conversions)**

_(Hungarian → English: “conversion”)_

#### **Normál alak (Scientific notation)**

```
500 mA   = 0.5 A      = 5 × 10⁻-¹ A  
2000 μA  = 0.002A        = 2 × 10⁰-3 A  
12,500 A = 12.5 kA    = 1.25 × 10⁴ A  
0.1 kΩ   = 100 Ω      = 1 × 10² Ω  
0.03 MΩ  = 30,000 Ω   = 3 × 10⁴ Ω  
1.2 kA   = 1200 A     = 1.2 × 10³ A  
20 mA    = 0.02 A     = 2 × 10⁻² A  
10 μA    = 0.00001 A  = 1 × 10⁻⁵ A  
0.06 kA  = 60 A       = 6 × 10¹ A  
0.12 mA  = 0.00012 A  = 1.2 × 10⁻⁴ A  
0.27 kA  = 270 A      = 2.7 × 10² A  
1.2 A    = 1200 mA    = 1.2 × 10³ mA  
0.38 A   = 380 mA     = 3.8 × 10² mA  
0.06 A   = 60 mA      = 6 × 10¹ mA  
36.2 A   = 36,200 mA  = 3.62 × 10⁴ mA  
1 MA     = 1,000,000 A= 1 × 10⁶ A  
20 μA    = 0.02 mA    = 2 × 10⁻² mA  
2060 V   = 2060,000 mV = 2.06 × 10⁶ mV  
720 mV   = 0.72 V     = 7.2 × 10⁻¹ V  
0.015 V  = 15 mV      = 1.5 × 10¹ mV  
0.02 μV  = 0.00000002 V = 2 × 10⁻⁸ V  
40 μV    = 0.00004 V  = 4 × 10⁻⁵ V  
3.2 MV   = 3,200,000 V = 3.2 × 10⁶ V  

---

### **Additional note at the bottom**
```

sebesség: km/h → m/s

## Feszültség és áramerősség iránya

When we say that **voltage** and **amperage (current)** have a **direction**, we're talking about the fact that both are **vector quantities** in the context of **circuit theory**, even though we often treat them like scalars in basic calculations.

Here's what that really means:

---

### ⚡ **Current (Amperage) Direction**
- **Current** is the **flow of electric charge**, typically carried by electrons.
- It has a direction: **from the positive to the negative terminal** in **conventional current flow** (opposite to the actual electron flow).
- In a circuit diagram, arrows show the direction of current.
- If you reverse the direction of current in a component (like a resistor), the **polarity of voltage across it will flip**.

---

### 🔋 **Voltage (Potential Difference) Direction**
- **Voltage** is the **difference in electric potential** between two points.
- It has a direction because it's measured **from one point to another**: e.g. “point A is +5V relative to point B”.
- If you reverse the direction of the voltage measurement (measure B relative to A), the sign of the voltage changes.

---

### 🔁 Why This Matters
- When analyzing a circuit (like with Kirchhoff's laws), you need to **be consistent with directions**.
- If your assumed direction is “wrong,” you won’t get an error — you'll just get a **negative value**, which means “opposite direction.”

---

### ✅ Example
If you have a resistor and:
- Current flows **left to right**, and
- Voltage across it is **+5V from left to right**,  
→ then the resistor **drops 5V** as current flows through it.

If you instead measured the voltage **right to left**, it would be **−5V**.

---
[[![[Adobe Scan 2025. ápr. 21._7.jpg]]]]
Here’s what your notes say, with a step‐by‐step English explanation:

---

### 1. Given data

- **Battery voltage**: 12 V  
- **Rated capacity**: 55 Ah  
- (You also note that 1 Ah = 3600 C, so the total charge capacity is  
  \[
- $$
    Q_{\rm tot} = 55\;\mathrm{Ah}\times3600\;\tfrac{\mathrm{C}}{\mathrm{Ah}}
               =198{,}000\;\mathrm{C}.
$$
  \])

---

### 2. Discharge over 12 hours leaves 25 Ah remaining

After 12 h of use, the battery still holds 25 Ah, so the amount **used up** is  
$$
\[
  Q_{\rm used} = 55\;\mathrm{Ah} - 25\;\mathrm{Ah} = 30\;\mathrm{Ah}.
\]
$$
---

### 3. What was the (average) discharge current?

Since you pulled 30 Ah out over 12 h, the average current was  
\[
$$
  I_{\rm load}
  = \frac{Q_{\rm used}}{t}
  = \frac{30\;\mathrm{Ah}}{12\;\mathrm{h}}
  = 2.5\;\mathrm{A}.
  $$
\]

---

### 4. How long to recharge that 30 Ah at 4 A?

If you feed in a constant 4 A charging current to replace the 30 Ah you used, the time required is  
\[
$$
  t_{\rm charge}
  = \frac{Q_{\rm used}}{I_{\rm charge}}
  = \frac{30\;\mathrm{Ah}}{4\;\mathrm{A}}
  = 7.5\;\mathrm{h}.
  $$
\]

---

**Summary in plain English:**

1. You started with a 12 V, 55 Ah battery (≈198 kC of charge).  
2. After 12 hours of use you’d drawn off 30 Ah (leaving 25 Ah).  
3. That corresponds to an average load current of 2.5 A.  
4. To put that 30 Ah back in at 4 A takes 7.5 hours of charging.

---

## 🔌 What is Voltage?

**Voltage** (also called *electric potential difference*) is the **force that pushes electric charges through a conductor**. It tells us how much potential energy each charge has at one point compared to another.

You can think of voltage as the “pressure” from an electric circuit's power source that pushes charged electrons (current) through a conducting loop.

### The formula for voltage is:

$$
V = \frac{W}{Q}
$$

Where:
- \( V \) = voltage (volts, V)  
- \( W \) = work or energy (joules, J)  
- \( Q \) = charge (coulombs, C)

So, **1 volt** means **1 joule of energy per coulomb of charge**.

---

## ⚡ Categories in Electric Conductivity

Electric conductivity is a measure of how easily electric charges can flow through a material.

There are **three main categories** based on how well a material conducts electricity:

### 1. **Conductors**
- **Examples:** Metals like copper, silver, aluminum
- **Properties:** Allow electricity to flow very easily
- **Reason:** Free electrons move easily through the material

### 2. **Insulators**
- **Examples:** Rubber, glass, plastic, air
- **Properties:** Resist the flow of electricity
- **Reason:** Electrons are tightly bound to atoms, so they can't move freely

### 3. **Semiconductors**
- **Examples:** Silicon, germanium
- **Properties:** Conductivity is between conductors and insulators
- **Special feature:** Can be modified to control the flow of electricity (basis of all modern electronics)

---

### Bonus: Electrical Conductivity Formula

The formula for **electrical conductivity** \( \sigma \) is:

$$
\sigma = \frac{1}{\rho}
$$

Where:
- \( \sigma \) = conductivity (siemens per meter, S/m)  
- \( \rho \) = resistivity (ohm-meter, \( \Omega \cdot \mathrm{m} \))

High conductivity ⇒ Low resistivity ⇒ Better conductor.

---

Let me know if you’d like visuals or more on semiconductors, resistors, or anything else!