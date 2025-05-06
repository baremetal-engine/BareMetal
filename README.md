# BareMetal Engine
**Neo, what if I told you... you could ship AAA visuals on a toaster?**

> **Modern GPUs are 95% useless.**  
> Because 95% of what they render is *never seen* by the player.

**BareMetal** is a new kind of game engine built on a forgotten truth:
You don’t need more power—you need **more control**.

While the industry races to brute-force photorealism through expensive GPUs,  
we use perceptual rendering, smart baking, and AI-assisted authoring to  
create AAA-quality visuals that run on yesterday’s hardware—and still look better.

---

## 🔗 Source Code  
👉 [baremetal-engine-core (Godot fork)](https://github.com/baremetal-engine/baremetal-engine-core)

---

## 🎯 The Objective

Run photorealistic graphics on original PS2 hardware by shifting the burden of rendering from the GPU to the game engine.

Instead of brute-forcing visuals at runtime, we precompute everything the player will see—so the GPU does less, and the game looks better.

---

## 🔧 What Is BareMetal?
**BareMetal** is an open-source, ultra-optimized game engine **forked from Godot** with a radical goal:

> Run photorealistic graphics on the lowest possible hardware — and expose the industry's obsession with GPU bloat.

---

## The Problem: How Power Killed Progress

For decades, we’ve been sold a lie:

That in order to achieve better graphics, we need **bigger GPUs**.  
More cores. More memory. More power.

Meanwhile, game engines have grown **bloated**, **inefficient**, and **dependent**.  
Developers offload lighting, shadows, reflections—even resolution—onto the GPU at runtime, instead of building these effects intelligently into the game itself.

This is not innovation.  
This is _**laziness by design**_ — and it’s killing creativity.

- **AMD and NVIDIA** grow profits  
- **Sony, Microsoft, and Nintendo** build “more powerful” consoles  
- **Developers** get lazier  
- **Engines** grow slower  
- **Players** get locked into an upgrade cycle they can’t afford

All while **90% of what’s rendered is invisible to the human eye.**

### This is the feedback loop we are breaking.

We believe that true advancement comes not from **brute-forcing hardware**,  
but from **mastering the engine**.

The game engine should be the source of **illusion** and **artistry** — not the GPU.

> You wouldn’t build a bigger car engine before optimizing the fuel.  
>  
> So why are we maxing out GPUs before maxing out the game engine?

---

## The Solution: Perceptual Rendering

The game industry has been brainwashed.

Big corporations like **AMD** and **NVIDIA** have convinced developers that modern games need things like **Ray Tracing**, **DLSS**, **FSR**, **Tessellation**, and a dozen other buzzwords to achieve "superior" graphics.

But here’s the truth no one talks about:

> **Up to 95% of what the GPU processes is never even seen by the player.**

So why are we wasting power simulating lighting, shadows, and reflections the human eye can’t perceive?

### Perceptual Rendering fixes this.

Perceptual Rendering is not a new idea—it’s how games were built from the PS2 era through the early 2010s:
- Lighting was **baked**
- Effects were **faked**
- Visuals were **crafted for perception, not simulation**

BareMetal revives this philosophy and supercharges it.

We’re forking the Godot engine to build **simple, developer-friendly tools** that let you:
- **Bake in lighting, shadows, reflections, fog, and polish**
- Use **AI-assisted workflows** to handle detail generation and optimization
- Maintain **full artistic control** over what the player sees—without burdening the GPU

### 🎨 What BareMetal Unlocks
- Build in any style—2D, 3D, stylized, or photoreal
- Focus on storytelling, aesthetics, and gameplay—not rendering hacks
- Let AI handle the grunt work while you refine the vision
- Ship a high-performance game without compromising the soul

Instead of relying on bloated real-time effects, BareMetal shifts the workload back to the **game engine**, where it belongs.
The result: stunning, photorealistic visuals that run on older hardware—with no compromise in quality.

> The GPU should display the illusion—not calculate it.

---

### 🧠 The Paradigm Shift: Code Over Consumption

Instead of a hardware arms race, we’re creating a **code race**:
- Who can write the most elegant, efficient, and performant engine?
- Who can help the most people game and build without gatekeepers?
- Who can liberate the next generation of devs from GPU dependence?

The answer won’t come from billion-dollar boardrooms.  
It will come from **millions of developers** uniting behind one idea:  
> **Make high-end graphics possible for everyone, on any machine.**

### ⚖️ The Two Paradigms

| **The Current Paradigm**                                     | **The New Paradigm**                                               |
|--------------------------------------------------------------|----------------------------------------------------------------------|
| Graphics improve → **GPUs must become more powerful**        | Graphics improve → **Engines must become more optimized**           |
| More power = more heat, more cost, more e-waste              | Smarter code = same graphics on cheaper hardware                    |
| Indie devs pushed out by hardware demands                    | Indie devs empowered to build AAA-tier games                        |
| Gamers forced to upgrade hardware                            | Gamers play on what they already have                               |
| Corporations profit through dependence                       | Developers and players win through freedom                          |

---

### 🌎 Why Everybody Wins

- 💸 **Gamers** save money — no more forced upgrades.
- 🚀 **Indie developers** build stunning games without licensing fees or AAA pipelines.
- 🌍 **Global access** expands — beautiful games, even on modest machines.
- 🔌 **Environmental impact** shrinks — less e-waste, less power draw.
- 🛠 **Engineering is reborn** — from brute-force back to craftsmanship.

---

BareMetal isn’t just an engine.  
It’s a rebellion.  
It’s a correction.  
It’s the beginning of the end for GPU tyranny.

**Join us. Optimize everything. Outcode everyone. Build the future.**

### 🔥 Our Mission

The modern gaming industry has locked photorealism behind $1,000 GPUs and wasteful engines. We believe:

- Optimization is more powerful than hardware.
- Photorealism should be possible on a PS2.
- Game engines should empower creators — not gatekeep them.
- The upgrade treadmill is a lie. **Let’s prove it.**

### 💡 Key Goals

- Strip Godot to the bone and optimize for *performance-first*.
- Deliver playable demos with AAA visuals on mid-tier GPUs.
- Build a contributor community of rebels, engineers, and artists.
- Make the industry admit the truth: **your hardware was never the problem.**

### 🛠 Want to Help?

We're looking for:

- Engine contributors (C++, Rust, Godot hackers)
- Shader optimization experts
- 3D artists who love performance
- Indie devs tired of Unity/Unreal lies
- Philosophers of efficient design

## 📖 Learn More

- 🧠 [Philosophy](PHILOSOPHY.md): Understand the cultural and technical roots of BareMetal.
- 🎯 [Vision](VISION.md): See where we’re headed and what success looks like.
- 🛠️ [Governance](GOVERNANCE.md): How decisions are made, who leads, and how leadership is earned.
- 📄 [GPU Gimmicks vs. Perceptual Rendering](GPU-Gimmick-Breakdown.md): Why modern GPUs are 95% useless.


---
> **Photorealism isn’t about more power. It’s about less waste.**

---

## 🚀 The Next Frontier: AI-Powered Game Optimization

> ⚠️ We believe AI should accelerate creativity—not replace it.
>
> That's why BareMetal is open-source.  
> So no company can quietly give AI creative control, and no artist can be silently replaced.
>
> Our tools are transparent, developer-controlled, and opt-in.  
> Because illusion should be engineered by humans—not dictated by machines.

Once we’ve proven that photorealism can run on a PS2, we’re not stopping—we’re scaling.

Our next goal is to build a toolchain that lets developers take **older games**—from any era—and run them through an **AI-powered visual optimizer** that:

- Replaces real-time effects with perceptually baked equivalents
- Suggests performance-saving approximations
- Auto-generates lighting, AO, reflections, and fog using perceptual models
- Outputs a visually upgraded version that runs better than the original

> Drop in an old game. Let AI do the grunt work. Polish it by hand. Ship something timeless.

Whether it's a GameCube-era classic or a Unity prototype from 2016—**we want to make it look better and run faster than ever.**

**This is not just about making new games.  
It’s about *preserving and upgrading everything we already built*—the right way.**


## 👤 Author & Founder

This project was created and is maintained by **Trevor Honer**.  
Feel free to reach out or follow the mission on GitHub.

[GitHub Profile »](https://github.com/baremetal-engine)

