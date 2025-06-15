# Image & Language-Generation-Tables
Researching and cataloging generative ai image parameters and language model (LLM) creative writing and comprehension.
## Table of Contents
- [Image & Language-Generation-Tables](#image--language-generation-tables)
- [Status](#status)
- [Language Model Evaluations](#language-model-evaluations)
  - [Language Models](#language-models)
- [Image Model Parameter Evaluation](#image-model-parameter-evaluation)
  - [Image Models](#image-models)
  - [Image Styles](#image-styles)
## Status
This project is in **early development status**.

## Language Model Evaluations
[https://github.com/Baratan-creates/-image-generation-tables/blob/3ebbbeef96040f1f1d4a6e08ae252010ddd95aea/Language%20Models/readme.md]()

## Image Model Parameter Evaluation
Rather than trying to rank image generation models based on subjective opinions I will record how the different parameters affect the outcome of the generation, hopefully allowing viewers to tweak their generations more to their liking. 
I will produce and publish image generations grids for the following parameters. 

**Generation Time** Records an average generation time on a RTX3080 GPU using listed parameters.

**Styles** counts the number of styles the model can produce naturally (anime, photo, 3d rendering, hyperrealism). 

**Name Recognition** Indicates whether or not an image generation model can produce recognizable likeness of named figures. 

**Characters** Indicates whether or not the model can generate images of common fictional characters without a lora or descriptive text.

### Image Models
| Model | Resolution | Steps | CFG | Sampler | Scheduler | Generation Time | Styles | Name Recognition | Characters | Text |
|:-----------|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| Flux.schnell <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation/Flux.Schnell.png?raw=true" width="256">| 1024x1024 | 4 | 1 | Euler | Beta | 9.72s |  | 0/5 | 2/5 | Yes |
| Flux.Dev <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation/Flux.Dev.png?raw=true" width="256">| 1024x1024 | 30 | 1 | Euler Ancestral | Beta | 64.78s |  | 0/5 | 2/5 | Yes |
| Stable-Diffusion 1.5 <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation/SD1.5-original.png?raw=true" width="256">| 512x512 | 30 | 6 | DPM++ 2M SDE | SGM Uniform | 2.42s | | 5/5 | 2/5 | No |
| Stable-Diffusion XL (SDXL) <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation/SDXL.png?raw=true" width="256">| 1024x1024 | 30 | 5 | DPM++ SDE | SGM Uniform | 14.39s | | 5/5 | 4/5 | No |
| <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation/2dnPony.png?raw=true" width="256"> PONY (SDXL) | 1024x1024 | 20 | 5 | DPM++ SDE | SGM Uniform | 10.0s | | 2/5 | 3/5 | |
| Illustrious (SDXL) <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation/%CE%A3%CE%99%CE%97.png?raw=true" width="256"> | 1024x1024 | 20 | 5 | DPM++ SDE | SGM Uniform | 10.0s | | | 5/5 | |
| Stable-Diffusion 3 | 1024x1024 | 20 | 5 | DPM++ SDE | SGM Uniform | 30.0s |
| Stable-Diffusion 3.5 Medium <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation/SD3.5Medium.png?raw=true" width="256"> | 1024x1024 | 30 | 5 | Euler | Normal | 15.34s | | No | 4/5 | Yes |
| Stable-Diffusion 3.5 Medium Tensor-Art TurboX <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation/SD3.5MediumTurbo.png?raw=true" width="256"> | 1024x1024 | 8 | 1.5 | Euler Ancestral | Beta | 4.83s | | No | 4/5 | No |
| Stable-Diffusion 3.5 Large <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation/SD3.5Large.png?raw=true" width="256">| 1024x1024 | 30 | 5 | Euler Ancestral | Normal | 49.64s | | Yes | 4/5 | Yes |
| Stable-Diffusion 3.5 Large Tensor-Art TurboX <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation/SD3.5LargeTurbo.png?raw=true" width="256"> | 1024x1024 | 8 | 1.5 | Euler | Normal | 15.75s | | Yes | 4/5 | Yes |
| Wan Text-To-Video 1.3B <img src="https://github.com/Baratan-creates/-image-generation-tables/raw/refs/heads/main/Image-Generation/wan-text-to-image-1.3b.webp" width="256"> | 640x640 | 40 | 5 | Euler Ancestral | Beta | 71.00s | | | 0/5 | |
| Wan Text-To-Video 14B <img src="https://github.com/Baratan-creates/-image-generation-tables/raw/refs/heads/main/Image-Generation/wan-text-to-image-14b.webp" width="256"> | 640x640 | 40 | 5 | Euler Ancestral | Beta | 8.45m | | | 2/5 | Yes |
| Wan Image-To-Video 14B - 480p <img src="https://github.com/Baratan-creates/-image-generation-tables/raw/refs/heads/main/Image-Generation/wan-text-to-image-14b.webp" width="256"> | 640x640 | 20 | 5 | Euler Ancestral | Beta | 120.0s | N/A | N/A | N/A |
| Wan Image-To-Video 14B - 720p <img src="https://github.com/Baratan-creates/-image-generation-tables/raw/refs/heads/main/Image-Generation/wan-text-to-image-14b.webp" width="256"> | 960x960 | 20 | 5 | Euler Ancestral | Beta | 340.0s | N/A | N/A | N/A |

### Image Styles
While there are thousands of styles that apply to image generation models. It is important to know which *basic* styles a model can produce before narrowing in on a specific artist or sub-style such as *cinematic film still*, or *analog film photo*. In the basic evaluation, I test to see whether or not an image model is capable of creating images in basic styles. Anime/Cartoon, Photorealistic, 3D Rendering, Hyperrealism/2.5D Art

| Style | Thumb | Sample Prompt |
|:-----------|:---:|:---:|
| Anime/Cartoon | <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation/anime_artwork.png?raw=true" width="256"> | anime artwork illustration of a cat in a magical rainbow forest |
| Photorealistic | <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation/cinematic_film.png?raw=true" width="256"> | cinematic film still of a cat in a magical rainbow forest |
| 3D Rendering | <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation/3d_rendering.png?raw=true" width="256"> | in-game 3d rendering of a cat in a magical rainbow forest |
| Hyperrealism/2.5D Art | <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation/hyperrealistic_art.png?raw=true" width="256"> | hyperrealistic art of a cat in a magical rainbow forest |
