## GPU Gimmicks vs. Perceptual Rendering

| **GPU Gimmick**         | **Problem**                                                                 | **Perceptual Rendering Solution**                                |
|-------------------------|------------------------------------------------------------------------------|------------------------------------------------------------------|
| **Ray Tracing (RT)**    | Massive performance cost for subtle lighting details. Most players turn it off. | Baked lighting, reflection probes, and shadow maps achieve 95% of the effect at 5% of the cost. |
| **DLSS / FSR**          | Fixes the performance hit caused by over-rendering in the first place. Adds blur and input lag. | Design the game to *never need it* by targeting native low-cost rendering from the start. |
| **Screen Space AO (SSAO)** | Real-time AO is GPU-heavy and often inaccurate. Over-applied and redundant in static scenes. | Bake AO into textures and vertex colors using AI-enhanced maps. |
| **Volumetric Fog & Lighting** | Simulates complex light scatter. Looks good in stills, often unnoticeable in gameplay. | Use animated fog planes, light shafts, and fullscreen alpha textures where the player actually notices. |
| **Real-Time Global Illumination (Lumen/RTGI)** | Hugely expensive. Rarely impacts fast-paced gameplay. | Combine light probes with AI-baked bounce light textures and lightmass baking. |
| **Tessellation / POM**  | Simulates high geometry depth, but burns performance. Barely noticeable in motion. | Use high-quality normal maps and fake parallax with texture tricks. |
| **Dynamic Shadows**     | Constant CPU/GPU drain for minimal gain in static scenes. | Pre-bake shadows into textures. Use projected decals for dynamic elements. |
| **Realtime Reflections**| Often inaccurate, performance-intensive. Wasteful on matte surfaces. | Use static reflection probes and environment cube maps with fake gloss layers. |
