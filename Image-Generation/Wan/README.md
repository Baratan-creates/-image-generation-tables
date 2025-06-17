# Wan Lora Comparison
**Each** gen has the lora and generation time listed. The following parameters were used. 
**All:** Prompt: "She smiles and eats a banana.", Sampler: Euler, Scheduler: Simple, Resolution: 480x480
**No Lora:** 20 video steps, 5 CFG, 16 FPS, 64 Frames
**Lora:** 5 video steps, 1 CFG, 24 FPS, 124 Frames

|     No Lora      | LightX2v | FusionX  | CauseVid | +MoviiGen | +AccVid  | +AccVid / +MoviiGen | CauseVid V2 |
| :--------------: | :------: | :------: | :------: | :-------: | :------: | :-----------------: | :---------: |
|     9.70 min     | 2.18 min | 2.06 min | 2.07 min | 2.12 min  | 2.12 min |      1.12 min       |  2.27 min   |
| <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation/Wan/No_Lora.webp?raw=true" width="256"> | <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation/Wan/LightXv2.webp?raw=true" width="256"> | <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation/Wan/FusionX.webp?raw=true" width="256"> | <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation/Wan/CauseVid.webp?raw=true" width="256"> | <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation/Wan/MoviiGen.webp?raw=true" width="256"> | <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation/Wan/AccVid.webp?raw=true" width="256"> | <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation/Wan/MoviiGen-AccVid.webp?raw=true" width="256"> | <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation/Wan/CauseVidV2.webp?raw=true" width="256"> |
>+ Indicates with CauseVid
>All generation done in SwarmUI
