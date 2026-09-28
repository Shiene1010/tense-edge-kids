# Lesson 2 Planning Specification: Magical Toy Factory

## 🎯 1. Linguistic Target & Cognitive Mapping
- **Linguistic Focus:** Progressive Reality (현재 진행형의 물리적 현실) vs. Past Perfect Trace (대과거 완료 상태가 남긴 고정된 과거의 흔적) vs. Conditional Forecast (조건부 미래 예측).
- **Spatial Concept:** Vertical descending objects (`Y-axis`) and sudden environmental freeze (Temporal Arrest).

## 🧸 2. Node-by-Node Interaction Scenario

### Node 1: Progressive Reality
- **Target String:** "The toy blocks are falling down fast!"
- **Visual Presentation:** Multiple colorful rectangular block arrays tumble down continuously down the dark conveyor belt. If a block leaves the viewport bottom, it wraps back to the top with randomized colors.
- **Audio Feedback:** Rhythmic 440Hz triangle oscillator melody playing at a rapid pace, representing a busy, operational factory line.
- **CCQ Check:** "Are the blocks still moving down? 🧸" (Answer: YES). Reinforces live progressive motion.

### Node 2: Past Perfect (Trace)
- **Target String:** "The toy shop had closed before the teddy bears arrived."
- **Visual Presentation:** After a 3-second countdown (`spawnTimer > 180`), the physics update loop forces `toyFactory.isRunning = false`. The blocks instantly freeze solid mid-air. A large red "CLOSED" warning sign is rendered across the screen. The frozen blocks stand as a visual historical monument of an action completed prior to another event.
- **Audio Feedback:** The live musical synthesizer sequence cuts out completely, replaced by a low, hollow wind noise node at 150Hz.
- **CCQ Check:** "Is the toy shop open right now? 🚪" (Answer: NO). Demonstrates that the state of being closed happened in the past and remains absolute.

### Node 3: Conditional Forecast
- **Target String:** "The lights might flash if it gets too busy."
- **Visual Presentation:** The frozen factory interface remains, but a translucent warning aura layer starts ambiently pulsing near the top control board.
- **Audio Feedback:** Intermittent, gentle chime sound patterns blended into the wind noise.
- **CCQ Check:** "Are the lights flashing right now? 💡" (Answer: NO). Explores epistemic uncertainty—something that is possible under conditions but not an active present fact.
