

# Main parts (what the symbols mean)

- Top left: the 3-phase supply lines L1, L2, L3 (often written U, V, W or L1,L2,L3). The small boxes in each phase are protective devices (fuses / switches) in the power supply.
    
- Big triple contact blocks (three contacts drawn together) — contactors (power contacts) that switch the three phases. There are separate contactors for the star connection and for the delta connection (and usually a main contactor).
    
- MVK (the labelled box): the motor controller/timer (in Hungarian: _motor vezérlő_), which sequences the star → delta change after a preset time.
    
- MK: the magnetic contactor / overload unit. In many drawings MK also includes the thermal overload/relay (a NC contact that opens on overload). The little resistor/zigzag symbol near MK could indicate a heater (thermal element) or internal trip mechanism of the overload relay.
    
- A1 / A2: coil terminals of the contactor (control coil). When A1–A2 is energized the contactor’s power contacts close.
    
- Small NC / NO auxiliary contacts in the control wiring: NC = normally closed, NO = normally open. These are used for stop/start and to interlock contactors.
    
- Bottom-left: the 3-phase motor. Terminals labelled U, V, W (or U1,V1,W1 and U2,V2,W2). The little internal connections drawn show how windings are connected in star or delta.
    
- Control pushbuttons at the right: “piros” (red) = STOP (normally-closed NC pushbutton), “zöld” (green) = START (NO pushbutton).
    

# What the starter does (purpose)

- **Star (Y) start**: motor windings are connected in star so each winding sees line voltage / √3 (reduced voltage). That lowers starting current and starting torque, making the motor start softly.
    
- **Switch to delta** after the motor reaches a certain speed (after a timer delay): windings are reconnected in delta so each winding sees full line voltage and motor runs at full torque.
    

# How the wiring / sequence works (step-by-step)

1. **Power and stop circuit**
    
    - The 3-phase supply L1/L2/L3 is present at the top. Control circuit power (a fused small supply) feeds the start/stop loop. The red STOP button is NC in series with the rest of the control circuit — when STOP is pressed the circuit opens and the motor stops.
        
    - The green START button is NO; pressing it momentarily completes the control circuit to energize the appropriate contactor coil.
        
2. **Start (press green)**
    
    - When you press the green (zöld) START, control power flows through the NC STOP button and the MK (overload) NC contact to the start coil (usually the coil of the _star_ contactor or the main contactor that closes the power contacts AND lets the controller begin the star timing).
        
    - The contactor that connects the motor windings in **star** closes its three power contacts, connecting the motor windings to the supply in star (U2/V2/W2 are tied together inside the starter).
        
    - The contactor also typically has an auxiliary NO (self-holding) contact wired in parallel with the green START button so the coil remains energized after you release START (latching). This is visible as an NO contact in the control circuit.
        
3. **Timer / motor controller (MVK)**
    
    - The MVK (motor controller/timer) senses that the star contactor is closed and starts its preset delay. During this delay the motor accelerates with reduced voltage/current.
        
    - The MVK will then command the changeover: it will open the star contactor and close the delta contactor (or operate separate changeover contactors in the correct order). The diagram shows auxiliary NC/NO contacts used to make sure star and delta contactors are not both closed.
        
4. **Star → Delta switching**
    
    - **Always**: the star contactor is opened first, then after a very short time the delta contactor is closed. This prevents a dead short between windings. The controller either uses built-in sequencing or external interlocking contacts to enforce this.
        
    - When the delta contactor closes the motor windings are reconnected in delta (U1→V2, V1→W2, W1→U2 typical), so each winding sees full line voltage and the motor runs at full torque.
        
5. **Running / stopping**
    
    - In the running (delta) state the controller holds the delta contactor closed. Pressing the red STOP button breaks control power (it opens the NC stop contact) and all contactor coils de-energize — main power contacts open and the motor stops.
        
    - If the thermal overload (MK overload) trips it opens its NC contact in the control circuit and de-energizes the coils, stopping the motor. The overload may need manual reset.
        

# Interlocks and safety features in the diagram

- **Electrical interlocks**: you can see NC auxiliary contacts of each power contactor placed into the coil circuit of the opposing contactor. That ensures star and delta cannot be energized simultaneously.
    
- **Mechanical interlocks** (often present in real contactors): provide a hard mechanical block so both star and delta contacts cannot close at the same time, preventing phase shorting.
    
- **Overload relay (a thermal NC contact)** in series with the coil circuit — opens on overload and protects the motor.
    
- **Fuses / circuit breaker** on the power phases protect wiring and contactor contacts.
    

# Labels / Hungarian words decoded

- **piros** = red (STOP button) — normally closed.
    
- **zöld** = green (START button) — normally open.
    
- **NC** = Normally Closed contact. **NO** = Normally Open contact.
    
- **MK** = mágneskapcsoló / motor kontaktor (magnetic contactor / includes overload in the drawing).
    
- **MVK** = motor vezérlő / motorvezérlő kapcsoló (motor controller / timer for star→delta).
    
- **A1 / A2** = coil terminals for contactor.
    

# Why use this arrangement?

- It’s a simple way to reduce starting current and mechanical stress for medium/large motors: start in **star** (reduced voltage) to limit inrush, then switch to **delta** for full power. Common on motors where a full-voltage starter would produce too much current or harsh mechanical shock.
    

# Practical cautions / commissioning notes

- Make sure the interlock contacts or mechanical interlock are present and functioning — simultaneous star & delta = short circuit.
    
- Control circuit fusing and coil voltage must match the diagram (use the small control fuse shown).
    
- Timer delay should match the motor’s acceleration time — too short can stall, too long prolongs reduced torque.
    
- Overload relay must be adjusted to motor full-load current rating.
    
- When testing, watch for mechanical latching (the auxiliary NO that latches the start) and verify STOP breaks the latch.
    

---

If you want, I can:

- redraw a clean annotated version of this specific diagram labeling each wire and terminal (U1/U2 etc.), or
    
- map exact terminal connections for star and delta (which motor terminal goes to which contactor terminal), or
    
- explain how to set the overload relay and timer values for a specific motor (you’d give motor nameplate current and supply voltage).
    

Which would help you most?