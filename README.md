final # Open Design and Technology  
## Final Project README

> **Project Weight:** 70%  
> **Team Size:** 2 students  
> **Project Duration:** 4 weeks  
> **Class Time Available:** 6 hours per class  
> **Total Time Available:** 48 effort-hours per team  
> **Project Type:** Playful, interactive, technology-based experience

---

# Before you begin

## Fork and rename this repository
After forking this repository, rename it using the format:

`ODT-2026-TeamName`

### Example
`ODT-2026-PixelWizards`

Do not keep the default repository name.

---

# How to use this README

This file is your team’s **working project document**.

You must keep updating it throughout the 4-week build period.  
By the final review, this README should clearly show:
- your idea,
- your planning,
- your design decisions,
- your technical process,
- your build progress,
- your testing,
- your failures and changes,
- your final outcome.

## Rules
- Fill every section.
- Do not delete headings.
- If something does not apply, write `Not applicable` and explain why.
- Add images, screenshots, sketches, links, and videos wherever useful.
- Update task status and weekly logs regularly.
- Use this file as evidence of process, not only as a final report.

---

# 1. Team Identity

## 1.1 Studio / Group Name
`[Bubble]`

## 1.2 Team Members

| Name | Primary Role | Secondary Role | Strengths Brought to the Project |
|---|---|---|---|
| `[Hemadri Mohta]` | `[ Coding / Fabrication / Circuit Making]` | `[Model Making]` | `[Coding]` |
| `[Aryaa Parmar]` | `[Model Making / Circuit Making]` | `[Coding]` | `[Product Making]` |

## 1.3 Project Title
`[Bubble Maker]`

## 1.4 One-Line Pitch
`[Pop-up your childhood]`

## 1.5 Expanded Project Idea
In 1–2 paragraphs, explain:
- what your project is,
- what kind of playful experience it creates,
- what makes it fun, curious, engaging, strange, satisfying, competitive, or delightful,
- what technologies are involved.

**Response:**  
`Our project is an interactive bubble-making machine. This project uses servo motor which controls the ring to move in an out of the soup solution, while DC motor works as a fan to generate airflow for forming bubbles. The system is programmed so that the fan speed of the DC motor responds to the angle of the servo motor, slow when the ring is dipped in the solution and rising and fast when it reaches the optimal position for bubble formation. The users interact with this through the buttons that allow them to manually control the movement for the ring.
The playful experience comes from the balance between control and surprise. While the user actively decides when and how the ring moves, the actual formation of bubbles feels slightly unpredictable and satisfying—sometimes producing perfect bubbles, sometimes none at all. This creates a sense of curiosity and experimentation, encouraging users to explore timing, positioning, and rhythm. It is engaging because it transforms a simple childhood activity into a responsive, interactive system, using technologies like MicroPython on ESP32, PWM motor control, serco motor operation, and user input through buttons.`

---

# 2. Philosophy Fit

## 2.1 Experience, Not Social Problem
This module does **not** require your project to solve a large social problem.

You are allowed to build:
- toys,
- games,
- interactive objects,
- playful machines,
- kinetic artifacts,
- humorous devices,
- strange but delightful experiences,
- things that are entertaining to use or watch.

## 2.2 What kind of experience are you creating?
Answer the following:
- What is the experience?
- What do you want the player or participant to feel?
- Why would someone want to try it again?

**Response:**  
`-The experience is of interacting with a bubble-making machine where the user controls the motion using buttons. You press to move the ring down into the soap and bring it back up, and at the same time the fan responds to that movement to try and form a bubble. You’re not just watching it happen, you’re kind of “operating” it and figuring out the right timing and position to get a good bubble.
-We want the players to feel satisfied about getting the timing right and seeing a clean bubble form, but it doesn’t happen perfectly every time, which makes it a bit playful and curious.
-You start experimenting with how fast to press, how high to lift the ring, or when to pause.`

## 2.3 Design Persona
Complete the sentence below:

> We are designing this project as if we are a small creative studio making a **[toy / game / playable object / interactive experience]** for **[children / teens / adults / classmates / exhibition visitors / mixed audience]**.

**Response:**  
`We are designing this project as if we are a small creative studio making a playful interactive installation for a mixed audience of classmates and exhibition visitors, where users actively control the creation of bubbles through simple physical inputs.`

---

# 3. Inspiration

## 3.1 References
List what inspired the project.

| Source Type | Title / Link | What Inspired You |
|---|---|---|
| `Toy` | `Automatic Bubble Machine Toy (generic bubble blower)` | `Inspired the basic idea of dipping a ring into soap solution and using airflow to create bubbles automatically.` |
| `Object` | `Handheld Bubble Wand` | `Gave insight into how bubble rings need to be dipped fully and then exposed to airflow at the right moment to form bubbles.` |
| `Video` | `“Arduino Bubble Machine using Servo and DC Motor” (YouTube)` | `Helped understand how to synchronize a servo motor movement with a fan/motor to generate bubbles efficiently.` |

## 3.2 Original Twist
What makes your project original?

**Response:**  
`So what really makes our bubble machine different? For starters, it’s not just a simple on/off gadget spinning all day. We actually gave the hardware some “real conversation” every part works together, and the microcontroller keeps everything in sync, mechanics and electronics teaming up. Most bubble machines? They just run a motor on a timer, or expect you to crank a handle. Ours is on another level. Here’s where things get cool: the fan’s speed changes based on exactly what the servo arm is doing at that moment. The microcontroller always knows where the bubble ring sits during each cycle. When the ring dips into the soap, the fan cuts out completely. As it comes up, the fan starts to spin. Once the ring’s out and ready, the fan blasts at full power. No wasted air, no guessing it’s like the machine has a mini brain, making decisions every step instead of just repeating itself like a robot. We didn’t want it totally hands-off, either. We put in two simple buttons so you can move the servo arm yourself set the pace however you want. Maybe sometimes you want a fast dip and a quick burst, or other times you want to slow down and really watch those bubbles build up. The machine actually pays attention to you. Instead of copying those basic toys with a spinning wand and constant breeze, we tried to capture the way people actually make bubbles: dip the ring, lift it out, and blow at the perfect moment. The machine kind of acts like you just with a little help from electronics.`

---

# 4. Project Intent

## 4.1 Core Interaction Loop
Describe the main loop of interaction.

Examples:
- press → launch → score → reset
- connect → control → observe → repeat
- turn → trigger → react → repeat
- move object → sensor detects → sound/light response → player reacts

**Response:**  
`button press → servo dips ring → ring rises → fan blows air through soap film → bubble forms → repeat
The core loop is: the user presses a button to move the servo down (dipping the ring in soap), then presses again to bring it back up in front of the fan, which speeds up automatically as the ring rises, blowing air through the soap film to create a bubble. The cycle then resets for the next bubble.`

## 4.2 Intended Player / Audience

| Question | Response |
|---|---|
| Who is this for? | `This is designed for children, students, and casual users who enjoy interactive and playful experiences. It can also be for adults who want to revisit their childhood memories.` |
| Age range | `6–16 years primarily, but enjoyable for all age groups including adults in informal or exhibition settings.` |
| Solo or multiplayer | `Primarily a solo interaction, but can be used in a shared environment where multiple users take turns or collaborate.` |
| Expected duration of one round | `1-3 minutes per interaction, depending on how long the user chooses to engage with the controls and create bubbles.` |
| What should the player feel? | `A sense of curiosity, control, nostalgia and satisfaction. The interaction should feel playful and rewarding, especially when the bubble is successfully formed through their input.` |
| Is explanation required before use? | `Minimal explanation is required. Basic instructions (e.g., “Press buttons to move the ring and create bubbles”) are sufficient, as the system is intuitive and responsive.` |

## 4.3 Player Journey
Describe exactly how a player will use the project.

1. **Approach:** `The player encounters the bubble machine as an interactive setup with a visible ring, fan (DC motor), and two control buttons. The moving parts and soap solution signal that it creates bubbles, inviting interaction.`
2. **Start:** `The system is already powered on, with the ring initially dipped in the soap solution. The player begins by pressing one of the buttons.`
3. **First Action:** `The player presses the “Up” button, causing the servo motor to lift the ring out of the soap solution.`
4. **Main Interaction:** `The player continuously presses the Up and Down buttons to control the height of the ring. They experiment with positioning the ring at different angles to try and create bubbles.`
5. **System Response:** `As the ring rises, the servo motor moves accordingly.
The DC motor (fan) adjusts its speed based on the ring’s height:
Low position → fan off
Mid position → fan slow
High position → fan fast
When the ring reaches the optimal height, the fast हवा flow creates bubbles.`
6. **Win / Lose / End Condition:** `Win condition: A successful bubble is formed when the ring is correctly positioned and airflow is sufficient.
There is no strict lose condition, but incorrect positioning results in no bubble formation.`
7. **Reset:** `The player presses the “Down” button to lower the ring back into the soap solution, re-coating it and preparing for the next attempt.`

## 4.4 Rules of Play
If your project is a game, list the rules clearly.

`Since this project is an interactive bubble-making machine and not a game, the following are the operating rules and guidelines for using the device:`
- `Rule 1: Ensure the soap solution tray is filled before powering on the device, and that the ring is positioned at the minimum angle (0°) so it begins fully submerged in the solution.`
- `Rule 2: Press the Up button to raise the servo motor incrementally (5° per press), lifting the ring out of the soap solution and into the path of the DC motor fan to create bubbles.`
- `Rule 3: Press the Down button to lower the servo motor incrementally (5° per press), re-dipping the ring into the soap solution to reload it for the next bubble cycle.`
- `Rule 4: Do not force the servo beyond its set limits — the ring will automatically stop at the minimum (0°) and maximum (120°) angles to prevent mechanical damage.`

---

# 5. Definition of Success

## 5.1 Definition of “Playable”
Your project will be considered complete only if these conditions are met.

- [ ] `The servo motor reliably moves the ring between the minimum and maximum angles using the two control buttons without jitter or stalling.`
- [ ] `The ring successfully dips into the soap solution and lifts out smoothly, forming a stable soap film at least most of the time.`
- [ ] `The DC motor (fan) changes speed based on the servo angle, with clearly observable OFF, slow, and fast states.`
- [ ] `At higher servo angles, the increased airflow consistently produces visible soap bubbles from the ring.`
- [ ] `The system responds in real-time to user input, allowing continuous interaction (holding or pressing buttons to control bubble generation).`

## 5.2 Minimum Viable Version
What is the smallest version of this project that still delivers the core experience?

**Response:**  
`All you really need is a servo and a standard DC motor. Forget about buttons or fancy features just keep it straightforward. The servo handles dipping the ring into the soap and lifting it up in front of a fan. The fan runs nonstop with the DC motor, so when the ring comes up, bubbles start flying right away.

Nothing complicated here. This simple setup does exactly what you want: dip the ring, lift it, make bubbles. Done.`

## 5.3 Stretch Features
What features are nice to have but not essential?

- `Automatic operation mode – enables continuous bubble generation without manual input, improving usability.`
- `Sensor-based activation – allows touchless operation, enhancing user interaction and efficiency.`
- `User-adjustable fan speed – provides control over bubble size and formation, increasing flexibility.`
- `Smooth servo motion – reduces abrupt movements, improving bubble consistency and mechanical reliability.`
- `LED indicators – offer real-time system feedback, making operation more intuitive.`
- `Calibration mode – allows adjustment of angle thresholds, making the system adaptable to different setups.`
- `Power-saving functionality – reduces energy consumption by turning off components when idle.`
- `Wireless/remote control – enables convenient operation and extends user accessibility.`

---

# 6. System Overview

## 6.1 Project Type
Check all that apply.

- [YES] Electronics-based
- [YES] Mechanical
- [ ] Sensor-based
- [ ] App-connected
- [YES] Motorized
- [ ] Sound-based
- [ ] Light-based
- [ ] Screen/UI-based
- [YES] Fabricated structure
- [ ] Game logic based
- [YES] Installation / tabletop experience
- [ ] Other: `[Write here]`

## 6.2 High-Level System Description
Explain how the system works in simple terms.

Include:
- input,
- processing,
- output,
- physical structure,
- app interaction if any.

**Response:**  
`The system is an interactive bubble-generating device that integrates user input, embedded processing, and coordinated motor control to produce a controlled physical output. User input is provided through two push buttons, which regulate the angular position of a servo motor attached to a ring. The microcontroller continuously processes these inputs and adjusts the servo motor accordingly while simultaneously evaluating the ring’s position against predefined threshold values. Based on this evaluation, the system modulates the speed of a DC motor (fan) using pulse-width modulation, establishing a direct relationship between the servo angle and airflow intensity. The physical structure comprises a servo-driven ring that dips into a soap solution and rises into the path of the fan, a DC motor positioned to generate airflow, and a motor driver to control speed variations. As the ring reaches an optimal height, increased airflow passes through the soap film, resulting in bubble formation. The system operates entirely through physical controls without any application-based interaction, demonstrating the effective synchronization of mechanical movement and electronic control to achieve a functional and responsive output.`

## 6.3 Input / Output Map

| System Part | Type | What It Does |
|---|---|---|
| `Push Buttons (Up & Down)` | Input | `Allow the user to manually control the position of the servo motor by increasing or decreasing its angle in discrete steps.` |
| `ESP32 Microcontroller` | Processing | `Reads button inputs, updates the servo angle, and dynamically controls the DC motor speed based on predefined angle thresholds.` |
| `Servo Motor (Ring Mechanism)` | Output | `Moves the ring between the soap solution and the airflow zone, determining when the bubble film is formed.` |
| `DC Motor with Fan (via L298N Driver)` | Output | `Generates airflow at variable speeds (off, slow, fast) to form bubbles when the ring reaches appropriate positions.` |
| `Ring + Soap Solution + Fan Setup` | Physical Action | `Dips the ring into the soap solution to form a film and exposes it to airflow, resulting in bubble formation.` |

---

# 7. Sketches and Visual Planning

## 7.1 Concept Sketch
Add an early sketch of the full idea.

**Insert image below:**  
<img src="https://github.com/Aryaa20057/ODT-2026-Bubble-maker/blob/main/images/Rough%20sketch%20of%20idea" width="400">

Example:
```md

```

## 7.2 Labeled Build Sketch
Add a sketch with labels showing:
- structure,
- electronics placement,
- user touch points,
- moving parts,
- output elements.

**Insert image below:**  
<img src="https://github.com/Aryaa20057/ODT-2026-Bubble-maker/blob/main/images/labled%20diagram%20of%20final%20.jpeg">

## 7.3 Approximate Dimensions

| Dimension | Value |
|---|---|
| Length | `38cm` |
| Width | `30cm` |
| Height | `15cm` |
| Estimated weight | `500g-1kg` |

---

# 8. Mechanical Planning

## 8.1 Mechanical Features
Check all that apply.

- [ ] Gears
- [ ] Pulleys
- [ ] Belt drives
- [ ] Linkages
- [ ] Hinges
- [ ] Shafts
- [ ] Springs
- [ ] Bearings
- [ ] Wheels
- [ ] Sliders
- [ ] Levers
- [yes] Not applicable

## 8.2 Mechanical Description
Describe the mechanism and what it is meant to do.

**Response:**  
`The mechanism is an electromechanical bubble-generation system designed to produce soap bubbles in a controlled and repeatable manner. It consists of a ring attached to a servo motor and a fan driven by a DC motor. The servo motor provides precise angular motion, allowing the ring to move vertically between two positions: dipping into a soap solution and rising into the airflow path.

When the servo rotates downward, the ring is submerged in the solution, forming a thin liquid film across its surface. As the servo lifts the ring upward, it aligns the film in front of the DC motor (fan). The DC motor, controlled through pulse-width modulation (PWM), generates airflow that deforms the liquid film and inflates it into a bubble.

The system is designed such that the speed of the DC motor is dynamically linked to the servo’s angle. At lower angles (when the ring is submerged or just emerging), the fan remains off or operates at low speed to prevent premature disruption of the film. As the ring reaches higher angles, the fan speed increases, providing sufficient airflow to form bubbles effectively.

Additionally, the mechanism includes user input through push buttons, allowing manual control of the servo’s position. This enables interactive operation, where the user can control the dipping and lifting process while the system automatically adjusts airflow for optimal bubble formation.`

## 8.3 Motion Planning
If something moves, explain:
- what moves,
- what causes the movement,
- how far it moves,
- how fast it moves,
- what could go wrong.

**Response:**  
`In this system, two main things move: the ring attached to the servo motor and the fan blades of the DC motor. The ring moves up and down in an arc, first dipping into the soap solution and then rising up in front of the fan, while the fan spins to blow air and create bubbles.

The movement of the ring is controlled by the servo motor, which responds to the user pressing the “up” and “down” buttons. Each press slightly changes the angle of the servo, either lifting the ring out of the solution or lowering it back in. At the same time, the fan is powered by a DC motor, and its speed automatically changes depending on how high the ring is.

The ring moves within a set range from fully dipped in the solution to fully raised above it. Instead of jumping instantly, it moves in small steps, making the motion smooth and controlled. The servo moves relatively slowly, while the fan speed changes more noticeably from off, to medium, to fast as the ring rises.

A few things can go wrong in this process. If the ring doesn’t dip properly, the soap film may not form. If the fan blows too hard or too early, the film can break before a bubble is made. Misalignment between the ring and the fan can also affect bubble formation. On the technical side, issues like unresponsive buttons, uneven motor speeds, or loose connections could impact how well the system works.`

## 8.4 Simulation / CAD / Animation Before Making
If your project includes mechanical motion, document the digital planning before fabrication.

| Tool Used | File / Link | What Was Tested |
|---|---|---|
| `[Fusion 360 / Tinkercad / other]` | `[Link or screenshot]` | `[What did you validate?]` |
| `[Tool]` | `[Link or screenshot]` | `[What did you validate?]` |
`not applicable`

## 8.5 Changes After Digital Testing
What changed after the CAD, animation, or simulation stage?

**Response:**  
`Not applicable`

---

# 9. Electronics Planning

## 9.1 Electronics Used

| Component | Quantity | Purpose |
|---|---:|---|
| `Component	Quantity	Purpose
|`ESP32` | `1` | `Acts as the main controller, reading button inputs and controlling both the servo motor and DC motor.` |
| `Servo Motor` | `1` | `Moves the ring up and down to dip into the soap solution and position it for bubble formation.` |
| `DC Motor` | `1` | `Spins to create airflow that forms bubbles from the soap film.` |
|`L298N Motor Driver` | `1` | `Controls the speed of the DC motor using PWM signals from the ESP32.` |
| `LM2596 Buck Converter` | `1` | `Steps down and regulates the voltage to safely power components like the ESP32 and motors.` |
| `Push Buttons` | `2` | `Allow the user to control the upward and downward movement of the servo motor.` |
| `Jumper Wires` | `14` | `Used to connect all electronic components in the circuit.` |
| `Power Adapter` | `1` | `Supplies power to the entire system.` |

## 9.2 Wiring Plan
Describe the main electrical connections.

**Response:**  
`**Response:**
The wiring is organized around the ESP32, which acts as the central controller and is placed on the breadboard. Power from the adapter is first passed through the LM2596 buck converter to step down the voltage to a safe level. This regulated power is then distributed to the ESP32, the servo motor, and the L298N motor driver. All components share a common ground connection to ensure stable operation.

The servo motor is connected to the ESP32 with three wires: power (VCC), ground (GND), and a signal wire connected to D21. This allows the ESP32 to control the angular position of the servo.

The DC motor is connected to the output terminals of the L298N motor driver. The driver itself is connected to the ESP32 using three pins: IN1 (D 27) and IN2 (D 26) to control direction, and ENA (D 14) for speed control using PWM.

Two push buttons are connected to D 18 and D 19. One side of each button is connected to ground, and the other side goes to the respective D pin, using the ESP32’s internal pull-up resistors to detect button presses.

The breadboard is used to organize these connections neatly, with jumper wires linking all components. Overall, the wiring ensures that power is properly regulated and that signals between the ESP32, motors, and user inputs are correctly established for smooth operation of the system.`

## 9.3 Circuit Diagram
Insert a hand-drawn or software-made circuit diagram.

**Insert image below:**  
<img src="https://github.com/Aryaa20057/ODT-2026-Bubble-maker/blob/main/images/final%20circuit.jpeg">

## 9.4 Power Plan

| Question | Response |
|---|---|
| Power source | `DC Power Adapter (primary) + regulated supply via LM2596 Buck Converter` |
| Voltage required | `12V input (for DC motor via L298N), stepped down to 5V for ESP32 and Servo Motor using LM2596` |
| Current concerns | `DC motor can draw high current (especially at startup/stall), which may cause voltage drops affecting ESP32 and servo. Need adequate current-rated adapter. Separate regulation for logic (ESP32) and motor load helps prevent instability.` |
| Safety concerns | `Overheating of L298N and LM2596 under high load, risk of short circuits with jumper wires, voltage mismatch damaging ESP32 (must not exceed 5V input), proper insulation required, and secure connections to avoid sparks or failure.Also working with soap water and ellectric` |

---

# 10. Software Planning

## 10.1 Software Tools

| Tool / Platform | Purpose |
|---|---|
| `[MicroPython / Arduino / MIT App Inventor / CAD tool / other]` | `NA` |
| `[Tool]` | `NA` |

## 10.2 Software Logic
Describe what the code must do.

Include:
- startup behavior,
- input handling,
- sensor reading,
- decision logic,
- output behavior,
- communication logic,
- reset behavior.

**Response:**  
`1. Startup Behavior
When the system is powered on, all hardware components are initialized:
Push buttons are configured as input with pull-up resistors.
The servo motor is initialized and set to the minimum angle (ring dipped in soap solution).
The DC motor is initialized with a default OFF state (PWM duty = 0).
The motor driver direction pins are set so the fan rotates in a single direction.
A message (“Bubble Machine Initialized. Ready to operate.”) is printed for confirmation.
2. Input Handling
Two push buttons are used:
Up Button: increases the servo angle.
Down Button: decreases the servo angle.
The system continuously checks button states in a loop.
Buttons use active-low logic (pressed = 0).
A small delay (0.1 seconds) is used for debouncing and smooth control.
3. Sensor Reading
There are no external sensors in this system.
Instead, the servo angle acts as a virtual state indicator, representing the position of the ring:
Low angle → ring in soap solution
Medium angle → ring out of solution
High angle → ring in front of fan
4. Decision Logic
The system uses predefined angle thresholds:
Below THRESHOLD_SLOW (45°) → fan OFF
Between 45° and 90° → fan runs at slow speed
Above THRESHOLD_FAST (90°) → fan runs at full speed
The servo angle determines the state of the DC motor speed.
5. Output Behavior
Servo Motor Output:
Moves up or down in steps of 5° based on button input.
Limited between minimum (0°) and maximum (120°) angles.
DC Motor Output:
Controlled using PWM via the motor driver:
0 duty → OFF
~512 duty → Medium speed
1023 duty → Full speed
Speed dynamically changes based on servo position to create bubbles.
6. Communication Logic
There is no external communication (Wi-Fi, Bluetooth, etc.).
Basic communication is done through the serial console:
Prints current servo angle and movement direction for debugging and monitoring.
7. Reset Behavior
On reset or power cycle:
The servo returns to the minimum angle (ring dipped in solution).
The DC motor is turned OFF initially.
All variables (like current angle) are reinitialized.
The system resumes normal operation after initialization.`

## 10.3 Code Flowchart
Insert a flowchart showing your code logic.

Suggested sequence:
- start,
- initialize,
- wait for input,
- read input,
- decision,
- trigger output,
- repeat or reset,
- error handling.

**Insert image below:**  
<img src="https://github.com/Aryaa20057/ODT-2026-Bubble-maker/blob/main/images/code%20flow.jpeg">

## 10.4 Pseudocode

```text
from machine import Pin, PWM
import time
from servo import Servo

# 1. Buttons
btn_up = Pin(18, Pin.IN, Pin.PULL_UP)   # pin 18 is button up
btn_down = Pin(19, Pin.IN, Pin.PULL_UP) # pin 19 is button down

# 2. Servo Motor
servo_pin = Pin(21, Pin.OUT)
ring_servo = Servo(servo_pin)

# 3. L298N DC Motor Driver
IN1 = Pin(27, Pin.OUT)
IN2 = Pin(26, Pin.OUT)
en = PWM(Pin(14), freq=1000)


# Change this value after doing your tests to set exactly when the fan speeds up
SPEED_UP_ANGLE = 120
STOP_ANGLE = 90 # Angle at which the ring is just dipping into the soap solution (to be determined experimentally)

# Set initial state for the servo to 90 degrees (outside solution)
current_angle = 65
ring_servo.write_angle(current_angle)

print("Bubble Machine Initialized. Ready to operate.")

while True:
    # Check "Up" Button
    if btn_up.value() == 0:
        current_angle = current_angle + 5
        # maximum limit of 180
        if current_angle > 180:
            current_angle = 180
        ring_servo.write_angle(current_angle)
        print("Moving Up | Angle: " + str(current_angle))
        
    # Check "Down" Button
    if btn_down.value() == 0:
        current_angle = current_angle - 5
        # minimum limit of 0
        if current_angle < 0:
            current_angle = 0
        ring_servo.write_angle(current_angle)
        print("Moving Down | Angle: " + str(current_angle))

    # --- DC Motor Speed Control ---
    
    if current_angle < STOP_ANGLE:
        # Stop motor (Ring is dipping down into the soap)
        en.duty(0)
        IN1.value(0)
        IN2.value(0)
        
    elif current_angle >= STOP_ANGLE and current_angle < SPEED_UP_ANGLE:
        # Rotate DC Motor in clockwise direction with Medium Speed
        en.duty(600)
        IN1.value(0) 
        IN2.value(1)
        
    else: 
        # Rotate DC Motor in clockwise direction with Max Speed (Angle >= SPEED_UP_ANGLE)
        en.duty(1000)
        IN1.value(0) 
        IN2.value(1)

    
    time.sleep(0.1)
```

---

# 11. MIT App Inventor Plan

## 11.1 Is an app part of this project?
- `No`

If yes, complete this section.

## 11.2 Why is the app needed?
Explain what the app adds to the experience.

Examples:
- remote control,
- score tracking,
- mode selection,
- personalization,
- triggering effects,
- displaying data.

**Response:**  
`[NA]`

## 11.3 App Features

| Feature | Purpose |
|---|---|
| `[NA]` | `[NA]` |
| `[NA]` | `[NA]` |
| `[NA]` | `[NA]` |

## 11.4 UI Mockup
Insert a sketch or screenshot of the app interface.

**Insert image below:**  
`[NA]`

## 11.5 App Screen Flow

1. `[NA]`

---

# 12. Bill of Materials

## 12.1 Full BOM

| Item | Quantity | In Kit? | Need to Buy? | Estimated Cost | Material / Spec | Why This Choice? |
|---|---:|---|---|---:|---|---|
| `[ESP32]` | `1` | `Yes` | `yes` | `Rs. 331` | `Wi-Fi + Bluetooth` | `Main controller to handle inputs, servo control, and PWM for motor` |
| `Servo Motor` | `1` | `Yes` | `No` | `0` | `180° rotation, 5V` | `Precise angular control for dipping and lifting the ring` |
| `DC Motor` | `1` | `Yes` | `No` | `0` | `3–12V DC motor` | `Generates airflow to create bubbles` |
| `Fan Blade` | `1` | `No` | `Yes` | `Rs. 50` | `blades` | `Generates airflow to create bubbles` |
| `L298N Motor Driver` | `1` | `Yes` | `No` | `0` | `Dual H-bridge driver` | `Controls speed of DC motor using PWM` |
| `LM2596 Buck Converter` | `1` | `No` | `Yes` | `Rs.104` | `Adjustable step-down module` | `Regulates voltage safely for ESP32 and motors` |
| `Push Buttons` | `[2` | `Yes` | `No` | `0` | `Momentary tactile switches` | `User input to control servo movement (up/down)` |
| `Potentiometer` | `1` | `No` | `Yes` | `Rs. 130` | `10kΩ variable resistor` | `Got for the previous idea` |
| `Jumper Wires` | `15` | `Yes` | `Yes` | `Rs. 75` | `Male–Male / Male–Female` | `Electrical connections between components` |
| `Power Supply (Adapter/Battery)` | `1` | `Yes` | `No` | `0` | `5V–12V DC supply` | `Provides stable power to system` |
| `Bangle (Ring)` | `8` | `No` | `Yes` | `Rs. 76` | `Lightweight` | `Acts as bubble-forming loop` |
| `Soap Solution Container` | `1` | `No` | `Yes` | `Rs.115` | `Plastic bowl/container` | `Holds soap solution for dipping ring` |
| `Connecting Hardware (Tape, Glue)` | `1 each` | `No` | `Yes` | `Rs. 45` | `Adhesives & fasteners` | `Secures components in place` |

## 12.2 Material Justification 
Explain why you selected your main materials and components.

Examples:
- Why acrylic instead of cardboard?
- Why MDF instead of 3D print?
- Why servo instead of DC motor?
- Why bearing instead of a plain shaft hole?

**Response:**  
`12.2 Material Justification

The materials and components used in this project were selected based on reliability, control precision, cost-efficiency, and ease of integration within a circuit-based system.

1. ESP32 (Microcontroller)
The ESP32 was chosen over simpler boards because it provides high processing capability, multiple GPIO pins, and built-in PWM support. This is essential for simultaneously controlling the servo motor, DC motor speed, and reading button inputs. It also allows future scalability (e.g., adding automation or wireless control).

2. Servo Motor (for ring movement)
A servo motor was used instead of a standard DC motor because it allows precise angular control. The project requires the ring to move to specific positions (dip in solution, rise to fan level), which cannot be reliably achieved with a DC motor without complex feedback systems. The servo ensures accuracy and repeatability.

3. DC Motor with Fan (for bubble formation)
A DC motor was selected to drive the fan because it provides continuous rotational motion. Unlike a servo, it can run at variable speeds, which is necessary to control airflow intensity for bubble formation. The speed variation (slow to fast) is critical for controlled bubble generation.

4. LM2596 Buck Converter
The LM2596 buck converter is used to step down voltage efficiently from the power supply to levels suitable for the ESP32 and motors. It was chosen over linear regulators because it is more energy-efficient, produces less heat, and can handle higher current loads required by motors.

5. Push Buttons
Push buttons provide a simple and reliable user interface for manual control of the servo motor (up and down movement). They are cost-effective, easy to integrate, and intuitive for user interaction.

6. Jumper Wires
Jumper wires were chosen for circuit connections because they allow quick prototyping, easy modifications, and secure connections without soldering, which is ideal for iterative design processes.

7. 3D printed ring (Ring Structure)
A 3D printed ring is used as the bubble ring because of its smooth circular shape, lightweight nature, and ready availability. Compared to custom-fabricated rings, it is cost-effective and already optimized for forming consistent soap films.

8. Container (Soap Solution Holder)
A container is used to hold the soap solution due to its stability and ability to maintain sufficient depth for proper dipping. It ensures consistent coating of the ring for bubble formation.

9. Power Supply (Power House Supply)
A stable external power supply is used instead of batteries to provide consistent voltage and current, especially important for running motors without performance drops over time.Was replaced by LM2596 later.

10. Fan Structure
The fan attached to the DC motor was chosen to direct airflow efficiently through the ring. Compared to passive airflow, it provides controlled and consistent air pressure, which is necessary for forming bubbles reliably.`

## 12.3 Items to Purchase Separately

| Item | Why Needed | Purchase Link | Latest Safe Date to Procure | Status |
|---|---|---|---|---|
| `ESP32` | `Previous one burned out` | `ROBU got through a friend` | `1st April 2026` | `Received` |
| `Breadboard Power Supply` | `Previous one burned out` | `ROBU got through a friend` | `1st April 2026` | `Received` |
| `LM2596` | `Power supply was not enough for DC motor` | `got through a friend` | `18th April 2026` | `Received` |
| `Fan blades` | `for DC motor` | `got through a friend` | `18th April 2026` | `Received` |
| `Jumper wires 1m` | `Needed longer wires for model` | `got through a friend` | `19th April 2026` | `Received` |

## 12.4 Budget Summary

| Budget Item | Estimated Cost |
|---|---:|
| Electronics | `331 + 104 + 75 = Rs. 510` |
| Mechanical parts | `50 + 76 = Rs. 126` |
| Fabrication materials | `115 + 45 = Rs. 160` |
| Purchased extras | `Rs. 130` |
| Contingency | `Total so far = 510 + 126 + 160 + 130 = Rs. 926. so, 10% contingency ≈ Rs. 100 (rounded)` |
| **Total** | `Rs. 1026` |

## 12.5 Budget Reflection
If your cost is too high, what can be simplified, removed, substituted, or shared?

**Response:**  
`Your cost isn’t extremely high, but it can definitely be tightened with a few smart adjustments especially since this is a prototype. The easiest win is removing unnecessary components. The potentiometer (Rs. 130) is already not used in your final system, so it can be completely eliminated. That alone cuts a noticeable chunk of the budget without affecting functionality. Next, look at substitution and reuse. The fan blade (Rs. 50) doesn’t have to be bought—you could reuse one from an old toy motor, broken fan, or even make a simple one using lightweight plastic or cardboard. Similarly, instead of buying multiple bangles (Rs. 76), you really only need one effective ring; the rest can be removed or replaced with a single wire loop or 3D-printed ring. For fabrication materials, costs can be reduced by improvisation. The soap container (Rs. 115) can be replaced with any household bowl or recycled plastic container. Tape and glue can also be shared across teams instead of each group purchasing separately. Finally, sharing high-cost electronics across teams (like the ESP32 or power supply) during testing phases can further reduce individual project cost if allowed. Overall, by removing unused components, reusing readily available materials, and sharing resources, the budget can be significantly reduced without compromising the working or concept of the project.
`

---

# 13. Planning the Work

## 13.1 Team Working Agreement
Write how your team will work together.

Include:
- how tasks are divided,
- how decisions are made,
- how progress will be checked,
- what happens if a task is delayed,
- how documentation will be maintained.

**Response:**  
`Our team will work collaboratively by dividing tasks based on each member’s strengths and the requirements of the project. Responsibilities such as circuit design, coding, mechanical setup, testing, and documentation will be distributed so that each member has a defined role while still supporting others when needed.

Decisions will be made through group discussions, where we both can share ideas and opinions. If there is a disagreement, the team will evaluate options based on feasibility, efficiency, and project goals, and come to a consensus. In time-sensitive situations, a majority decision will be followed.

Progress will be checked regularly through short team meetings and updates at the end of each work session. We will review completed tasks, identify any issues, and plan the next steps to ensure the project stays on track.

If a task is delayed, the team will first identify the reason for the delay and provide support to the member responsible. Tasks may be redistributed if necessary to meet deadlines, ensuring that overall progress is not affected.

Documentation will be maintained continuously throughout the project. One or more team members will be responsible for updating the project log, including design changes, code updates, testing results, and observations. All team members will review the documentation periodically to ensure accuracy and completeness.`

## 13.2 Task Breakdown

| Task ID | Task | Owner | Estimated Hours | Deadline | Dependency | Status |
|---|---|---|---:|---|---|---|
| T1 | `[Finalize concept]` | `Aryaa and Hemadri` | `2` | `1/4/26` | `None` | `Done` |
| T2 | `[Complete BOM]` | `Aryaa and Hemadri` | `1` | `20/4/26` | `T1` | `Done` |
| T3 | `[Test electronics]` | `Hemadri` | `2` | `17/4/26` | `T1` | `Done` |
| T4 | `[Build structure]` | `Aryaa and Hemadri` | `4` | `16/4/26` | `T1` | `Done` |
| T5 | `[Write control code]` | `Aryaa` | `4` | `15/4/26` | `T3` | `Done` |
| T6 | `[Integrate system]` | `Aryaa and Hemadri` | `4` | `17/4/26` | `T4, T5` | `Done` |
| T7 | `[Playtest]` | `Aryaa and Hemadri` | `2` | `18/4/26` | `T6` | `Done` |
| T8 | `[Refine and document]` | `Aryaa and Hemadri` | `3` | `20/4/26` | `T7` | `Done` |

## 13.3 Responsibility Split

| Area | Main Owner | Support Owner |
|---|---|---|
| Concept and gameplay | `Both` | `NA` |
| Electronics | `Aryaa` | `Hemadri` |
| Coding | `Hemadri` | `Aryaa` |
| App | `NA` | `NA` |
| Mechanical build | `Aryaa` | `Hemadri` |
| Testing | `both` | `NA` |
| Documentation | `Aryaa` | `Hemadri` |

---

# 14. Weekly Milestones

## 14.1 Four-Week Plan

### Week 1 — Plan and De-risk
Expected outcomes:
- [ ] Idea finalized 
- [ ] Core interaction decided
- [ ] Sketches made
- [ ] BOM completed
- [ ] Purchase needs identified
- [ ] Key uncertainty identified
- [ ] Basic feasibility tested

### Week 2 — Build Subsystems
Expected outcomes:
- [ ] Electronics tests completed
- [ ] CAD / structure planning completed
- [ ] App UI started if needed
- [ ] Mechanical concept tested
- [ ] Main subsystems partially working

### Week 3 — Integrate
Expected outcomes:
- [ ] Physical body built
- [ ] Electronics integrated
- [ ] Code connected to hardware
- [ ] App connected if required
- [ ] First playable version exists

### Week 4 — Refine and Finish
Expected outcomes:
- [ ] Technical bugs reduced
- [ ] Playtesting completed
- [ ] Improvements made
- [ ] Documentation completed
- [ ] Final build ready

## 14.2 Weekly Update Log

| Week | Planned Goal | What Actually Happened | What Changed | Next Steps |
|---|---|---|---|---|
| Week 1 | `Finalization of the idea` | `were able to figure out the mechanism and tools` | `the difficulty of the concept was a bit confusing` | `Making sure we had the parts ready within the next week` |
| Week 2 | `getting the components` | `we got most of the parts but not he main one (the bicycle)` | `we started to think of alternatives calling many people but couldn't find it` | `looking for a solution or alternative` |
| Week 3 | `think of new idea that could work in a week's time` | `we got a list of ideas and got it approved` | `finalisation happened but we had to replan all the steps for the new one plus our newly bought parts were wasted` | `divide the work and make deadlines to create the new product i.e. the bubble making machine game` |
| Week 4 | `finishing the project` | `we were able to finish it in time 2 days before the deadline` | `end moment fan did not work hence we had to rebuid fan by hand` | `finish project and documentation` |

---

# 15. Risks and Unknowns

## 15.1 Risk Register

| Risk | Type | Likelihood | Impact | Mitigation Plan | Owner |
|---|---|---|---|---|---|
| `Servo motor misalignment (ring not dipping properly)` | `Technical` | `Medium` | `High` | `Calibrate MIN_ANGLE and MAX_ANGLE; test angles before final assembly` | `Aryaa` |
| `DC motor speed not producing bubbles` | `Technical` | `Medium` | `High` | `Adjust PWM thresholds (THRESHOLD_SLOW, THRESHOLD_FAST) and test different speeds` | `Hemadri and Aryaa` |
| `Soap film not forming properly on ring` | `Material` | `High` | `Medium` | `Adjust soap solution ratio, test different ring sizes` | `Aryaa` |
| `Structure instability or vibration` | `Mechanical` | `Low` | `High` | `Reinforce base, secure motors tightly, use stable frame` | `Hemadri` |
| `Loose wiring or connection failure` | `Technical` | `Medium` | `High` | `Proper soldering, use insulation, check connections before testing` | `Hemadri` |


## 15.2 Biggest Unknown Right Now
What is the single biggest uncertainty in your project at this stage?

**Response:**  
`The biggest uncertainty at this stage is achieving consistent bubble formation. While the servo motor and DC motor can be controlled precisely through code, the actual formation of bubbles depends on external and variable factors such as soap film quality, airflow strength, and timing between the ring position and fan speed. Ensuring that these elements align reliably to produce bubbles every time remains the key challenge.`

---

# 16. Testing and Playtesting

## 16.1 Technical Testing Plan

| What Needs Testing | How You Will Test It | Success Condition |
|---|---|---|
| `Servo motor movement (ring motion)` | `Press up/down buttons and observe angle changes and ring movement` | `Ring moves smoothly between MIN_ANGLE and MAX_ANGLE without jitter or stalling` |
| `DC motor speed control (fan)` | `Move servo through angles and observe change in fan speed` | `Fan turns OFF, SLOW, and FAST correctly based on defined angle thresholds` |
| `Button input response` | `Press buttons repeatedly and hold them` | `Each press reliably changes angle; no missed inputs or erratic behavior` |
| `Servo + DC motor synchronization` | `Run full motion cycle and observe timing between ring position and fan speed` | `Fan speed increases exactly when ring reaches bubble position` |
| `Bubble formation mechanism` | `Run complete system multiple times with soap solution` | `Bubbles are formed consistently when ring reaches top position` |

## 16.2 Playtesting Plan

| Question | How You Will Check |
|---|---|
| Do players understand what to do? | `Give the device to first-time users without instructions and observe if they can figure out the button controls and purpose` |
| Is the interaction satisfying? | `Ask users to operate the buttons and observe their reaction to bubble formation; collect quick verbal feedback` |
| Do players want another turn? | `Check if users voluntarily try again or continue interacting after the first successful bubble` |
| Is the challenge balanced? | `Observe if controlling the timing/position feels too easy or too difficult; adjust angle increments if needed` |
| Is the response clear and immediate? | `Press buttons and observe delay between input (button press) and output (servo movement + fan response)` |

## 16.3 Testing and Debugging Log

| Date | Problem Found | Type | What You Tried | Result | Next Action |
|---|---|---|---|---|---|
| `17/4/26` | `Power house not working` | `Technical` | `swapped it with LM2596` | `Worked` | `NONE` |
| `20/4/2026` | `Fan is no giving out enough air` | `mechanical` | `manually made the blades with a tin can` | `worked` | `none` |

## 16.4 Playtesting Notes

| Tester | What They Did | What Confused Them | What They Enjoyed | What You Will Change |
|---|---|---|---|---|
| `friend 1` | `Pressed buttons to move the ring up and down and tried to create bubbles multiple times` | `Initially unsure which button moves the ring up or down` | `Enjoyed seeing the bubble form when timing was correct` | `Add simple labels or arrows on buttons for clarity` |
| `classmate 1` | `Experimented with holding and tapping buttons to control the ring position` | `Did not understand why bubbles were not forming every time` | `Found the moment of successful bubble formation satisfying` | `Improve consistency by refining fan speed thresholds and soap solution` |

---

# 17. Build Documentation

## 17.1 Fabrication Process
Describe how the project was physically made.

Include:
- cutting,
- 3D printing,
- assembly,
- fastening,
- wiring,
- finishing,
- revisions.

**Response:**  
`The bubble-making device was fabricated through a combination of manual construction and digital fabrication techniques, ensuring both structural stability and functional precision.`

`Cutting:
The main body of the structure was made using foam board. The foam board sheets were carefully measured and cut using precision cutters to form the base, vertical supports, and motor mounts. Openings were also cut to securely place the servo motor and DC motor in alignment.`

`3D Printing:
The bubble ring, which is the key functional component, was designed digitally and fabricated using 3D printing. This allowed for accurate geometry and a smooth surface, ensuring consistent soap film formation for bubble generation.`

`Assembly:
All foam board components were assembled to create a stable frame. The structure was designed to hold the servo motor at an appropriate height so that the ring could dip into the soap solution and rise directly in front of the DC motor (fan).`

`Fastening:
Components were fastened using a combination of hot glue and adhesive, which provided quick bonding and sufficient strength for lightweight materials like foam board. The motors were securely fixed to prevent vibration or displacement during operation.`

`Wiring:
Electrical connections were made between the servo motor, DC motor driver (L298N), buttons, and the microcontroller. Proper routing of wires was ensured to avoid tangling or interference with moving parts. Connections were tested to ensure reliable signal transmission and power delivery.`

`Finishing:
The structure was refined by reinforcing weak joints and ensuring smooth movement of the ring mechanism. Edges were cleaned, and alignment between the ring and the fan was adjusted for optimal bubble formation.`

`Revisions:
Several iterations were made during the fabrication process. Adjustments included recalibrating the servo angles, repositioning the motors for better alignment, and modifying the ring design to improve bubble consistency. The thresholds for fan speed were also fine-tuned to achieve effective bubble formation at the correct moment.`

## 17.2 Build Photos
Add photos throughout the project.

Suggested images:
- early sketch,
- prototype,
- electronics testing,
- mechanism test,
- app screenshot,
- final build.

Example:
```md



```

## 17.3 Version History

| Version | Date | What Changed | Why |
|---|---|---|---|
| `v1` | `14/4/2026` | `Basic structure made using foam board, servo motor attached to ring and DC motor added but ran at constant speed` | `To create a working prototype and test basic bubble formation mechanism` |
| `v2` | `16/4/2026` | `Introduced angle-based control for DC motor speed using PWM; improved alignment between ring and fan` | `To improve bubble quality and ensure air flow matches ring position` |
| `v3` | `19/4/2026` | `Added button controls for manual servo movement; refined angle limits and thresholds; improved wiring and stability` | `To give user control, increase precision, and make the system more reliable and interactive` |

---

# 18. Final Outcome

## 18.1 Final Description
Describe the final version of your project.

**Response:**  
`The final version of the project is an automated bubble-making device that integrates a servo motor, a DC motor (fan), and user-controlled inputs through buttons. The servo motor controls the vertical movement of a 3D-printed ring, allowing it to dip into a soap solution and then rise into position. As the ring moves upward, the DC motor operates at variable speeds based on the angle of the servo motor. When the ring reaches an optimal height, the fan spins at high speed to create bubbles. The system is mounted on a foam board structure, with all components aligned to ensure smooth operation and consistent bubble formation. The interaction between mechanical movement and programmed control allows for a simple but effective automated system.`

## 18.2 What Works Well
- `The synchronization between the servo motor position and DC motor speed effectively produces bubbles at the right moment.`
- `The button-controlled interface allows easy and precise control of the ring movement.`
- `The 3D-printed ring design successfully holds the soap film and enables consistent bubble formation.`

## 18.3 What Still Needs Improvement
- `The foam board structure could be made more durable and stable using stronger materials.`
- `The bubble formation is sometimes inconsistent and depends on environmental factors like airflow and soap quality.`
- `The wiring and component layout could be made more compact and organized for better reliability and aesthetics.`

## 18.4 What Changed From the Original Plan
How did the project change from the initial idea?

**Response:**  
`## **18.4 What Changed From the Original Plan**

**Response:**
The original concept of the project was to create an interactive system where a physical bicycle would control an online car racing game. The plan involved using a reed switch to measure the wheel’s revolutions per second (to simulate speed) and a potentiometer attached to the handlebar to detect turning inputs.

However, this idea was not carried forward due to practical constraints. The unavailability of a suitable bicycle and the limited time frame made it difficult to build and calibrate the system effectively. Additionally, integrating real-time physical inputs with a digital game would have required more complex setup and testing.

As a result, the project was redefined into a bubble-making machine using motors and simple user inputs. This new approach allowed us to focus on a manageable system involving servo and DC motors, while still demonstrating concepts of control systems, user interaction, and circuit integration within the given constraints.
`

---

# 19. Reflection

## 19.1 Team Reflection
What did your team do well?  
What slowed you down?  
How well did you manage time, tasks, and responsibilities?

**Response:**  
`## **19.1 Team Reflection**

**Response:**
Our team worked well in terms of collaboration and adaptability. We were able to communicate ideas clearly, divide tasks based on individual strengths, and support each other during both the design and implementation stages. Once we shifted to the bubble machine concept, we were more focused and efficient, especially in integrating the mechanical structure with the circuit and code.

However, what slowed us down initially was the change in project direction. Time was lost in exploring the first idea and then transitioning to a completely new concept. Additionally, some delays occurred during testing and calibration, particularly in aligning the servo movement with the DC motor speed for consistent bubble formation.

In terms of time, task, and responsibility management, we performed moderately well. While tasks were eventually distributed effectively, earlier planning and quicker decision-making could have improved our overall efficiency. Despite this, we were able to complete the project within the given timeframe by adjusting our workflow and prioritizing essential components.`

## 19.2 Technical Reflection
What did you learn about:
- electronics,
- coding,
- mechanisms,
- fabrication,
- integration?

**Response:**  
`This project helped us understand how different parts come together to make a working system.

In electronics, we learned how to connect and control components like the servo motor, DC motor, buttons, and the L298N driver. We got a clearer idea of how PWM works for speed control and how inputs from buttons can trigger physical actions.

For coding, we learned how to translate logic into real-world behavior. Writing code to control the servo angle and link it to the fan speed showed us how small changes in code can directly affect the output. We also understood the importance of calibration and testing.

In terms of mechanisms, we explored how motion works how the servo’s rotation could be used to dip and lift the ring, and how timing and positioning are important to actually form a bubble.

During fabrication, we worked with foam board and a 3D-printed part, which taught us about building stable structures, aligning components properly, and making small adjustments when things didn’t fit perfectly.

Finally, in integration, we realized that everything has to work together smoothly. Even if one part is slightly off whether in code, wiring, or structure  it affects the whole system. A lot of our learning came from testing, fixing, and improving the setup step by step.`

## 19.3 Design Reflection
What did you learn about:
- designing for play,
- delight,
- clarity,
- physical interaction,
- player understanding,
- iteration?

**Response:**  
``

## 19.4 If You Had One More Week
What would you improve next?

**Response:**  
`If we had one more week, we would focus on improving both the performance and user experience of the system. First, we would refine the mechanism to make the motion smoother and more consistent, especially the dipping and lifting of the ring. This would help in forming more reliable bubbles. We would also experiment with different ring designs and sizes to improve bubble quality. On the electronics and coding side, we would try to automate the process instead of relying only on manual button inputs possibly creating a loop where the system runs on its own with optimized timing. We would also fine tune the speed control of the DC motor for better synchronization with the servo movement. In terms of fabrication, we would make the structure more durable and precise, possibly using stronger materials or better mounting techniques to reduce vibrations and misalignment. Finally, we would work on improving the overall **integration**, making the system more compact, stable, and visually clean, while reducing loose wiring and making it easier to use.`

---

# 20. Final Submission Checklist

Before submission, confirm that:
- [ ] Team details are complete
- [ ] Project description is complete
- [ ] Inspiration sources are included
- [ ] Player journey is written
- [ ] Sketches are added
- [ ] BOM is complete
- [ ] Purchase list is complete
- [ ] Budget summary is complete
- [ ] Mechanical planning is documented if applicable
- [ ] App planning is documented if applicable
- [ ] Code flowchart is added
- [ ] Task breakdown is complete
- [ ] Weekly logs are updated
- [ ] Risk register is complete
- [ ] Testing log is updated
- [ ] Playtesting notes are included
- [ ] Build photos are included
- [ ] Final reflection is written

---

# 21. Suggested Repository Structure

```text
project-repo/
├── README.md
├── images/
│   ├── concept-sketch.jpg
│   ├── labeled-sketch.jpg
│   ├── circuit-diagram.jpg
│   ├── ui-mockup.jpg
│   ├── prototype-1.jpg
│   └── final-build.jpg
├── code/
│   ├── main.py
│   ├── test_code.py
│   └── notes.md
├── cad/
│   ├── models/
│   └── screenshots/
└── docs/
    ├── references.md
    └── extra-notes.md
```

---

# 22. Instructor Review

## 22.1 Proposal Approval
- [ ] Approved to proceed
- [ ] Approved with changes
- [ ] Rework required before proceeding

**Instructor comments:**  
`[Instructor fills this section]`

## 22.2 Midpoint Review
`[Instructor fills this section]`

## 22.3 Final Review Notes
`[Instructor fills this section]`
