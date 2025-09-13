Excellent — you're absolutely correct: Obsidian supports LaTeX-style math rendering inside either:

* Inline: `$ ... $`
* Block: `$$ ... $$`

I'll now rewrite the full content with Obsidian-friendly formatting. You can copy-paste this directly into your notes.

---
### Szinuszos váltakozóáram teljesítménye

A szinuszos váltakozóáram pillanatnyi teljesítménye periodikusan változik hasonlóan a feszültséghez és az áramerősséghez. A váltakozóáram átlagos effektív (hatásos) teljesítménye egy periódus (és így hosszabb idő) alatt:

P = U I cos ⁡ ϕ ![{\displaystyle P=UI\cos \phi }](https://wikimedia.org/api/rest_v1/media/math/render/svg/9142dc5cf971c091b1a3fc2fb484a8506be5d266) ,

ahol

U ![{\displaystyle U\,}](https://wikimedia.org/api/rest_v1/media/math/render/svg/435be01e77ffd4af9dd1ea8152a657958eecdf1c) az effektív feszültség,

I ![{\displaystyle I\,}](https://wikimedia.org/api/rest_v1/media/math/render/svg/988f6ada07675268dc7164f44f469dbec6e00b8a) az effektív áramerősség

ϕ ![{\displaystyle \phi \,}](https://wikimedia.org/api/rest_v1/media/math/render/svg/c69f1c4a95b2d750b30fa4cf5d5d068a573ac0d8) pedig a [fázisszög](https://hu.wikipedia.org/wiki/F%C3%A1ziseltol%C3%B3d%C3%A1s "Fáziseltolódás")

A háztartási villanyórák ezt mérik, a fogyasztókon ez hasznosul.

A hatásos teljesítmény mellett fontos fogalom a látszólagos és a meddő teljesítmény is.

![[Pasted image 20250615152109.png]]

A [látszólagos teljesítmény](https://hu.wikipedia.org/w/index.php?title=L%C3%A1tsz%C3%B3lagos_teljes%C3%ADtm%C3%A9ny&action=edit&redlink=1 "Látszólagos teljesítmény (a lap nem létezik)") (S) nem veszi figyelembe az esetleges fázistolás hatását az áram munkavégző képességére.

Számítása:

S = U I ![{\displaystyle S=UI}](https://wikimedia.org/api/rest_v1/media/math/render/svg/bceaadcb09f66e2a264d1303fd363a0c663ab5b7) , ahol U és I a megfelelő effektív értékek.

Mértékegysége VA (Voltamper).

Értéke nem lehet kisebb a hatásos teljesítménynél, de abban az esetben, ha c o s ϕ = 1 ![{\displaystyle cos\phi =1\,}](https://wikimedia.org/api/rest_v1/media/math/render/svg/b9ad3b390bbcbdf2509f10e11ab36d1c02c41249) , akkor megegyezik vele.

Például transzformátorok, generátorok jellemzésére használatos, melyeknél nem ismertek előre a terhelés által létrehozott fázistolások.

A [meddő teljesítmény](https://hu.wikipedia.org/wiki/Medd%C5%91_teljes%C3%ADtm%C3%A9ny_m%C3%A9r%C3%A9se "Meddő teljesítmény mérése") (Q) a látszólagos és a hatásos teljesítmény vektori különbségeként számítható képzetes fogalom.

Q = U I sin ⁡ ϕ ![{\displaystyle Q=UI\sin \phi }](https://wikimedia.org/api/rest_v1/media/math/render/svg/dba9532933c85d45cdab2283e6147b91de0ce797) 

Mértékegysége a VAr (Voltamper reaktív)

A meddő teljesítmény nem jelenik meg hasznos munkaként (innen ered az elnevezése is), káros hatásai viszont a betáplálási oldalon jelentkeznek, ezért célszerű csökkenteni.

s i n ϕ ![{\displaystyle sin\phi }](https://wikimedia.org/api/rest_v1/media/math/render/svg/513e336edd0107120a637bac9bc3b2d82d2b3131) előjelétől függően lehet a meddő teljesítmény induktív vagy kapacitív jellegű, ezek egymást gyengítik.

A [fázisjavítás](https://hu.wikipedia.org/wiki/F%C3%A1zisjav%C3%ADt%C3%A1s "Fázisjavítás") felfogható a meddő teljesítmények egymást kioltó hatásaként.

Ha c o s ϕ = 0 ![{\displaystyle cos\phi =0\,}](https://wikimedia.org/api/rest_v1/media/math/render/svg/5dc423a98fe059e4af3f050e65481306b640138b) , akkor a látszólagos és a meddő teljesítmény megegyezik, hatásos teljesítmény nem lép fel.

## Fáziseltolódás

Egyenáramú hálózatokban az [áram](https://hu.wikipedia.org/wiki/%C3%81ram "Áram") és a [feszültség](https://hu.wikipedia.org/wiki/Elektromos_fesz%C3%BClts%C3%A9g "Elektromos feszültség") időben egybeesik, viszont [váltakozó áramú](https://hu.wikipedia.org/wiki/V%C3%A1lt%C3%B3%C3%A1ram "Váltóáram") hálózatokban csak ideális esetben vannak egymással fázisban (amikor nincs közöttük időbeni eltérés). A szinuszos változás közben az áram a feszültséghez képest vagy siet ([kapacitív](https://hu.wikipedia.org/wiki/Kondenz%C3%A1tor_\(elektronika\) "Kondenzátor (elektronika)") tag esetén), vagy késik ([induktív](https://hu.wikipedia.org/wiki/Induktivit%C3%A1s "Induktivitás") tag esetén). A két görbe egymáshoz képest időben el van tolva. Az áram és a feszültség által bezárt [szög](https://hu.wikipedia.org/wiki/Sz%C3%B6g "Szög") a fázisszög, melynek a jele ![{\displaystyle \varphi }](https://wikimedia.org/api/rest_v1/media/math/render/svg/33ee699558d09cf9d653f6351f9fda0b2f4aaa3e) (fí). Ezt az eltolódást **fáziseltolódásnak** nevezzük.

### Elmélete
 Váltakozó áramú körökben csak ideális esetben van az a helyzet, amikor a [feszültség](https://hu.wikipedia.org/wiki/Elektromos_fesz%C3%BClts%C3%A9g "Elektromos feszültség") és az [áram](https://hu.wikipedia.org/wiki/Elektromos_%C3%A1ram "Elektromos áram") időben egybeesik, egymáshoz viszonyítva nincs eltérés. Ekkor az általuk bezárt szög φ=0. Ez csak ideális hálózatokra jellemző. A hatásos teljesítményből levezethetően P=U×I×cos φ ebből a cos φ=P/(U×I) Ezt a cos φ-t nevezik fázistényezőnek.

### Jelentősége
A generátor S ![{\displaystyle S}](https://wikimedia.org/api/rest_v1/media/math/render/svg/4611d85173cd3b508e67077d4a1252c9c05abca2) látszólagos [teljesítmény](https://hu.wikipedia.org/wiki/Teljes%C3%ADtm%C3%A9ny "Teljesítmény")éből annak csak egy része hasznosul hatásos teljesítmény formájában. Mivel az áram és a feszültség egymással szöget zár be, így egy adott időpillanatban vizsgálva annak csak az arra az időpillanatra eső vektora hasznosul – ugyanis ennek a nagysága a bezárt szögtől függ, ami megegyezik a cos ⁡ φ ![{\displaystyle \cos \varphi }](https://wikimedia.org/api/rest_v1/media/math/render/svg/544fef63b011ca474c1f9e4ffad26719f1068213) -szeresével. Így a hatásos teljesítmény P = U ⋅ I ⋅ cos ⁡ φ ![{\displaystyle P=U\cdot I\cdot \cos \varphi }](https://wikimedia.org/api/rest_v1/media/math/render/svg/daaebd0706c9e288007849c2eb9c8accc69f90f2) mechanikai munkaként (vagy hőleadásként), míg a meddő teljesítmény Q = U ⋅ I ⋅ sin ⁡ φ ![{\displaystyle Q=U\cdot I\cdot \sin \varphi }](https://wikimedia.org/api/rest_v1/media/math/render/svg/4b50df03678fb29cd789408e21c45d56c6effeb8) – veszteségként jelentkezik. A meddő teljesítmény a berendezés körüli [villamos](https://hu.wikipedia.org/wiki/Elektromos_mez%C5%91 "Elektromos mező") illetve [mágneses tér](https://hu.wikipedia.org/wiki/M%C3%A1gneses_mez%C5%91 "Mágneses mező") fenntartására fordítódik.
### Fázisjavítás
A fáziseltolódás általában [induktív](https://hu.wikipedia.org/w/index.php?title=Indukt%C3%ADv&action=edit&redlink=1 "Induktív (a lap nem létezik)") irányba mutat, amit a hálózatra kapcsolt induktív jellegű fogyasztó ([transzformátor](https://hu.wikipedia.org/wiki/Transzform%C3%A1tor "Transzformátor"), [villamos motor](https://hu.wikipedia.org/wiki/Villamos_motor "Villamos motor") stb.) okoz. Amennyiben egy hálózaton induktív és kapacitív jellegű eszközök is vannak, úgy az [rezgőkört](https://hu.wikipedia.org/wiki/Rezg%C5%91k%C3%B6r "Rezgőkör") alkot. **cos φ =1** esetén a rezgőkör frekvenciája éppen egybeesik a hálózat frekvenciájával, ami minimális eltérés esetén is jelentős kilengésekhez vezet az áram és feszültség tekintetében. Emiatt a fázisjavítás célja sosem az 1 hanem egy ahhoz közeli érték elérése.

### Javítása kondenzátorral

A fáziseltolódáson az áramkörbe kapcsolt ún. fázisjavító [kondenzátorral](https://hu.wikipedia.org/wiki/Kondenz%C3%A1tor_\(elektronika\) "Kondenzátor (elektronika)") segítenek. Ennek (vagy ezeknek) a hatására az áram sietni fog a feszültséghez képest, ami azt eredményezi, hogy az induktív tagok miatt az áram feszültséghez viszonyított késése kisebb lesz. Ennek révén a bezárt szög ( φ ![{\displaystyle \varphi }](https://wikimedia.org/api/rest_v1/media/math/render/svg/33ee699558d09cf9d653f6351f9fda0b2f4aaa3e) ) csökken, közelít a φ = 0 ![{\displaystyle \varphi =0}](https://wikimedia.org/api/rest_v1/media/math/render/svg/192287b02f5764a18fe39f37b8199d72000aa220) értékhez, így a cos ⁡ φ = 1 ![{\displaystyle \cos \varphi =1}](https://wikimedia.org/api/rest_v1/media/math/render/svg/edb888b236ece183bf12d2d1e14d001fe526979f) értékhez.

---
# Coils (Inductors) and Capacitors in Series and Parallel — Full Notes

---

## 1. Basic Definitions

### Capacitor (C)

Stores energy in an electric field.

* Capacitance:
  $C = \frac{Q}{V}$
* Reactance (opposition to AC):
  $X_C = \frac{1}{2 \pi f C}$

### Inductor (L)

Stores energy in a magnetic field.

* Inductance:
  $v = L \frac{di}{dt}$
* Reactance:
  $X_L = 2 \pi f L$

---

## 2. Series & Parallel Combinations

### 2.1 Capacitors

* **Series**
  $\frac{1}{C_{\text{eq}}} = \frac{1}{C_1} + \frac{1}{C_2} + \cdots$

  * Total capacitance decreases.

* **Parallel**
  $C_{\text{eq}} = C_1 + C_2 + \cdots$

  * Total capacitance increases.

### 2.2 Inductors

* **Series**
  $L_{\text{eq}} = L_1 + L_2 + \cdots$

  * Total inductance increases.

* **Parallel**
  $\frac{1}{L_{\text{eq}}} = \frac{1}{L_1} + \frac{1}{L_2} + \cdots$

  * Total inductance decreases.

---

## 3. Resonance & Impedance in LC Networks

When inductors and capacitors are combined, they create frequency-selective circuits.

### Series Resonance (L and C in series)

* Resonant frequency:
  $f_0 = \frac{1}{2 \pi \sqrt{LC}}$
* At $f_0$, impedances cancel:
  $X_L = X_C$
* The total impedance is minimal (limited only by small resistive losses).

### Parallel Resonance (L and C in parallel)

* Resonant frequency is the same:
  $f_0 = \frac{1}{2 \pi \sqrt{LC}}$
* At $f_0$, net susceptance is zero:
  $\frac{1}{X_L} + \frac{1}{X_C} = 0$
* The impedance peaks — the circuit behaves like an open circuit at resonance.

---

## 4. Performance Parameters & Loss Mechanisms

### 4.1 Quality Factor (Q)

Quality factor measures how "lossy" or "selective" a component is.

#### Capacitor:

$Q_C = \frac{X_C}{R_{\text{ESR}}}$

#### Inductor:

$Q_L = \frac{X_L}{R_{\text{DC}} + R_{\text{AC}}}$

* High $Q$ means lower loss and sharper resonance.
---

## 6. Free Online Resources

| Platform                     | Coverage                                                                    | Link                                                                                                        |
| ---------------------------- | --------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------- |
| **Khan Academy**             | Fundamentals of capacitors and inductors, simple RC/LC circuits             | [Khan Academy Electrical Engineering](https://www.khanacademy.org/science/electrical-engineering)           |
| **All About Circuits**       | In-depth tutorials on L, C, R, series/parallel, resonance, practical design | [All About Circuits - AC](https://www.allaboutcircuits.com/textbook/alternating-current/)                   |
| **MIT OpenCourseWare**       | Full electronics course with lecture videos, notes                          | [MIT OCW Circuits and Electronics](https://ocw.mit.edu/courses/6-002-circuits-and-electronics-spring-2007/) |
| **HyperPhysics**             | Visual maps on series/parallel formulas, resonance, Q factor                | [HyperPhysics](http://hyperphysics.phy-astr.gsu.edu/hbase/electric/seri.html)                               |
| **Electronics-Tutorials.ws** | Worked examples, formulas, interactive diagrams                             | [Electronics Tutorials - LC Oscillator](https://www.electronics-tutorials.ws/oscillator/lc-oscillator.html) |

---

Here’s a self‑contained sample problem in English, with a step‑by‑step solution. All math is formatted for Obsidian (you can copy–paste directly).

---

## Sample Exercise

A series R–L–C circuit is connected to a sinusoidal AC source of $V_{\text{rms}} = 230\ \text{V}$ at $f = 50\ \text{Hz}$. The components are:

* $R = 40\ \Omega$
* $L = 100\ \text{mH}$
* $C = 50\ \mu\text{F}$

1. Calculate the inductive reactance $X_L$ and capacitive reactance $X_C$.
2. Find the total impedance $Z$ (magnitude and phase angle $\phi$).
3. Determine the circuit current $I_{\text{rms}}$.
4. Compute the apparent power $S$, active (real) power $P$, and reactive power $Q$.
5. What value of capacitance $C_{\text{new}}$ (in $\mu\text{F}$) would be required (in parallel with the existing $C$) to correct the power factor to unity?

---

## Solution

### 1. Reactances

Angular frequency:

$$
\omega = 2\pi f = 2\pi\cdot50 = 100\pi\ \text{rad/s}
$$

Inductive reactance:

$$
X_L = \omega L = 100\pi \times 0.1 = 10\pi\ \Omega \approx 31.42\ \Omega
$$

Capacitive reactance:

$$
X_C = \frac{1}{\omega C} = \frac{1}{100\pi \times 50\times10^{-6}}
= \frac{1}{0.005\pi} = \frac{200}{\pi}\ \Omega \approx 63.66\ \Omega
$$

---

### 2. Total Impedance

In a series R–L–C:

$$
Z = R + j(X_L - X_C) = 40 + j\bigl(10\pi - \tfrac{200}{\pi}\bigr)\ \Omega
$$

Numeric difference:

$$
X_L - X_C \approx 31.42 - 63.66 = -32.24\ \Omega
$$

$$
Z \approx 40 - j\,32.24\ \Omega
$$

Magnitude:

$$
|Z| = \sqrt{40^2 + (-32.24)^2} \approx \sqrt{1600 + 1039} = \sqrt{2639} \approx 51.37\ \Omega
$$

Phase angle (current lags if positive inductive, here net capacitive so current leads):

$$
\phi = \arctan\!\bigl(\tfrac{\Im Z}{\Re Z}\bigr)
= \arctan\!\bigl(\tfrac{-32.24}{40}\bigr) \approx -38.8^\circ
$$

---

### 3. Circuit Current

$$
I_{\text{rms}} = \frac{V_{\text{rms}}}{|Z|}
= \frac{230}{51.37} \approx 4.48\ \text{A}
$$

---

### 4. Powers

**Apparent power**

$$
S = V_{\text{rms}}\;I_{\text{rms}}
= 230 \times 4.48 \approx 1030\ \text{VA}
$$

**Active (real) power**

$$
P = S\cos\phi = 1030 \times \cos(-38.8^\circ) \approx 1030 \times 0.78 = 803\ \text{W}
$$

**Reactive power**

$$
Q = S\sin\phi = 1030 \times \sin(-38.8^\circ) \approx 1030 \times (-0.63) = -649\ \text{VAR}
$$

(The negative sign indicates net capacitive reactive power.)

---

### 5. Power‑Factor Correction

To achieve unity power factor, we need to cancel the net reactive power $Q$ by adding a capacitor whose reactive power $Q_C$ equals $+649\ \text{VAR}$.

Required capacitive reactance:

$$
Q_C = V_{\text{rms}}^2\,\omega C_{\text{add}}
\quad\Longrightarrow\quad
C_{\text{add}} = \frac{Q_C}{V_{\text{rms}}^2\,\omega}
$$

Plugging in (using $Q_C = 649$ VAR):

$$
C_{\text{add}} = \frac{649}{230^2 \times 100\pi}
= \frac{649}{52900\,\pi}
\approx \frac{649}{166182}
\approx 3.90\times10^{-3}\ \text{F}
= 3900\ \mu\text{F}
$$

Since you already have $50\ \mu\text{F}$, you’d add about $3850\ \mu\text{F}$ in parallel.

---
