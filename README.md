# Image & Language-Generation-Tables
Researching and cataloging generative ai image parameters and language model (LLM) creative writing and comprehension.

# Status
This project is in **early development status**. This means that the basic catalogue of data has not yet been converted to the appropriate format for this website.

# Roadmap
I plan on evaluating and cataloging the following sets of data.
**Language Model Evaluations**
**Score** Language Model Creative Writing Scoring Index
Langage models are scored based on `compliance, comprehension, coherence, creativity and realism.

| Model | Score | Size | Quant Tested | Template |
|:-----------|:---:|:---:|:---:|:---:|
| Example #1 | 100 | 12B | EXL2 | Mistral |
| Example #2 | 75 | 12B | Q5_K_M | ChatML |
| Example #3 | 50 | 8B | Q4_K_M | ChatML |

**Image Model Parameter Evaluation**
Rather than trying to rank image generation models based on subjective opinions I will record how the different parameters affect the outcome of the generation, hopefully allowing viewers to tweak their generations more to their liking. 
I will produce and publish image generations grids for the following parameters. 

**Generation Time** Records an average generation time on a RTX3080 GPU using listed parameters.

**Styles** counts the number of styles the model can produce naturally (anime, photo, 3d rendering, hyperrealism). 

**Name Recognition** Indicates whether or not an image generation model can produce recognizable lickeness of named figures. 

**Characters** Indicates whether or not the model can generate images of common fictional characters without a lora or descriptive text.

**Below Grid data without an image is placeholder**
| Model | Resolution | Steps | CFG | Sampler | Scheduler | Generation Time | Styles | Name Recognition | Characters | Text |
|:-----------|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| Flux.schnell <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation/Flux.Schnell.png?raw=true" width="100">| 1024x1024 | 4 | 1 | Euler | Beta | 9.72s |  | No | No | Yes |
| Flux.Dev <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation/Flux.Dev.png?raw=true" width="100">| 1024x1024 | 30 | 1 | Euler Ancestral | Beta | 64.78s |  | No | Yes | Yes |
| Stable-Diffusion 1.5 <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation/SD1.5.png?raw=true" width="100">| 512x512 | 30 | 6 | DPM++ 2M SDE | SGM Uniform | 2.42s | | Yes | Yes | No |
| Stable-Diffusion XL (SDXL) | 1024x1024 | 20 | 5 | DPM++ SDE | SGM Uniform | 10.0s |
| Pony (SDXL) | 1024x1024 | 20 | 5 | DPM++ SDE | SGM Uniform | 10.0s |
| Illustrious (SDXL) | 1024x1024 | 20 | 5 | DPM++ SDE | SGM Uniform | 10.0s |
| Stable-Diffusion 3 | 1024x1024 | 20 | 5 | DPM++ SDE | SGM Uniform | 30.0s |
| Stable-Diffusion 3.5 Medium <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation/SD3.5Medium.png?raw=true" width="100"> | 1024x1024 | 30 | 5 | Euler | Normal | 15.34s | | No | Yes | Yes |
| Stable-Diffusion 3.5 Medium Tensor-Art TurboX <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation/SD3.5MediumTurbo.png?raw=true" width="100"> | 1024x1024 | 8 | 1.5 | Euler Ancestral | Beta | 4.83s | | No | Yes | No |
| Stable-Diffusion 3.5 Large | 1024x1024 | 20 | 5 | Euler | Beta | 60.0s |
| Stable-Diffusion 3.5 Large Tensor-Art TurboX <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation/SD3.5LargeTurbo.png?raw=true" width="100"> | 1024x1024 | 8 | 1.5 | Euler | Normal | 15.75s | | Yes | Yes | Yes |
| Wan Text-To-Video 1.3B <img src="https://github.com/Baratan-creates/-image-generation-tables/raw/refs/heads/main/Image-Generation/wan-text-to-image-1.3b.webp" width="100"> | 640x640 | 40 | 5 | Euler Ancestral | Beta | 71.00s |
| Wan Text-To-Video 14B <img src="https://github.com/Baratan-creates/-image-generation-tables/raw/refs/heads/main/Image-Generation/wan-text-to-image-14b.webp" width="100"> | 640x640 | 40 | 5 | Euler Ancestral | Beta | 8.45m | | | | Yes |
| Wan Image-To-Video 14B - 480p | 640x640 | 20 | 5 | Euler Ancestral | Beta | 120.0s |
| Wan Image-To-Video 14B - 720p | 960x960 | 20 | 5 | Euler Ancestral | Beta | 340.0s |

**Above Grid data without an image is placeholder**
