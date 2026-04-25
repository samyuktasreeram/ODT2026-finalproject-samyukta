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
`Samyukta: Empire State of Mind`

## 1.2 Team Members

| Name | Primary Role | Secondary Role | Strengths Brought to the Project |
|---|---|---|---|
| `[Samyukta Sreeram]` | `[Electronics / Coding / Fabrication / Mechanics]` | `[Documentation]` | `[hardware-software integration, creative game design, independent problem solving, building skills, adaptability, detail orientation.]`|

## 1.3 Project Title
`[Empire State of Mind]`

## 1.4 One-Line Pitch
`[An Interactive reaction game involving a light up Empire State Building to test the player's pattern recognition and memory.]`

## 1.5 Expanded Project Idea
In 1–2 paragraphs, explain:
- what your project is,
- what kind of playful experience it creates,
- what makes it fun, curious, engaging, strange, satisfying, competitive, or delightful,
- what technologies are involved.

**Response:**  
`Empire State of Mind is a gamified, physical interaction in which the player lights up a model of the Empire State Building by completing three levels of a pattern-memory game. Each level corresponds to a section of the building's facade, lit by 2 dedicated LED strips. The game flashes a sequence of touch-pad positions for the player to memorise and reproduce — getting harder to remember as the pressure mounts. Correct answers reward the player with ascending tones and a purple light sweep; mistakes trigger a harsh buzzer and a red/ pink flash across the whole structure.

What makes the experience compelling is its combination of sensory feedback and architectural storytelling. The building itself becomes a scoreboard — each successfully lit section adds to a growing, glowing structure. The buzzer sounds are deliberately emotional: satisfying when correct, jarring when wrong. This psychological push-and-pull creates a loop of tension and reward that keeps players coming back. Technologies involved include an ESP32 microcontroller, six NeoPixel LED strips, six capacitive touch pads, and a PWM buzzer, all programmed in MicroPython.`

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
`The experience of this installation is a tactile, real-time memory and pattern game. The player should feel a mix of nervous focus during the pattern display, tension while inputting, and a rush of satisfaction or disappointment depending on the outcome. The reward system of buzzer sounds and coloured lights, and architectural feedback (lighting up the building floor by floor) creates strong engagement and motivation to replay, and the pattern is randomly generated each round, so no two games are identical.`

## 2.3 Design Persona
Complete the sentence below:

> We are designing this project as if we are a small creative studio making a **[toy / game / playable object / interactive experience]** for **[children / teens / adults / classmates / exhibition visitors / mixed audience]**.

**Response:**  
`We are designing this project as if we are a small creative studio making an interactive and experential sensory game for exhibition visitors who are competitive, `

---

# 3. Inspiration

## 3.1 References
List what inspired the project.

| Source Type | Title / Link | What Inspired You |
|---|---|---|
| `Toy / Game` | `Simon (Hasbro, 1978)` | `Core mechanic: show a colour/sound pattern, player repeats it. Borrowed the escalating-pressure structure.` |
| `Interactive installation` | `TeamLab Borderless, Tokyo` | `Architecture as canvas — the idea that a physical structure can be a dynamic output display.` |
| `Video game` | `Bop It! (Hasbro)` | `Single-player reflex game with multi-modal feedback (sound + light). Inspired the buzzer tone design.` |

## 3.2 Original Twist
What makes your project original?

**Response:**  
`Empire State of Mind transforms a simple game into an architectural interaction with a feedback system that keeps the player on edge but simultaneously wanting to play more.`

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
`start game ---> watch pattern ---> remember ---> touch ---> react ---> repeat w next level (advance or restart)`

## 4.2 Intended Player / Audience

| Question | Response |
|---|---|
| Who is this for? | `[Exhibition visitors, anyone encountering it in an open display context]` |
| Age range | `[10+ yr olds to]` |
| Solo or multiplayer | `Solo player` |
| Expected duration of one round | `15-20 seconds` |
| What should the player feel? | `Anxiety, tension, excitement, reward` |
| Is explanation required before use? | `Very slight - pretty self explanatory after watching 1 or 2 rounds.` |

## 4.3 Player Journey
Describe exactly how a player will use the project.

1. **Approach:** `Player sees a dimly glowing Empire State Building model in idle mode. (Laptop screen says "Touch to start.")`
2. **Start:** `Player touches the start pad to begin plaaying the game. All strips flash white and the game begins.`
3. **First Action:** `The first 'level' (first 2 LED strips) flash a 4-step pattern.`
4. **Main Interaction:** `The player has to observe, remember and replicate the pattern by touching the touchpads in the correct order.`
5. **System Response:** `The correct input of the pattern triggers purple confirmation flashes and a happy buzz; and the player moves to the next level. Wrong inputs trigger a red flash and a descending buzz, and the game restarts.`
6. **Win / Lose / End Condition:** `A player can win the game by completing 3 levels/ rounds of pattern replication. The game ends and restarts on any wrong input.`
7. **Reset:** `On completion, the LEDs clear, and the system returns to an idle glow, waiting for the start pad again.`

## 4.4 Rules of Play
If your project is a game, list the rules clearly.


- `Press the start button to commence the game.`
- `Watch the LED pattern carefully — it plays only once.`
- `Touch the pads in the exact same order as the pattern shown`
- `You have 3 levels to complete; each uses a different section of the building, and the pattern on the next level starts as soon as the previous level finishes.`
- `One wrong input ends the game immediately and it goes back to the start mode.`

---

# 5. Definition of Success

## 5.1 Definition of “Playable”
Your project will be considered complete only if these conditions are met.

- [ ] `Start touchpin works reliably to commence the game`
- [ ] `All 3 LED strips respond correctly to game state`
- [ ] `Touch pads register input reliably without false triggers`
- [ ] `Win and lose states both trigger distinct light + sound feedback`
- [ ] `Game resets cleanly after every round`

## 5.2 Minimum Viable Version
What is the smallest version of this project that still delivers the core experience?

**Response:**  
`The smallest version would be a single LED strip running one level of the pattern game with working touch input, correct/wrong buzzer feedback, and a basic reset.`

## 5.3 Stretch Features
What features are nice to have but not essential?

- `[Increasing pattern length as difficulty ramps up across levels (e.g. 4 → 5 → 6 steps).]`
- `[A high-score timer displayed via serial or a small OLED screen]`
- `[possibly a 2 or multiplayer competitive mode where they take turns]`

---

# 6. System Overview

## 6.1 Project Type
Check all that apply.

- [/] Electronics-based
- [ ] Mechanical
- [/] Sensor-based
- [ ] App-connected
- [ ] Motorized
- [/] Sound-based
- [/] Light-based
- [ ] Screen/UI-based
- [/] Fabricated structure
- [/] Game logic based
- [/] Installation / tabletop experience
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
`The player touches a start pad to wake the system. An ESP32 microcontroller generates a random 4-step pattern and flashes it on one of 3 NeoPixel LED strips embedded in an Empire State Building model. The player reproduces the pattern using 6 capacitive touch pads. The ESP32 compares the input to the pattern and triggers buzzer tones and LED colors to signal correct or incorrect responses. 3 successful levels triggers a full building light-up and a win melody on the buzzer.
**Input:** 6 capacitive touch pads + 1 start pad  
**Processing:** ESP32 running MicroPython game logic  
**Output:** 3 NeoPixel LED strips (18 LEDs total) + PWM buzzer  
**Structure:** Fabricated Empire State Building model`

## 6.3 Input / Output Map

| System Part | Type | What It Does |
|---|---|---|
| `[Start touch pad]` | Input | `[Wakes the game from idle state]` |
| `[6 Capacitive touch pads]` | Input | `[Detect player finger input for pattern reproduction]` |
| `[ESP32]` | Processing | `[Runs game logic, generates patterns, compares input, controls outputs]` |
| `[6 NeoPixel LED strips]` | Output | `[Display patterns, confirm input, signal win/lose states]` |
| `[Buzzer]` | Output | `[Plays correct, wrong, and win sound feedback]` |
| `[Building the structure]` | Physical Action | `[to house the electronics, provide an interface and display the patterns and levels.]` |

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
| Length | `[Write here]` |
| Width | `[Write here]` |
| Height | `[Write here]` |
| Estimated weight | `[Write here]` |

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
- [/] Not applicable

## 8.2 Mechanical Description
Describe the mechanism and what it is meant to do.

**Response:**  
`[n.a - This project has no moving mechanical parts. The physical build consists of a static fabricated structure. All interaction is electronic (touch input) and all output is light and sound.]`

## 8.3 Motion Planning
If something moves, explain:
- what moves,
- what causes the movement,
- how far it moves,
- how fast it moves,
- what could go wrong.

**Response:**  
`n.a`

## 8.4 Simulation / CAD / Animation Before Making
If your project includes mechanical motion, document the digital planning before fabrication.

| Tool Used | File / Link | What Was Tested |
|---|---|---|
| `[Fusion 360 / Tinkercad / other]` | `[Link or screenshot]` | `[What did you validate?]` |
| `[Tool]` | `[Link or screenshot]` | `[What did you validate?]` |

## 8.5 Changes After Digital Testing
What changed after the CAD, animation, or simulation stage?

**Response:**  
`[n.a. - testing done using physical corkboard and cardboard model.]`

---

# 9. Electronics Planning

## 9.1 Electronics Used

| Component | Quantity | Purpose |
|---|---:|---|
| `[ESP32]` | `1` | `[Main controller]` |
| `[NeoPixel LED strip (6 LEDs)]` | `[6]` | `[Game display — 2 per level.]` |
| `[Capacitive touch pads]` | `[7]` | `[Player input]` |
| `[Buzzer]` | `[1]` | `[Audio feedback]` |

## 9.2 Wiring Plan
Describe the main electrical connections.

**Response:**  
`[Write here]`

## 9.3 Circuit Diagram
Insert a hand-drawn or software-made circuit diagram.

**Insert image below:**  
`[Upload image and link here]`

## 9.4 Power Plan

| Question | Response |
|---|---|
| Power source | `[USB / battery / adapter / other]` |
| Voltage required | `[Write here]` |
| Current concerns | `[Write here]` |
| Safety concerns | `[Write here]` |

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
-`**Startup:** Initialise LED strips, touch pads, and buzzer. Enter idle state (dim green-teal glow on all strips).`
- `**Input handling:** Poll start pad continuously in idle loop. Poll all 6 touch pads during player input phase with debounce delay.`
-` **Sensor reading:** TouchPad.read() returns a capacitance value — a reading below the threshold (100) registers as a confirmed touch.`
- `**Decision logic:** After player input is collected, compare the input list directly against the stored pattern list. Match = level passed; mismatch = game over.`
- `**Output behaviour:** Drive LED strips with dim() colour values for all visual states. Drive buzzer via PWM frequency and duty cycle for all audio states.`
- `**Reset behaviour:** After win animation or game-over flash, clear all LEDs and return to idle start loop.]`

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

text
`SETUP:
  Define 6 LEDs per strip, 30% brightness
  Initialize 3 LED strips on pins 18, 19, 21
  Initialize 6 touch pads on pins 15, 4, 27, 14, 12, 13
  Initialize buzzer on pin 32
  Set touch threshold = 100


HELPER FUNCTIONS:

  dim(color):
    Return color scaled down to 30% brightness

  buzz_wrong():
    Play two descending low tones (sad sound)

  buzz_correct():
    Play four ascending tones (happy sound)

  buzz_win():
    Play a 7-note victory melody

  clear_all():
    Turn off every LED on all 3 strips

  fill_strip(strip, color):
    Set all LEDs on a strip to a given color instantly

  fill_strip_animated(strip, color):
    Set LEDs one by one with a short delay (sweeping effect)

  flash_pattern(strip, pattern):
    FOR each index in pattern:
      Light up that LED → wait 0.5s → turn it off → wait 0.3s

  get_touch():
    LOOP forever:
      FOR each touch pad:
        IF pad is touched (reading < threshold):
          Wait briefly (debounce)
          RETURN the index of that pad

  get_player_input(length, strip):
    REPEAT 'length' times:
      Wait for a touch → record it
      Briefly flash that LED purple to confirm input
    RETURN list of recorded touches

  show_result_all(correct):
    IF correct → fill all strips with teal
    ELSE       → fill all strips with red/pink
    Wait 1 second → clear all

  win_animation():
    Flash all strips purple ON/OFF 5 times
    Keep all strips lit for 7 seconds
    Clear all


WAIT FOR START:
  LOOP forever:
    Set all strips to dim green-teal (idle glow)
    IF start pad is touched:
      Flash all strips white → wait → clear → EXIT loop


MAIN GAME LOOP (runs forever):

  Wait for start touch
  Clear all LEDs

  FOR level 1 to 3:
    Select the strip for this level

    Generate a random pattern of 4 touch-pad indices (0–5)
    Show the pattern on the strip using flash_pattern()

    Record player input (4 touches) using get_player_input()

    IF player input matches the pattern:
      Play correct sound
      Animate strip fill (purple sweep)

    ELSE:
      Play wrong sound
      Flash all strips red
      Mark game as over → BREAK out of level loop

  `[IF all 3 levels passed:
    Play win melody
    Play win animation (purple flashing + hold)

  Clear all LEDs
  Print "Waiting to restart..." → loop back to start]`

# 11. MIT App Inventor Plan

## 11.1 Is an app part of this project?
- [ ] Yes
- [/] No

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
`[n.a! game is self contained on esp 32]`

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
| `[ESP32]` | `1` | `Yes` | `yes` | `400` | `[ESP32-WROOM-32]` | `[reqd for coding and touchpins to execute the game]` |
| `[Neopixel LED roll]` | `[1 roll - 1 meter]` | `[no]` | `[Yes]` | `[275]` | `[5V rgb individually addressable]` | `[each led can be individually coded in the strip to flash the reqd pattern]` |
| ` Power Supply ` | `[1]` | `[Yes/No]` | `[Yes]` | `[ Borrowed from friend thus O]` | `[Spec]` | `[Reason]` |

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
| `[spraypaint]` | `[ for presentation of the physical structure.]` | `[Link]` | `[19th April ]` | `[Received]` |

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

## 13.1 Team Working Agreement - not applicable (working individually)

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
| T1 | Finalise concept and game rules | 2 | End Week 1 | None |Done |
| T2 | Complete BOM and source materials | 1 | End Week 1 | T1 | Done |
| T3 | Test ESP32 touch pads and LED strips | 2 | End Week 1 | T1 | Done |
| T4 | Design and fabricate building structure | 4 | End Week 2 | T1 | To Do |
| T5 | Write and test full game code | 4 | End Week 2 | T3 | Done |
| T6 | Integrate electronics into structure | 4 | End Week 3 | T4, T5 | To Do |
| T7 | Playtest with peers and refine | 2 | End Week 3 | T6 | To Do |
| T8 | Refine, document, and finalise README | 3 | End Week 4 | T7 | To Do |

## 13.3 Responsibility Split - not applicable (working individually)

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
- [/] Idea finalized
- [/] Core interaction decided
- [ ] Sketches made
- [/] BOM completed
- [/] Purchase needs identified
- [ ] Key uncertainty identified
- [/] Basic feasibility tested

### Week 2 — Build Subsystems
Expected outcomes:
- [/] Electronics tests completed
- [ ] CAD / structure planning completed
- [ ] App UI started if needed
- [ ] Mechanical concept tested
- [ ] Main subsystems partially working

### Week 3 — Integrate
Expected outcomes:
- [-] Physical body built
- [/] Electronics integrated
- [/] Code connected to hardware
- [ ] App connected if required
- [ ] First playable version exists

### Week 4 — Refine and Finish
Expected outcomes:
- [/] Technical bugs reduced
- [/] Playtesting completed
- [/] Improvements made
- [/] Documentation completed
- [/] Final build ready

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

vid link: https://www.instagram.com/reel/DXkhksPz1QL/?igsh=MWM2b2d2cmlmODFjeQ==

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
