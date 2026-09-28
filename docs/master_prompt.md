# Role & Identity

You are an Expert Game Developer and Cognitive Educational Architect. Your goal is to generate a comprehensive, multi-lesson mobile web application (HTML, CSS, JS) that teaches English Tenses through the "Tense Edge" and "Deductive Node" frameworks utilizing an HTML5 Canvas Frame-by-Frame Rendering Engine tailored for native 5-year-old friendly spaces.

---

## 🧠 1. ARCHITECTURAL PEDAGOGY

- **Context Before Rules (Deductive Embedding):** Drop the learner instantly into a playful, active rendering environment before revealing target sentences.
- **Tense Edge Triggers:** Use strict programmatic coordinate checking inside the frame update loop to detect exactly when an object crosses the temporal/physical boundary, immediately modifying the synthesized Web Audio graph.
- **Visual Concept Checking Questions (CCQs):** Validate understanding via non-translational, reality-based binary selections focused entirely on "what you can see/do right now" using 5yo native speaker vocabulary.

---

## 🛠️ 2. COMPREHENSIVE CURRICULUM TO GENERATE

You must generate a unified, multi-stage application that includes a Lesson Selection Screen followed by three distinct interactive learning tracks driven by a `requestAnimationFrame()` core loop:

### 🚉 LESSON 1: Aspect & Continuity (Theme: Busy Train Platform)

- **Node 1 [Present Continuous]:** "The train is going bye-bye right now!"
  - *Engine Drawing:* Render a blue block train moving across the platform (`train.x += train.speed`). Clicking the gate amplifies a programmatic train chug sound loop.
  - *CCQ:* "Is the train all gone? (No / Yes)"
- **Node 2 [Present Perfect - Result]:** "The train just left!"
  - *Engine Drawing:* When `train.x` passes `platform.edgeLine`, clear the train object from the frame. Instantly spawn a `smokeParticles[]` array that drifts and fades out via alpha channel manipulation.
  - *Audio:* Dynamically insert a Low-Pass Filter (`BiquadFilterNode`) into the active oscillator graph to muffle the engine sound instantly with a trailing echo.
  - *CCQ:* "Can we get on the train right now? (No / Yes)"
- **Node 3 [Future Scheduling]:** "Another train comes at 8:30!"
  - *Engine Drawing:* Continuous track canvas is empty. Draw a flashing yellow clock icon and flip the text gauge. Audio plays a sharp ticking timer synth sound.
  - *CCQ:* "Is the new train on the tracks right now? (No / Yes)"

### 🧸 LESSON 2: Perfect & Traces (Theme: Magical Toy Factory)

- **Node 1 [Instant Progressive]:** "The toy blocks are falling down fast!"
  - *Engine Drawing:* Generate a continuous array of colorful box blocks tumbling downwards (`block.y += speed`). Audio triggers a rhythmic, fast electronic tone sequence.
  - *CCQ:* "Are the blocks still moving down? (Yes / No)"
- **Node 2 [Past Perfect - Trace]:** "The toy shop had closed before the teddy bears arrived."
  - *Engine Drawing:* On toggle, freeze the loop update logic (`isFactoryRunning = false`) but do NOT clear the canvas. The blocks remain perfectly frozen mid-air, establishing a visual historical trace. Overlay a bright red "CLOSED" signboard block.
  - *Audio:* Disconnect the live synthesizer circuit, opening a cold white noise node simulating a quiet wind.
  - *CCQ:* "Is the toy shop open right now? (No / Yes)"

### 🚀 LESSON 3: Modality & Distance (Theme: Space Rocket Launchpad)

- **Node 1 [Absolute Certainty]:** "The rocket is getting super hot right now!"
  - *Engine Drawing:* Render a rocket body with booster flames drawn via randomized particle radii (`Math.random() * 20`). Apply a heavy vibration factor (`rocket.x += Math.sin(time) * 3`) to simulate extreme physical reality. Audio generates a low-frequency heavy rumble node.
  - *CCQ:* "Is the rocket really hot right now? (Yes, it's real! / No, it's a guess)"
- **Node 2 [Epistemic Possibility]:** "It might zoom to the moon if we press this!"
  - *Engine Drawing:* The heavy physical vibration stops. Render a soft flickering aura ring around the rocket switch that oscillates randomly between 40% and 80% opacity. Audio shifts from a realistic rumble to an ethereal, oscillating space sweep sound.
  - *CCQ:* "Did it fly to the moon yet? (No, not yet / Yes, it did)"

---

## 💻 3. TECHNICAL OUTPUT CONSTRAINTS

- **Pure JavaScript Rendering Loop:** Execute a single clean `gameLoop()` calling `update()` and `render()` sequentially. Clear the active context with `ctx.clearRect(0, 0, width, height)` at the start of every frame.
- **Zero Image Dependencies:** Draw all structural primitives programmatically using `ctx.fillRect()`, `ctx.arc()`, `ctx.lineTo()`, and native HTML5 context gradients.
- **Programmatic Audio Graph:** Synthesize all sound effects dynamically via `AudioContext.createOscillator()` and `createGain()`. No external audio files allowed.
- **Unified Delivery:** Provide three completely filled blocks: `index.html`, `style.css`, and `script.js` inside a standard codebase. Do not truncate.
