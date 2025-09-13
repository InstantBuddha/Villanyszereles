### AC (Alternating Current) Utilization Categories

#### Short version:
You are right to ask for clarification, as the initial list provided only the most common AC categories for main power circuits. The full IEC classification system is much more extensive and is broken down further based on the type of device (e.g., contactors, circuit breakers, relays) and the application.

Here's a more comprehensive look at the AC categories, along with some real-world examples to illustrate the differences in amperage ratings.

### AC Categories - A More Complete Picture

The IEC 60947 series of standards defines a range of utilization categories for different types of switchgear and controlgear. The number in the category often corresponds to the device type:

* **AC-1 through AC-8:** These are the primary categories for **contactors and starters** used in main power circuits.
* **AC-12 through AC-15:** These are for **auxiliary contacts and control relays** in control circuits, which handle smaller currents.
* **AC-20 through AC-23:** These are for **switches and disconnectors**, which are designed to switch currents under different load conditions, including overloads.

The categories you most commonly encounter for main power switching are still AC-1, AC-3, and AC-4, but many others exist for specific applications:

* **AC-1 (Non-Inductive/Slightly Inductive Loads):** For applications like heaters, ovens, and lighting circuits where the power factor is high ($\cos\phi \ge 0.95$).
* **AC-3 (Squirrel-Cage Motors, Normal Operation):** The most common category for motor control, where the switch makes the starting inrush current but breaks the normal running current.
* **AC-4 (Squirrel-Cage Motors, Severe Duty):** For applications with frequent jogging or plugging, where the switch must make and break the high starting current repeatedly.
* **AC-5a (Discharge Lamps) & AC-5b (Incandescent Lamps):** For switching lighting loads with their unique inrush and operating characteristics.
* **AC-6a (Transformers) & AC-6b (Capacitor Banks):** For highly specialized applications where a device must handle the very high inrush currents associated with these loads.
* **AC-7a (Slightly Inductive Household Appliances) & AC-7b (Motor Loads for Household Appliances):** For applications in residential and small commercial settings.
* **AC-8a & AC-8b (Hermetic Refrigerant Compressor Motors):** For HVAC and refrigeration systems where the motor is hermetically sealed and the thermal behavior is a primary concern.

### Amperage Examples: AC-1 vs. AC-3

A single switch or contactor will almost always have different rated currents for different utilization categories. The rating in the most demanding category (e.g., AC-4) will be significantly lower than the rating in the least demanding category (e.g., AC-1).

Let's use a real-world example from a major electrical component manufacturer like Schneider Electric. Consider a common industrial contactor, such as the **LC1D25**.

* **AC-1 Rating:** For non-inductive or slightly inductive loads, this contactor is typically rated for **40A**. This is its maximum current handling capacity for a "simple" resistive load.
* **AC-3 Rating:** For controlling a squirrel-cage motor, the same contactor is rated for **25A**. This is a significant reduction.



These categories apply to AC contactors and relays for controlling power circuits.

- **AC-1: Non-inductive or Slightly Inductive Loads**
    
    - **Load Type:** This is the simplest category. It covers loads where the power factor (cosϕ) is greater than or equal to 0.95. This includes purely resistive loads and loads with very little inductance.
        
    - **Application Examples:** Resistive furnaces, heaters, distribution circuits, and incandescent lighting (though there are more specific categories for this).
        
    - **Operation:** Switching on and off of the load at its rated current. There are no significant inrush currents or high-voltage arcs to contend with, so the switching device is subjected to the least amount of stress. This is often the highest current rating for a given switch.
        
- **AC-2: Slip-ring Motors**
    
    - **Load Type:** Slip-ring motors. These motors are less common in modern industrial applications than squirrel-cage motors.
        
    - **Operation:** The switch must make the starting current, which is typically about 2.5 times the motor's rated current. On opening, it must break the starting current at a voltage that is less than or equal to the main supply voltage. This is a more difficult operation than AC-1 due to the inductive nature and starting current.
        
- **AC-3: Squirrel-cage Motors**
    
    - **Load Type:** The most common type of industrial motor, the squirrel-cage motor.
        
    - **Operation:** The switch makes (closes) the circuit to start the motor, which involves a high inrush current (typically 5 to 7 times the rated running current). The switch then breaks (opens) the circuit when the motor is running at full speed. At this point, the current is only the motor's rated current, and the voltage across the contacts as they open is relatively low. This is a common and moderately severe duty cycle.
        
    - **Application Examples:** Pumps, fans, compressors, conveyors, and elevators.
        
- **AC-4: Squirrel-cage Motors with "Plugging" and "Inching"**
    
    - **Load Type:** Squirrel-cage motors.
        
    - **Operation:** This is the most demanding category for AC motor control. It includes "plugging" (rapidly reversing the motor by reversing the primary connections while it's still running) and "inching" (frequent, short-duration starts and stops to achieve small movements). In these operations, the switch must make and break the high starting current multiple times, and the voltage across the contacts can be much higher as the motor's back EMF adds to the supply voltage. The electrical and mechanical stress on the contacts is extremely high.
        
    - **Application Examples:** Cranes, hoists, wire drawing machines, and other applications requiring rapid and precise motor control.
        
- **AC-5a: Switching of Electric Discharge Lamps**
    
- **AC-5b: Switching of Incandescent Lamps**
    
    - **Load Type:** Lighting loads.
        
    - **Operation:** These categories are for specific types of lighting with distinct electrical characteristics. For example, incandescent lamps have a very low cold resistance, leading to a high inrush current when switched on. Electric discharge lamps (like fluorescent lights) have complex electrical behavior and often use ballasts that can be either inductive or capacitive.
        
- **AC-6a: Switching of Transformers**
    
- **AC-6b: Switching of Capacitor Banks**
    
    - **Load Type:** Transformers and capacitor banks.
        
    - **Operation:** These are very specific and difficult loads. When a switch closes on an unenergized transformer, it can experience a very high magnetic inrush current. Switching capacitor banks results in an extremely high, instantaneous capacitive inrush current as the capacitors charge. These operations require robust switching devices specifically designed to handle these surges.