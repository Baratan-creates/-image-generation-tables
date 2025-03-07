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
This project is in **early development status**. This means that the basic catalogue of data has not yet been converted to the appropriate format for this website.

## Language Model Evaluations
**Score** Language Model Creative Writing Scoring Index
Langage models are scored based on `compliance, comprehension, coherence, creativity and realism.

| Model | Score | Size | Quant Tested | Template |
|:-----------|:---:|:---:|:---:|:---:|
| Example #1 | 100 | 12B | EXL2 | Mistral |
| Example #2 | 75 | 12B | Q5_K_M | ChatML |
| Example #3 | 50 | 8B | Q4_K_M | ChatML |

## Image Model Parameter Evaluation
Rather than trying to rank image generation models based on subjective opinions I will record how the different parameters affect the outcome of the generation, hopefully allowing viewers to tweak their generations more to their liking. 
I will produce and publish image generations grids for the following parameters. 

**Generation Time** Records an average generation time on a RTX3080 GPU using listed parameters.

**Styles** counts the number of styles the model can produce naturally (anime, photo, 3d rendering, hyperrealism). 

**Name Recognition** Indicates whether or not an image generation model can produce recognizable lickeness of named figures. 

**Characters** Indicates whether or not the model can generate images of common fictional characters without a lora or descriptive text.

### Image Models
| Model | Resolution | Steps | CFG | Sampler | Scheduler | Generation Time | Styles | Name Recognition | Characters | Text |
|:-----------|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| Flux.schnell <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation/Flux.Schnell.png?raw=true" width="256">| 1024x1024 | 4 | 1 | Euler | Beta | 9.72s |  | No | No | Yes |
| Flux.Dev <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation/Flux.Dev.png?raw=true" width="256">| 1024x1024 | 30 | 1 | Euler Ancestral | Beta | 64.78s |  | No | Yes | Yes |
| Stable-Diffusion 1.5 <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation/SD1.5.png?raw=true" width="256">| 512x512 | 30 | 6 | DPM++ 2M SDE | SGM Uniform | 2.42s | | Yes | Yes | No |
| Stable-Diffusion XL (SDXL) <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation/SDXL.png?raw=true" width="256">| 1024x1024 | 30 | 5 | DPM++ SDE | SGM Uniform | 14.39s | | Yes | Yes | No |
| Pony (SDXL) | 1024x1024 | 20 | 5 | DPM++ SDE | SGM Uniform | 10.0s |
| Illustrious (SDXL) | 1024x1024 | 20 | 5 | DPM++ SDE | SGM Uniform | 10.0s |
| Stable-Diffusion 3 | 1024x1024 | 20 | 5 | DPM++ SDE | SGM Uniform | 30.0s |
| Stable-Diffusion 3.5 Medium <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation/SD3.5Medium.png?raw=true" width="256"> | 1024x1024 | 30 | 5 | Euler | Normal | 15.34s | | No | Yes | Yes |
| Stable-Diffusion 3.5 Medium Tensor-Art TurboX <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation/SD3.5MediumTurbo.png?raw=true" width="256"> | 1024x1024 | 8 | 1.5 | Euler Ancestral | Beta | 4.83s | | No | Yes | No |
| Stable-Diffusion 3.5 Large <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation/SD3.5Large.png?raw=true" width="256">| 1024x1024 | 30 | 5 | Euler Ancestral | Normal | 49.64s | | Yes | Yes | Yes |
| Stable-Diffusion 3.5 Large Tensor-Art TurboX <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation/SD3.5LargeTurbo.png?raw=true" width="256"> | 1024x1024 | 8 | 1.5 | Euler | Normal | 15.75s | | Yes | Yes | Yes |
| Wan Text-To-Video 1.3B <img src="https://github.com/Baratan-creates/-image-generation-tables/raw/refs/heads/main/Image-Generation/wan-text-to-image-1.3b.webp" width="256"> | 640x640 | 40 | 5 | Euler Ancestral | Beta | 71.00s |
| Wan Text-To-Video 14B <img src="https://github.com/Baratan-creates/-image-generation-tables/raw/refs/heads/main/Image-Generation/wan-text-to-image-14b.webp" width="256"> | 640x640 | 40 | 5 | Euler Ancestral | Beta | 8.45m | | | | Yes |
| Wan Image-To-Video 14B - 480p | 640x640 | 20 | 5 | Euler Ancestral | Beta | 120.0s |
| Wan Image-To-Video 14B - 720p | 960x960 | 20 | 5 | Euler Ancestral | Beta | 340.0s |

### Image Styles
While there are thousands of styles that apply to image generation models. It is important to know which *basic* styles a model can produce before narrowing in on a specific artist or sub-style such as *cinematic film still*, or *analog film photo*. In the basic evaluation, I test to see whether or not an image model is capable of creating images in basic styles. Anime/Cartoon, Photorealistic, 3D Rendering, Hyperrealism/2.5D Art

| Style | Thumb | Sample Prompt |
|:-----------|:---:|:---:|
| Anime/Cartoon | <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation/anime_artwork.png?raw=true" width="256"> | anime artwork illustration of a cat in a magical rainbow forest |
| Photorealistic | <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation/cinematic_film.png?raw=true" width="256"> | cinematic film still of a cat in a magical rainbow forest |
| 3D Rendering | <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation/3d_rendering.png?raw=true" width="256"> | in-game 3d rendering of a cat in a magical rainbow forest |
| Hyperrealism/2.5D Art | <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation/hyperrealistic_art.png?raw=true" width="256"> | hyperrealistic art of a cat in a magical rainbow forest |
