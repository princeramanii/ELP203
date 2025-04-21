
# Comprehensive Guide to Electrical Machines Laboratory Experiments

This guide provides detailed information on conducting electrical machine experiments from the laboratory manual. Each experiment includes theoretical background, procedural steps, circuit diagrams, and data collection methods.

## Cycle I: Experiment 1 - Steady-state Performance of a 1-phase Transformer

### Theoretical Background

Transformers are essential devices that transfer electrical energy between circuits through electromagnetic induction. They're crucial in power systems for voltage transformation between generation, transmission, and distribution levels. The equivalent circuit of a single-phase transformer can be represented as shown in Fig. 1.1, with parameters:

- R₀ and X₀: Account for no-load current components (determined by O.C. test)
- R₁ and X₁: Represent winding impedances (determined by S.C. test)

These parameters allow calculation of efficiency, regulation, and expected temperature rise under actual load conditions with minimal power wastage.

### Equipment Required

- One 1-phase transformer (under test)
- One 1-phase auto-transformer
- One low PF and one UPF wattmeter
- Two AC ammeters
- Two AC voltmeters or multimeter


### Procedure and Circuit Diagrams

#### 1. Open Circuit (O.C.) Test

This test determines core loss parameters (R₀ and X₀).

**Circuit Diagram:** Connect as shown in Fig. 1.3 with LV side energized and HV side open.

**Procedure:**

1. Apply rated voltage V₀ to the LV side
2. Record power input (W₀) and current drawn (I₀)
3. Repeat for different input voltages below rated value
4. Tabulate readings as shown in Table 1.1

#### 2. Short Circuit (S.C.) Test

This test determines winding impedance parameters (R₁ and X₁).

**Circuit Diagram:** Connect as shown in Fig. 1.4 with HV side energized and LV side short-circuited.

**Procedure:**

1. Apply voltage (Vsc) to achieve rated current (Isc)
2. Record power input (Wsc)
3. Repeat for different short circuit currents below rated value
4. Tabulate readings as shown in Table 1.2

### Data Processing

1. **Calculate Losses:**
    - Iron loss (at rated voltage) from O.C. test
    - Full load copper loss from S.C. test
2. **Plot Graphs:**
    - I₀ vs. V₀
    - W₀ vs. V₀
    - Isc vs. Vsc
    - Wsc vs. Vsc
3. **Calculate Equivalent Circuit Parameters:**
From O.C. test:
    - No-load PF (cos φ₀) = W₀/(V₀I₀)
    - Active component: Iw = I₀cos φ₀
    - Reactive component: Iμ = I₀sin φ₀
    - R₀ = V₀/Iw
    - X₀ = V₀/Iμ

From S.C. test:
    - Total impedance: Z₂ = Vsc/Isc
    - Total resistance: R₂ = Wsc/Isc²
    - Total reactance: X₂ = √(Z₂² - R₂²)
    - Referred to LV side: R₁ = R₂(N₁/N₂)², X₁ = X₂(N₁/N₂)²
4. **Calculate Efficiency and Regulation:**
    - Efficiency at any load (x times full load) at given PF:
η = Output/(Output + Losses) = Output/(Output + Wi + Wcu)
    - Percentage regulation at full load at given PF:
% regulation = r·cos φ ± x·sin φ
(+ for lagging PF, - for leading PF)

## Cycle I: Experiment 2 - Parallel Operation of Single-phase Transformers

### Theoretical Background

Parallel operation of transformers is used when a single transformer is insufficient to handle increased load demands. Two transformers can be connected in parallel to supply a common load, sharing it between them.

For satisfactory parallel operation, transformers should have:

1. Same voltage ratio
2. Same polarities
3. Same per unit (or percentage) impedances
4. Same phase sequence (in 3-phase case) and zero relative phase displacement

The load sharing between transformers depends on their impedances. With equal per unit impedances, the currents carried by two transformers are proportional to their ratings.

### Equipment Required

- Two single-phase transformers
- Measuring instruments (voltmeters, ammeters, wattmeters)
- Variac
- Loads


### Procedure and Circuit Diagrams

**Circuit Diagram:** Connect as shown in Fig. 2.1

**Procedure:**

1. Before connecting secondaries in parallel, check polarity:
    - Connect primaries to the same single-phase supply
    - Connect secondaries in series
    - Measure voltage across unconnected terminals
    - If voltage is double the expected secondary voltage, terminals have same polarity
    - If voltage is zero, terminals have opposite polarity
2. For parallel operation:
    - Connect terminals of same polarity together
    - Set variac to minimum output position
    - Switch on 1-phase supply
    - Increase variac to get rated voltage
    - Check voltmeter across switch reads zero, then close switch
    - If voltmeter doesn't read zero, interchange terminals of one transformer's secondary
3. Load testing:
    - Apply load in steps
    - Record current, voltage, power from primaries of both transformers
    - Also record load voltage and current
    - Continue until full rated current is reached
4. Short circuit test:
    - Conduct SC test on each transformer separately
    - Determine their Req, Xeq, and Zeq values

### Data Collection

1. Measure voltage, current, and power for both transformers under different loads
2. Conduct short circuit tests to determine impedance parameters
3. Calculate and compare KVA loads and power factors

### Data Processing

1. Calculate Req, Xeq, and Zeq for both transformers
2. Calculate power factors under different load conditions
3. Verify if theoretical calculations match experimental values
4. Compare load distribution (current, active power, reactive power) with respect to transformer parameters
5. Compare power factors of both transformers

## Cycle I: Experiment 3 - Steady-state Performance of 3-phase Transformer

### Theoretical Background

Three-phase transformers are essential for transforming three-phase power in generation, transmission, and distribution systems. Various connection configurations are possible:

1. **Delta-Delta Connection:**
    - Line voltage ratio equals transformation ratio
    - System can operate at 58% capacity if one transformer fails
    - Favored for voltages below 50 kV
2. **Delta-Star Connection:**
    - Provides higher secondary voltage for transmission
    - Commonly used at generating end of transmission lines
    - Y neutral is generally grounded
3. **Star-Star Connection:**
    - Permits grounding neutral points of both primary and secondary
    - Requires delta-connected tertiary windings when primary neutral isn't connected to source neutral
4. **Star-Delta Connection:**
    - Commonly used at receiving end of high voltage transmission lines
5. **Star-Delta-Star Connection:**
    - Uses tertiary delta as auxiliary winding
    - Helps balance the system under unbalanced loading

### Equipment Required

- Three identical single-phase transformers OR a single 3-phase transformer
- Voltmeters and ammeters
- Three-phase loading devices


### Procedure and Circuit Diagrams

**Circuit Diagram:** Fig. 3.1 shows Y-Y connected three-phase transformer

**Procedure:**

1. Conduct polarity test for all three single-phase transformers
2. Connect primaries and secondaries as shown in Fig. 3.1
3. Connect primary to appropriate three-phase supply
4. Measure open circuit primary and secondary voltages (both line and phase)
5. Connect loads across secondary windings according to ratings
6. Measure relevant currents and powers

### Data Collection

1. Record nameplate ratings
2. For no-load test, record:
    - Primary line and phase voltages
    - Primary line and phase currents
    - Secondary line and phase voltages
3. For load test, record:
    - Primary and secondary line and phase voltages
    - Primary and secondary line and phase currents

### Data Processing

1. Compare observed results with theoretical values from transformer ratings
2. Analyze phase and line currents and voltages for various connection cases

## Cycle I: Experiment 4 - Study of Steady-state Performance of a Separately Excited DC Generator

### Theoretical Background

DC generators continue to find applications despite advantages of AC systems due to their flexibility. The relationship between induced EMF in the armature and excitation current (at rated speed) is known as the open circuit characteristic (OCC) or magnetization characteristic. The terminal voltage vs. load current relationship (at constant excitation and speed) is known as external characteristic.

The OCC shows how field current affects armature EMF, while load characteristics show how terminal voltage varies with load current. In separately excited generators, terminal voltage drops gradually with increasing load due to armature resistance drop and flux reduction from armature reaction.

### Equipment Required

- Separately excited DC motor-generator set
- Two rheostats for field control
- Two DC ammeters
- Two DC voltmeters


### Procedure and Circuit Diagrams

**Circuit Diagram:** Connect as shown in Fig. 4.2

#### 1. Magnetization Characteristics

**Procedure:**

1. Start DC shunt motor using starter and bring to rated speed
2. Keep generator's armature terminals open
3. Set generator field current to zero
4. Increase field current in steps to rated value
5. Record terminal voltage and field current
6. Decrease field current in steps to zero
7. Record corresponding terminal voltage
8. Tabulate data in Table 4.1

#### 2. Load Characteristics

**Procedure:**

1. Set field current to rated value
2. Maintain speed at rated value
3. Note terminal voltage
4. Keep field current and speed constant
5. Record terminal voltage for different load currents (0 to rated)
6. Tabulate data in Table 4.2
7. Measure armature and field winding resistances

### Data Processing

1. Plot magnetizing curve and back EMF constant vs. field current
2. Plot terminal voltage vs. load current
3. From external characteristics, draw internal characteristics
4. Comment on the shape of the graphs

## Cycle I: Experiment 5 - Steady-state Performance of a DC Motor

### Theoretical Background

DC motors are highly controllable, which makes them competitive in adjustable speed industrial drives. The torque (T) and speed (n) of a DC motor are given by:

T = K₁φIa
n = (Vt - IaRa)/(K₂φ)

Where K₁, K₂ are design constants.

Speed control methods include:

1. **Field Excitation Control:**
    - Speed increased by increasing field rheostat resistance (field weakening)
    - Provides constant horsepower drive
    - Best for speeds above base speed
2. **Armature Circuit Resistance Control:**
    - Reduces speed by inserting external resistance in armature circuit
    - Speed varies with load
    - Power loss in external resistor is large
    - Provides constant torque drive
3. **Armature Terminal Voltage Control:**
    - Changes speed with constant excitation
    - Requires auxiliary equipment (rectifier or motor-generator set)
    - Ward-Leonard system provides precise control over wide range

### Equipment Required

- Test DC motor
- Rheostats for field and armature control
- Voltmeters and ammeters
- Loading device - DC generator
- Tachometer


### Procedure and Circuit Diagrams

#### 1. Shunt Field Rheostat Control

**Circuit Diagram:** Connect as shown in Fig. 5.2

**Procedure:**

1. Apply rated voltage and start motor using starter
2. Keep field current at maximum value
3. Gradually increase field resistance
4. Observe speed variation with field current at no load
5. Repeat for various constant loads (0.5 and 1.0 p.u. of armature current)

#### 2. Armature Voltage Control

**Procedure:**

1. Bring motor to rated speed at no load
2. Keep field resistance fixed
3. Gradually vary armature voltage
4. Observe speed variation with armature terminal voltage
5. Repeat for various constant loads

### Data Collection

1. For field rheostat control: Record field current and motor speed at different loads
2. For armature voltage control: Record armature voltage, motor speed, armature current, and voltage across generator at different loads

### Data Processing

1. Draw graphs of speed vs. field current for no load and few loading conditions
2. For armature resistance control:
    - Plot armature voltage vs. speed
    - Plot power loss in resistance vs. speed

## Cycle II: Experiment 1 - Steady-state Performance of a 3-phase Induction Motor

### Theoretical Background

Induction motors consume a large percentage of generated electrical power. Their steady-state performance can be represented by the equivalent circuit in Fig. 1.1, with parameters:

- R₁, X₁: Stator resistance and leakage reactance
- R₂, X₂: Rotor resistance and leakage reactance (referred to stator)
- Xm: Magnetizing reactance
- Rc: Core loss resistance

The developed torque is given by:
T = 3I₂²R₂/(sω) N·m

Where:

- ω = synchronous speed in radians/sec
- s = per unit slip

The torque-speed characteristic (Fig. 1.2) shows stable and unstable operating regions, with key points being starting torque (Ts), pull-out torque (Tm), and full-load torque (Tf).

### Equipment Required

- Three-phase induction motor (cage or wound rotor)
- Three-phase auto transformer
- Measuring instruments (ammeters, voltmeters, wattmeters, tachometer)


### Procedure and Circuit Diagrams

#### 1. Stator Winding Resistance Measurement

**Circuit Diagram:** Connect as shown in Fig. 1.3

**Procedure:**

1. Apply low voltage DC supply
2. Ensure current is below rated value
3. Measure voltage and current to calculate resistance

#### 2. Rotor Winding Resistance Measurement (for slip ring motors)

**Procedure:** Same as stator resistance measurement

#### 3. Light Running (No-Load) Test

**Circuit Diagram:** Connect as shown in Fig. 1.4

**Procedure:**

1. Start motor with reduced voltage
2. Gradually increase to rated voltage
3. For slip-ring motors, short-circuit slip-rings before starting
4. Record voltmeter, ammeter, wattmeter, and tachometer readings at different voltages

#### 4. Blocked Rotor Test

**Procedure:**

1. Keep rotor blocked
2. Record instrument readings for different input currents (0 to 1.5 p.u.)
3. Take average readings if values change with rotor position
4. Be careful not to apply high voltages

### Data Processing

1. Calculate equivalent circuit parameters:
    - From no-load test: Rc and Xm
    - From blocked rotor test: R₁, R₂, X₁, X₂
2. Predict motor performance using:
    - Thevenin's equivalent circuit
    - Circle diagram
    - Computer simulation with performance equations
3. Plot:
    - Torque vs. speed
    - Input current vs. speed
    - Power factor, efficiency, power input, input current vs. power output

## Cycle II: Experiment 2 - Steady-state Performance of a 1-phase Squirrel Cage Induction Motor

### Theoretical Background

Single-phase induction motors are widely used in fractional horsepower applications. Their behavior can be analyzed using double revolving field theory, where a pulsating MMF is resolved into two oppositely rotating MMFs of equal magnitude.

The equivalent circuit (Fig. 2.2) shows:

- Forward impedance Zf and backward impedance Zb
- At no-load (Fig. 2.3) and blocked rotor (Fig. 2.4) conditions

The motor current at any slip s is:
I = V/Ztotal at slip s

The forward and backward torques are:
Tf = I₃²r'/2s (synchronous Watts)
Tb = I₅²r'/2(2-s) (synchronous Watts)

### Equipment Required

- Single-phase induction motor with starting arrangement
- AC and DC ammeters and voltmeters
- Single element wattmeter
- Stroboscope or tachometer
- Rheostat
- Single-phase auto-transformer


### Procedure and Circuit Diagrams

**Circuit Diagram:** Connect as shown in Fig. 2.6

#### 1. Stator Resistance Measurement

**Procedure:**

1. Measure DC resistance of stator winding
2. Calculate effective AC value accounting for skin effect and temperature rise

#### 2. No-Load Test

**Procedure:**

1. Apply 1.2 p.u. voltage to the machine
2. Record current, power, and speed
3. Reduce voltage in steps of 0.2 p.u.
4. Measure corresponding input current, power, and speed

#### 3. Blocked Rotor Test

**Procedure:**

1. Disconnect auxiliary winding
2. Block the rotor
3. Apply voltage to achieve 1.2 p.u. current
4. Record applied voltage and input power
5. Reduce current in steps of 0.2 p.u.
6. Record corresponding voltage and power

#### 4. Direct Load Test

**Procedure:**

1. Load motor with mechanical load or DC dynamometer
2. Start motor and bring to rated speed at normal voltage
3. Gradually increase load from no-load to full-load
4. Measure input current, power, speed, torque, and output power

### Data Processing

1. Calculate impedance parameters of stator and rotor
2. Calculate magnetizing reactance
3. Predict performance characteristics using parameters
4. Plot efficiency, power factor, stator current, input power, speed, and torque vs. output power

## Cycle II: Experiment 3 - Steady-state Performance of a 3-phase Alternator

### Theoretical Background

The voltage regulation of an alternator is the per unit voltage rise at its terminal when a load is removed, with excitation and speed remaining constant. It can be predetermined using the synchronous impedance method.

In this method, armature reaction is expressed as a voltage drop (IaXar), and combined with leakage reactance to form synchronous reactance (Xs = Xl + Xar). The equivalent circuit (Fig. 3.1) and phasor diagram (Fig. 3.2) show the relationship between terminal voltage (V), induced EMF (E), and impedance drops.

### Equipment Required

- Three-phase alternator coupled to DC motor
- Three-phase autotransformer
- AC and DC ammeters
- AC voltmeter
- Wattmeter
- Field control rheostat
- Tachometer


### Procedure and Circuit Diagrams

**Circuit Diagram:** Connect as shown in Fig. 3.4

#### 1. Open Circuit Test

**Procedure:**

1. Start DC motor and adjust to synchronous speed
2. Keeping speed constant, increase alternator field current from zero until saturation
3. Record field current and open circuit armature voltage

#### 2. Short Circuit Test

**Procedure:**

1. Drive alternator at synchronous speed with armature terminals short-circuited
2. Gradually increase field current until full load armature current is achieved
3. Record armature current
4. Keep speed constant at synchronous speed

#### 3. Load Test

**Procedure:**

1. Connect alternator terminals to 3-phase load
2. Start DC motor and bring to synchronous speed
3. Adjust field current for rated terminal voltage
4. Vary load to change alternator current from zero to full-load
5. Record terminal voltage, current, and DC motor input power

#### 4. Armature Resistance Measurement

**Procedure:**

1. Use low voltage DC supply
2. Take effective resistance as 1.5 times DC resistance

### Data Processing

1. Draw open circuit and short circuit characteristics on same graph
2. Calculate synchronous reactance: Zs = OC Voltage/SC Current
3. Calculate Xs = √(Zs² - Ra²)
4. Draw phasor diagram and calculate regulation at rated kVA for different power factors
5. Compare efficiencies and regulations obtained by synchronous impedance method and load test

## Cycle II: Experiment 4 - Synchronization and Steady-state Performance of a 3-phase Synchronous Motor

### Theoretical Background

Synchronous motors can operate at different power factors by varying excitation, which is useful for improving system power factor. The armature current phasor is given by:
I = (V-E)/Za

Where:

- V is applied voltage phasor (constant)
- E is induced EMF phasor (depends on DC excitation)
- Za is synchronous impedance

The motor draws lagging current when under-excited and leading current when over-excited. The plots of armature current vs. field current form "V-curves" (Fig. 4.2).

### Equipment Required

- Synchronous machine coupled to DC machine
- DC/AC ammeters and voltmeters
- Two wattmeters with reversing switch
- Field control rheostats
- Synchronizing board
- Tachometer


### Procedure and Circuit Diagrams

**Circuit Diagram:** Connect as per Fig. 4.3

**Procedure:**

1. Start DC machine as motor and bring to synchronous speed
2. Adjust alternator field current for rated terminal voltage
3. Synchronize alternator to mains using two bright lamp and one dark lamp method
4. Disconnect DC machine from mains
5. With no load on DC generator, adjust alternator field current for minimum armature current (unity PF)
6. Record field current, armature current, and wattmeter readings
7. Vary field current in both directions and record readings
8. When wattmeters kick back, reverse voltage coil and record as negative value
9. Load synchronous motor by connecting load to DC generator
10. Repeat experiment for 25%, 50%, and 100% of full load

### Data Processing

1. Calculate power factor using two wattmeter readings:
tan φ = √3(W₂-W₁)/(W₂+W₁)
2. Plot armature current vs. field current for constant output (V-curves)
3. Plot power factor vs. field current (inverted V-curves)

## Cycle II: Experiment 5 - Steady-state Performance of a 3-phase Variable Frequency Driven Squirrel-cage Induction Motor

### Theoretical Background

Speed control of induction motors is important in many industrial applications. Variable frequency drives (VFDs) provide an effective method of speed control.

The stator voltage can be written as:
Va = (fe/frated) × (Bpeak/Brated) × Vrated

For frequencies below rated frequency, constant flux density operation is maintained by keeping:
Va/fe = Vrated/frated (constant V/f operation)

For frequencies above rated frequency, terminal voltage is kept at rated value, resulting in reduced flux density.

Fig. 5.1 shows typical torque-speed curves with variable frequency drive, while Fig. 5.2 shows constant torque and constant power regions.

### Equipment Required

- Three-phase induction motor coupled to separately excited DC motor
- Variable voltage-variable frequency AC drive
- Wattmeter, ammeter, and voltmeter


### Procedure and Circuit Diagrams

**Circuit Diagram:** Connect as shown in Fig. 5.3

#### 1. No-Load Test

**Procedure:**

1. Apply rated voltage to AC drive using variac
2. Push start button and slowly increase speed controller
3. Record speed, frequency, stator voltage, current, and power factor at different speeds

#### 2. Load Test at 25 Hz

**Procedure:**

1. Switch on field DC supply of separate DC generator
2. Start AC drive and increase speed to 25 Hz
3. Apply load on DC generator step-wise
4. Record results in Table 5.1

#### 3. Load Test at 50 Hz

**Procedure:**

1. Reduce generator load to minimum
2. Increase motor speed to 50 Hz
3. Apply load on DC generator step-wise
4. Record results in Table 5.2

### Data Processing

1. Determine equivalent circuit parameters of induction motor
2. Plot speed, current, power factor, and efficiency vs. output power at 25 Hz and 50 Hz
3. Compute starting torque and current for constant V/f and constant flux operation
4. Plot torque-speed and stator current-speed at different frequencies with constant V/f ratio

This comprehensive guide covers all the experiments in detail. For each experiment, I've included the theoretical background, equipment requirements, procedural steps, circuit diagrams, data collection methods, and data processing techniques. Following these instructions will help you successfully complete all the laboratory experiments.
