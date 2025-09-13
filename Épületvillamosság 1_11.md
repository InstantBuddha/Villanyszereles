## Kismegszakitók

In Europe, miniature circuit‑breakers (MCBs) are classified by their instantaneous (magnetic) tripping characteristics into Types A, B, C and D per IEC/EN 60898‑1. The key difference lies in the multiple of rated current (In) at which the breaker will trip almost instantaneously (typically <100 ms), which determines how tolerant it is of inrush currents:

| **Type** | **Instantaneous trip** | **Characteristics**                                            | **Typical use cases**                                                                                                                                                        |
| -------- | ---------------------- | -------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **A**    | 2–3 × In               | *Very* sensitive to surges. Includes semiconductor protection. | Sensitive electronics and control circuits (e.g. PLCs, low‐power semiconductor devices)                                                                                      |
| **B**    | 3–5 × In               | Standard “general‑purpose” breaker.                            | Domestic lighting and socket circuits; small resistive loads (fridges, washing machines)<br>Hőtermelő berendezések, Bojler, tűzhely, sütő és általános háztartási dugalj     |
| **C**    | 5–10 × In              | Handles moderate inductive inrush.                             | Commercial and light‑industrial: small motors (pumps, fans), fluorescent lighting, HVAC units<br>Bekapcsoláskor jelentős áramugrás tapasztalható<br>Indukciós főzőlap, klíma |
| **D**    | 10–20 × In             | Lets very high surges pass.                                    | Heavy industrial equipment: large motors, transformers, welding machines, UPS inrush                                                                                         |

---
Itt az alsó értékeknél a bimetál csap le, a felső értéknél meg az elektromágnes.

| **Type** | **Instantaneous trip** | **10A**  | **16A**  |
| -------- | ---------------------- | -------- | -------- |
| **A**    | 2–3 × In               | 20-30A   | 32-48A   |
| **B**    | 3–5 × In               | 30-50A   | 48-80A   |
| **C**    | 5–10 × In              | 50-100A  | 80-160A  |
| **D**    | 10–20 × In             | 100-200A | 160-320A |

---

| **A**      | **vezeték**   | **plusz info**                                       |
| ---------- | ------------- | ---------------------------------------------------- |
| (1)        | $1.5mm^2$     |                                                      |
| 2          | $1.5mm^2$     |                                                      |
| 4          | $1.5mm^2$     |                                                      |
| 6          | $1.5mm^2$     |                                                      |
| (8)        | $1.5mm^2$     |                                                      |
| 10         | $1.5mm^2$     |                                                      |
| ==**13**== | ==$1.5mm^2$== | ==Átlag háztartásba elég==                               |
| 16         | $2.5mm^2$     | Ha messze van a fogyasztó                            |
| 20         | $4mm^2$       |                                                      |
| 25         | $6mm^2$       |                                                      |
| ==**32**== | ==$10mm^2$==  | ==Mérőtől az elosztóig is $10mm^2$-el KELL behozni== |
| 40         |               |                                                      |
| 50         | $16mm^2$      |                                                      |
| 63         | $25mm^2$      |                                                      |

---

### How it works

1. **Thermal trip** (overload protection): a bimetallic strip heats up under moderate overcurrents and bends to trip the breaker (same mechanism for all types).
2. **Magnetic trip** (short‑circuit protection): an electromagnet instantly plucks the trip lever when fault current exceeds the type’s instantaneous threshold (e.g. 5×In for Type C).

Selecting the right type prevents nuisance tripping on inrush currents while still safeguarding against damaging short circuits.

---

### Choosing the right type

* **Type A**: Rare in power distribution; used when you need extra sensitivity or to protect semiconductor loads (e.g. power supplies, sensitive instrumentation) ([ifixit.com][1]).
* **Type B**: Default for most homes and light commercial installations; trips quickly on genuine faults but may nuisance‑trip on larger motor starts.
* **Type C**: The workhorse for commercial/industrial settings with moderate inductive loads; strikes a balance between immunity to start‑up inrush and rapid fault clearing.
* **Type D**: Specialized industrial use where extremely high start‑up currents occur (e.g. welding, large transformers), ensuring the breaker only trips on true faults.

By matching the breaker’s magnetic trip curve to your load’s inrush profile, you ensure both safety and continuity of service.

![[Pasted image 20250707142953.jpg]]
    1. Actuator lever - used to manually trip and reset the circuit breaker. Also indicates the status of the circuit breaker (On or Off/tripped). Most breakers are designed so they can still trip even if the lever is held or locked in the "on" position. This is sometimes referred to as "free trip" or "positive trip" operation.
    2. Actuator mechanism - forces the contacts together or apart.
    3. Contacts - Allow current when touching and break the current when moved apart.
    4. Terminals
    5. Bimetallic strip
    6. Calibration screw - allows the manufacturer to precisely adjust the trip current of the device after assembly.
    7. Solenoid
    8. Arc divider / extinguisher

---
![[Pasted image 20250708222527.jpg]]
This plot is the classic “time–current characteristic” chart for miniature circuit‑breakers (MCBs) of types B, C and D.  Here’s how to read it:

---

### 1. Axes

* **Horizontal axis**: the multiple of the breaker’s rated current, $I/I_n$.

  * At $I/I_n=1$ you’re at the nominal (continuous) current rating.
  * As you move right, you’re looking at fault or overload currents that are 2×, 5×, 10×, etc. the breaker’s rating.

* **Vertical axis**: the time in seconds (log scale) it takes the breaker to open.

  * At the top (10 000 s ≈ 3 hours) you see how long the breaker can sustain a very slight overload (just above 1 × In).
  * Down at 0.01 s you see how quickly it will clear a heavy short‑circuit.

---

### 2. Two parts of the trip‑curve

1. **Thermal (long‑time) portion** (the wide “inverse‑time” curve rising steeply on the left):

   * Governs protection against sustained overloads (e.g. 1.1…1.5 × In).
   * At 1.13 × In it may take up to about an hour to trip, at 1.45 × In maybe only a few minutes.

2. **Magnetic (short‑time/instantaneous) portion** (the almost‐vertical “bar” on the right of each shaded region):

   * Governs protection against short circuits or high inrush currents.
   * It “instant‑trips” if the fault current exceeds a specified multiple of In.

---

#### Why choose one type over another?

* You always size the breaker so that normal start‑up currents stay **below** its instantaneous threshold (so it doesn’t nuisance‑trip),
* …but any **fault currents** (e.g. a dead short) exceed the threshold by a large margin, so the breaker opens very quickly and protects the wiring.

Thus by selecting B, C or D you tailor the breaker to the expected inrush profile of your load.

[szelektivitás](https://assets.legrand.com/pim/NP-FT-GT/EXB15015_TG_Coordination_EN.pdf?utm_source=chatgpt.com)