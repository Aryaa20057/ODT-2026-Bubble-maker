# Open Design and Technology  
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
`[Pup-up your childhood]`

## 1.5 Expanded Project Idea
In 1–2 paragraphs, explain:
- what your project is,
- what kind of playful experience it creates,
- what makes it fun, curious, engaging, strange, satisfying, competitive, or delightful,
- what technologies are involved.

**Response:**  
`[Our project is an interactive bubble-making machine. This project uses servo motor which controls the ring to move in an out of the soup solution, while DC motor works as a fan to generate airflow for forming bubbles. The system is programmed so that the fan speed of the DC motor responds to the angle of the servo motor, slow when the ring is dipped in the solution and rising and fast when it reaches the optimal position for bubble formation. The users interact with this through the buttons that allow them to manually control the movement for the ring.
The playful experience comes from the balance between control and surprise. While the user actively decides when and how the ring moves, the actual formation of bubbles feels slightly unpredictable and satisfying—sometimes producing perfect bubbles, sometimes none at all. This creates a sense of curiosity and experimentation, encouraging users to explore timing, positioning, and rhythm. It is engaging because it transforms a simple childhood activity into a responsive, interactive system, using technologies like MicroPython on ESP32, PWM motor control, serco motor operation, and user input through buttons.]`

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
`So what really makes our bubble machine different? For starters, it’s not just a simple on/off gadget spinning all day. We actually gave the hardware some “real conversation” every part works together, and the microcontroller keeps everything in sync, mechanics and electronics teaming up. Most bubble machines? They just run a motor on a timer, or expect you to crank a handle. Ours is on another level.

Here’s where things get cool: the fan’s speed changes based on exactly what the servo arm is doing at that moment. The microcontroller always knows where the bubble ring sits during each cycle. When the ring dips into the soap, the fan cuts out completely. As it comes up, the fan starts to spin. Once the ring’s out and ready, the fan blasts at full power. No wasted air, no guessing—it’s like the machine has a mini brain, making decisions every step instead of just repeating itself like a robot.

We didn’t want it totally hands-off, either. We put in two simple buttons so you can move the servo arm yourself set the pace however you want. Maybe sometimes you want a fast dip and a quick burst, or other times you want to slow down and really watch those bubbles build up. The machine actually pays attention to you.

Instead of copying those basic toys with a spinning wand and constant breeze, we tried to capture the way people actually make bubbles: dip the ring, lift it out, and blow at the perfect moment. The machine kind of acts like you just with a little help from electronics.

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
`[Upload image and link here]`

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
`[Upload image and link here]`

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

The servo motor is connected to the ESP32 with three wires: power (VCC), ground (GND), and a signal wire connected to GPIO 21. This allows the ESP32 to control the angular position of the servo.

The DC motor is connected to the output terminals of the L298N motor driver. The driver itself is connected to the ESP32 using three pins: IN1 (GPIO 27) and IN2 (GPIO 26) to control direction, and ENA (GPIO 14) for speed control using PWM.

Two push buttons are connected to GPIO 18 and GPIO 19. One side of each button is connected to ground, and the other side goes to the respective GPIO pin, using the ESP32’s internal pull-up resistors to detect button presses.

The breadboard is used to organize these connections neatly, with jumper wires linking all components. Overall, the wiring ensures that power is properly regulated and that signals between the ESP32, motors, and user inputs are correctly established for smooth operation of the system.`

## 9.3 Circuit Diagram
Insert a hand-drawn or software-made circuit diagram.

**Insert image below:**  
`[Upload image and link here]`

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
| `[MicroPython / Arduino / MIT App Inventor / CAD tool / other]` | `[Purpose]` |
| `[Tool]` | `[Purpose]` |

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
`[Write here]`

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
`[Upload image and link here]`

## 10.4 Pseudocode

```text
[Write your pseudocode here]
```

---

# 11. MIT App Inventor Plan

## 11.1 Is an app part of this project?
- [ ] Yes
- [ ] No

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
`[Write here]`

## 11.3 App Features

| Feature | Purpose |
|---|---|
| `[Bluetooth connect button]` | `[Purpose]` |
| `[Score display]` | `[Purpose]` |
| `[Control button / slider / label]` | `[Purpose]` |

## 11.4 UI Mockup
Insert a sketch or screenshot of the app interface.

**Insert image below:**  
`[Upload image and link here]`

## 11.5 App Screen Flow

1. `[Step 1]`
2. `[Step 2]`
3. `[Step 3]`
4. `[Step 4]`

---

# 12. Bill of Materials

## 12.1 Full BOM

| Item | Quantity | In Kit? | Need to Buy? | Estimated Cost | Material / Spec | Why This Choice? |
|---|---:|---|---|---:|---|---|
| `[ESP32]` | `1` | `Yes` | `No` | `0` | `[Spec]` | `[Reason]` |
| `[Item]` | `[Qty]` | `[Yes/No]` | `[Yes/No]` | `[Cost]` | `[Spec]` | `[Reason]` |
| `[Item]` | `[Qty]` | `[Yes/No]` | `[Yes/No]` | `[Cost]` | `[Spec]` | `[Reason]` |

## 12.2 Material Justification
Explain why you selected your main materials and components.

Examples:
- Why acrylic instead of cardboard?
- Why MDF instead of 3D print?
- Why servo instead of DC motor?
- Why bearing instead of a plain shaft hole?

**Response:**  
`[Write here]`

## 12.3 Items to Purchase Separately

| Item | Why Needed | Purchase Link | Latest Safe Date to Procure | Status |
|---|---|---|---|---|
| `[Item]` | `[Reason]` | `[Link]` | `[Date]` | `[Pending / Ordered / Received]` |
| `[Item]` | `[Reason]` | `[Link]` | `[Date]` | `[Pending / Ordered / Received]` |

## 12.4 Budget Summary

| Budget Item | Estimated Cost |
|---|---:|
| Electronics | `[Cost]` |
| Mechanical parts | `[Cost]` |
| Fabrication materials | `[Cost]` |
| Purchased extras | `[Cost]` |
| Contingency | `[Cost]` |
| **Total** | `[Cost]` |

## 12.5 Budget Reflection
If your cost is too high, what can be simplified, removed, substituted, or shared?

**Response:**  
`[Write here]`

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
`[Write here]`

## 13.2 Task Breakdown

| Task ID | Task | Owner | Estimated Hours | Deadline | Dependency | Status |
|---|---|---|---:|---|---|---|
| T1 | `[Finalize concept]` | `[Name]` | `2` | `[Date]` | `None` | `To Do` |
| T2 | `[Complete BOM]` | `[Name]` | `1` | `[Date]` | `T1` | `To Do` |
| T3 | `[Test electronics]` | `[Name]` | `2` | `[Date]` | `T1` | `To Do` |
| T4 | `[Build structure]` | `[Name]` | `4` | `[Date]` | `T1` | `To Do` |
| T5 | `[Write control code]` | `[Name]` | `4` | `[Date]` | `T3` | `To Do` |
| T6 | `[Integrate system]` | `[Name]` | `4` | `[Date]` | `T4, T5` | `To Do` |
| T7 | `[Playtest]` | `[Name]` | `2` | `[Date]` | `T6` | `To Do` |
| T8 | `[Refine and document]` | `[Name]` | `3` | `[Date]` | `T7` | `To Do` |

## 13.3 Responsibility Split

| Area | Main Owner | Support Owner |
|---|---|---|
| Concept and gameplay | `[Name]` | `[Name]` |
| Electronics | `[Name]` | `[Name]` |
| Coding | `[Name]` | `[Name]` |
| App | `[Name]` | `[Name]` |
| Mechanical build | `[Name]` | `[Name]` |
| Testing | `[Name]` | `[Name]` |
| Documentation | `[Name]` | `[Name]` |

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
| Week 1 | `[Write here]` | `[Write here]` | `[Write here]` | `[Write here]` |
| Week 2 | `[Write here]` | `[Write here]` | `[Write here]` | `[Write here]` |
| Week 3 | `[Write here]` | `[Write here]` | `[Write here]` | `[Write here]` |
| Week 4 | `[Write here]` | `[Write here]` | `[Write here]` | `[Write here]` |

---

# 15. Risks and Unknowns

## 15.1 Risk Register

| Risk | Type | Likelihood | Impact | Mitigation Plan | Owner |
|---|---|---|---|---|---|
| `[Example: Bluetooth disconnects]` | `Technical` | `Medium` | `High` | `[Fallback interaction / simplify connection flow]` | `[Name]` |
| `[Example: Structure breaks during play]` | `Mechanical` | `Medium` | `High` | `[Reinforce joints / change material]` | `[Name]` |
| `[Risk]` | `[Technical / Material / Time / Gameplay]` | `[Low/Medium/High]` | `[Low/Medium/High]` | `[Plan]` | `[Name]` |
| `[Risk]` | `[Type]` | `[Low/Medium/High]` | `[Low/Medium/High]` | `[Plan]` | `[Name]` |

## 15.2 Biggest Unknown Right Now
What is the single biggest uncertainty in your project at this stage?

**Response:**  
`[Write here]`

---

# 16. Testing and Playtesting

## 16.1 Technical Testing Plan

| What Needs Testing | How You Will Test It | Success Condition |
|---|---|---|
| `[Bluetooth connection]` | `[Method]` | `[What counts as success?]` |
| `[Mechanism movement]` | `[Method]` | `[What counts as success?]` |
| `[Sensor behavior]` | `[Method]` | `[What counts as success?]` |
| `[App communication]` | `[Method]` | `[What counts as success?]` |

## 16.2 Playtesting Plan

| Question | How You Will Check |
|---|---|
| Do players understand what to do? | `[Method]` |
| Is the interaction satisfying? | `[Method]` |
| Do players want another turn? | `[Method]` |
| Is the challenge balanced? | `[Method]` |
| Is the response clear and immediate? | `[Method]` |

## 16.3 Testing and Debugging Log

| Date | Problem Found | Type | What You Tried | Result | Next Action |
|---|---|---|---|---|---|
| `[Date]` | `[Describe issue]` | `[Technical / Mechanical / UI / Gameplay]` | `[What you did]` | `[Worked / Partly / Failed]` | `[Next step]` |
| `[Date]` | `[Describe issue]` | `[Type]` | `[What you did]` | `[Result]` | `[Next step]` |

## 16.4 Playtesting Notes

| Tester | What They Did | What Confused Them | What They Enjoyed | What You Will Change |
|---|---|---|---|---|
| `[Peer / friend / classmate]` | `[Observation]` | `[Observation]` | `[Observation]` | `[Action]` |
| `[Peer / friend / classmate]` | `[Observation]` | `[Observation]` | `[Observation]` | `[Action]` |

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
`[Write here]`

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
| `v1` | `[Date]` | `[Describe]` | `[Reason]` |
| `v2` | `[Date]` | `[Describe]` | `[Reason]` |
| `v3` | `[Date]` | `[Describe]` | `[Reason]` |

---

# 18. Final Outcome

## 18.1 Final Description
Describe the final version of your project.

**Response:**  
`[Write here]`

## 18.2 What Works Well
- `[Point 1]`
- `[Point 2]`
- `[Point 3]`

## 18.3 What Still Needs Improvement
- `[Point 1]`
- `[Point 2]`
- `[Point 3]`

## 18.4 What Changed From the Original Plan
How did the project change from the initial idea?

**Response:**  
`[Write here]`

---

# 19. Reflection

## 19.1 Team Reflection
What did your team do well?  
What slowed you down?  
How well did you manage time, tasks, and responsibilities?

**Response:**  
`[Write here]`

## 19.2 Technical Reflection
What did you learn about:
- electronics,
- coding,
- mechanisms,
- fabrication,
- integration?

**Response:**  
`[Write here]`

## 19.3 Design Reflection
What did you learn about:
- designing for play,
- delight,
- clarity,
- physical interaction,
- player understanding,
- iteration?

**Response:**  
`[Write here]`

## 19.4 If You Had One More Week
What would you improve next?

**Response:**  
`[Write here]`

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
