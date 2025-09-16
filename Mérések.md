## 1. Ellenállás és feszültségmérés:

### Ellenállás:

**Never measure resistance with the circuit live!!!**
1. Set your DMM to the resistance (Ω) range, for example 200Ω.
2. It is easiest to touch a fixed Neutral point (such as the neutral rail) and Line point. (The resistance of the wiring is negligible).

### Feszültség:
1. Set DMM to **AC volts** (select a range higher than the mains; e.g., 600 V).
2. Turn the power on.
3. It is easiest to touch a fixed Neutral point (such as the neutral rail) and Line point.

---

### Számítások:
- **R műszer = 0,7 Ω**  
    (R_műszer = instrument/meter resistance = 0.7 Ω)
    
- **R mért = 36,5 Ω**  
    (R_mért = measured resistance = 36.5 Ω)
    
- Curly brace connecting those two values to the right with the equation label:
    
    - **Rizzó = R mért − R műszer =**
        
    - **= 36,5 − 0,7 = 35,8 Ω**
        
- **Uk = 231 V** (supply / terminal voltage used)
    
- **Imax = Uk / Rizzó =**  
  $$
  I_{\text{max}} \;=\; \dfrac{231}{35{,}8} \;=\; 6{,}45\ \mathrm{A}
  $$
    (I_max computed as 231 ÷ 35.8 = 6.45 A)
    
- Efficiency/ratio line:
    
    - **η = Imax / Iüzemi = (orange text) Rmeleg / Rhideg =**  
      $$
      \eta \;=\; \dfrac{6{,}45}{0{,}442} \;=\; 14{,}6
      $$
        

### Üzem közbeni mérés:

- Curly brace grouping next to a small block of text:
    
    - **Uk = 231 V**
        
    - **Iü = 442 mA** (handwritten as **Iü = 442 mA** — which is 0,442 A)
        
- Resistance (hot) computed:
    
    - **Rmeleg = Uk / Iü =**  
      $$
      R_{\text{meleg}} \;=\; \dfrac{231}{0{,}442} \;=\; 522{,}6\ \Omega
      $$  
        (R_meleg = hot resistance = 522.6 Ω)
        
- Apparent power:
    
    - **S = Uk · Iü = 231 · 0,442 = 102 VA**

### Fogyasztás számítása mérővel:

Amikor villan a mérő, elindítom a stoppert és mérem mikor villan megint.

Energy meter pulse / power calculation

- Left text: **0,5 kWh/imp** (or “0,5 kWh/imp” — energy per pulse)
    
- **t_imp = 18 sec** (time per pulse measured as 18 s)
    
- Formula and result (boxed / circled):
    
    - **P = 3600 / t_imp · 0,5 = (3600 / 18) · 0,5 = 100 W**  
      $$
      P \;=\; \dfrac{3600}{t_{\text{imp}}}\cdot 0{,}5 \;=\; \left(\dfrac{3600}{18}\right)\cdot 0{,}5 \;=\; 100\ \mathrm{W}
      $$
---
