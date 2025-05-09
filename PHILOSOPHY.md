# The BareMetal Philosophy

## 🎯 Prime Directive

> **To run photorealistic graphics on the lowest possible GPU. Always.**

Every line of code, every asset decision, every rendering pipeline in this engine exists to serve this one goal.

---
## 1. What Actually Makes Graphics Look Photorealistic

Modern games often chase photorealism using brute-force GPU computation — but the truth is, **perceptual realism** (what *humans actually see*) is the key. The BareMetal engine is built around this idea: **optimize only the variables that contribute to visual immersion.**

Below are the core variables that create the illusion of realism:

| Variable                          | Why It Matters                                                                 |
|----------------------------------|--------------------------------------------------------------------------------|
| Lighting Direction & Softness    | Humans are extremely sensitive to light source direction, diffusion, and contrast. Poor lighting immediately breaks immersion. |
| Shadow Placement & Blur          | Hard shadows look fake. Soft, dynamically placed shadows increase depth perception and spatial realism. |
| Surface Reflectivity (Specular)  | Our brains distinguish materials through specular response. Correct specular > high resolution. |
| Material Response (PBR)          | Simulates how surfaces reflect/absorb light realistically — even at low polycounts. |
| Global Illumination Approximation| Full light bounces aren't needed. The brain is easily tricked by ambient occlusion/fake GI. |
| Color Grading & Tone Mapping     | Mimics eye adaptation and cinematic tone shifts, which boosts realism.         |
| Camera Effects (DOF, etc.)       | Subtle lens tricks (grain, DOF, aberration) convince the brain it's real.      |
| Motion Blur                      | Smoothed blur mimics natural perception of motion — useful in fast gameplay.   |
| Real-World Scale & Perspective   | Proper object sizing and FOV help players feel grounded inside the world.      |
| Temporal Stability               | Prevents frame-to-frame flicker and pop-in. Visual stability feels "real."    |

These are the **only things that matter** for human-perceived realism.

---

## 2. Why AMD/NVIDIA Buzzwords Are Mostly Wasteful

The GPU industry thrives on hype: every year, new marketing terms like **"Ray Tracing"**, **"DLSS"**, and **"8K Textures"** are sold as revolutionary. But:

| Technique                        | Why It’s Ineffective or Wasteful                                              |
|----------------------------------|--------------------------------------------------------------------------------|
| Ray Tracing Everywhere           | Eye can’t detect multi-bounce lighting in fast gameplay. Most GI can be faked cheaper with no perceptual loss. |
| 8K Textures                      | Human eyes can't resolve the difference past 2K at gameplay speed. The extra GPU strain is pointless. |
| DLSS/FSR                         | These upscalers fix problems caused by over-rendering. BareMetal avoids the problem in the first place. |
| Volumetric Clouds & Fog          | Looks great in trailers. Usually has zero gameplay impact and drains performance. |
| Subsurface Scattering on Everything | Only needed for skin and wax-like materials. Often wasted on irrelevant objects. |

### BareMetal’s Stance:
> We will still achieve **eyecandy** — but every frame will be **lean, intentional, and perceptually optimized**.

---

# The 95% Rendering Waste Problem

## Why Most of What GPUs Render Is Never Seen

### 1. Biological Limits of Human Perception
- Motion perception caps at ~60–90 FPS.
- Visual acuity sharply drops outside the central 60° field of vision.
- Eye can’t distinguish subtle lighting or texture differences during fast motion.

### 2. Compression Algorithms Prove It
- H.264, H.265, AV1 compress video by **90–95%** with *no perceptual loss*.
- That proves most visual data is unnecessary for human perception.

### 3. Overdraw and Redundant Computation
- Engines redraw the entire screen every frame — even if 90% is unchanged.
- Shadows, light bounces, and reflections often update pointlessly.

### 4. Ray Tracing is Largely Wasted
- Secondary light bounces and ultra-detailed reflections often fall outside player focus.
- These are simulated at massive computational cost — with **no perceived difference**.

### 5. LOD and Mipmap Levels Are Already an Admission
- Engines reduce quality based on distance/focus — proving that full detail isn’t needed.
- BareMetal embraces and perfects this logic, instead of hiding it.

---

## BareMetal’s Conclusion
> If only 5–10% of the pixels and computations matter to the human experience, then 90–95% of modern GPU effort is wasted. We’re not lowering the bar. We’re building the most perceptually efficient renderer ever made.

This is how you get **jaw-dropping graphics** without next-gen hardware — by mastering what the *player* actually sees.

---

## ⚔️ The Problem

Modern game engines are bloated. They’re optimized for silicon, not for users. The result?

- Beautiful games that run like garbage on anything but the latest GPU
- Indie devs locked out by complexity and cost
- Forced obsolescence every 2–3 years
- An industry built on fake “progress”

This isn’t innovation. It’s manipulation.

---

## 🔁 The New Trajectory

> The gaming industry pushes the limits of **hardware**.  
> **We push the limits of the engine.**

What Unreal and Unity do with 4080s, we aim to do with 1060s.  
And every time we succeed, we break the illusion that you need more power to have better games.

---

## 🤖 AI and the Future of Optimization

BareMetal welcomes the use of AI tools to accelerate engine development, testing, and performance tuning — **not to replace developers**, but to empower them.

We believe AI is a key ally in:
- Writing efficient boilerplate code
- Prototyping systems rapidly
- Benchmarking and stress-testing builds
- Refactoring bloated logic into lean, elegant solutions

As long as the resulting code honors the philosophy of **efficiency, decentralization, and accessibility**, we encourage AI-assisted contributions.

Smarter code is the mission — and AI is one more tool to get there faster.

---

## 🚀 Why Open Source?

- So no corporation can claim or lock away our tools
- So anyone, anywhere, can contribute or build with it
- So we can prove — in public — what they told you was impossible

---

## 🧠 This Is More Than a Project

This is a **rebellion**.  
This is a **correction**.  
This is a **liberation of gaming** from the hardware treadmill.

We’re not trying to match the industry.  
We’re trying to **reverse its trajectory**.

---

## 📢 Call to Action

- Fork this engine.
- Help us strip it down and sharpen its edge.
- Build a demo that makes the world ask: *“Why does this run better on a 2016 card than modern AAA games?”*

If you’ve ever stared at a stuttering menu and thought:
> *“Why is this slow on a $2,000 PC?”*

You belong here.

---

## ✍️ About the Founder

BareMetal was founded by **Trevor Honer**, a developer, creator, and rebel against hardware tyranny. This project is open to anyone who shares the vision.

---
> **Optimize the fuel, not the engine.**
