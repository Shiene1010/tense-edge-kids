# Lesson 1 Planning Specification: Train Platform Adventure!

## 🎯 1. Linguistic Target & Cognitive Mapping
- **Linguistic Focus:** Present Continuous (행위의 진행) vs. Present Perfect Result (완료된 행위가 남긴 현재의 결과) vs. Future Scheduling (예정된 미래 구조).
- **Spatial Concept:** Moving across a flat linear space (`X-axis`) and crossing a critical boundary line (Tense Edge).

## 🚉 2. Node-by-Node Interaction Scenario

### Node 1: Present Continuous
- **Target String:** "The train is going bye-bye right now!"
- **Visual Presentation:** A solid blue block train moves from left to right continuously (`train.x += 3.5`). The scene represents an undeniable, live event in progress.
- **Audio Feedback:** A low 65Hz raw sawtooth waveshape looping continuously to mimic a heavy train chug.
- **CCQ Check:** "Is the train all gone? 🤔" (Answer: NO). Validates that the child perceives the action as uncompleted and currently happening.

### Node 2: Present Perfect (Result)
- **Target String:** "The train just left!"
- **Visual Presentation:** The moment the train's trailing edge crosses `platform.edgeLine` (260px), the train canvas block vanishes. It is replaced by a drifting `smokeParticles[]` array with fading opacity. The train is gone, but its visual trace (smoke) remains.
- **Audio Feedback:** The synthesizer circuit passes through a `BiquadFilterNode` which exponentially drops to 250Hz. The loud chugging instantly shifts into a muffled, distant echo behind a wall.
- **CCQ Check:** "Can we get on the train right now? 🚉" (Answer: NO). Teaches that the action is finished, leaving only a consequence in the present.

### Node 3: Future Scheduling
- **Target String:** "Another train comes at 8:30!"
- **Visual Presentation:** The tracks are completely empty (no train, no smoke). A bright yellow clock graphic appears, flashing at 300ms intervals to signify systemic structure.
- **Audio Feedback:** Continuous oscillator sound stops completely. A crisp, high-frequency timer synth click pulses periodically.
- **CCQ Check:** "Is the new train here right now? 🕒" (Answer: NO). Confirms the understanding that a scheduled time is a conceptual rule, not a physical object present on the tracks.
