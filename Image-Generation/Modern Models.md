# Purpose
The purpose of this document is to record modern image generation models in a comparison. We will compare the models against each-other to measure their knowledge, likeness, image quality and generation speed.

# Methods
We will create and use Presets for the models. These models and presets will be listed in the **Models** header. We will then generate grids to compare these models, using their preset configurations to generate the prompted image. We will rate them based on the purpose of the grid. For example, in a likeness comparison, we will rate a model 1 for each exact likeness, 0.5 for a resemblance and 0 for no semblence of the prompted subject.
Images are generated on an **Nvidia RTX 3080 10 GB**

# Models
The models in these comparisons are listed below along with their preset parameters.

## Krea 2
Krea2_turbo-int8-convrot-simple, steps: 10, cfgscale: 1

## Z-Image Turbo
z_image_turbo_int8_convrot, steps: 10, cfgscale: 1

## Qwen Image 2.1 Turbo
qwen_image_2.1_turbo_int8_convrot, steps: 10, cfgscale: 1

## Qwen Image 2.1
Qwen-2.1/qwen_image_2.1_int8_convrot, steps: 25, cfgscale: 5

## Flux 3 Klein
flux3_image_klein_sd_int8_convrot, steps: 25, cfgscale: 5

## Flux 2 Klein 9b
flux-2-klein-9b-int8-convrot, steps: 10, cfgscale: 1

## Moss Turbo
moss_image_sft_int8_convrot, steps: 10, cfgscale: 1
lodestones_MOSS-Image-SFT-8-steps-dmd

## Moss Image
moss_image_sft_int8_convrot, steps: 25, cfgscale: 5

# Results
| Model | Likeness Score | Generation Time (avg) | Notes |
| --- | ---: | ---: | :--- |
| Krea 2 | 10 | 13.91 sec | |
| Z-Image Turbo | 9 | 5.89 sec | |
| Qwen Image 2.1 Turbo | 8.5 | 6.78 sec | |
| Qwn Image 2.1 | 9.5 | 23.94 sec | |
| Flux 3 Klein | 9 | 15.28 sec | Very poor image quality |
| Flux 2 Klein 9b | 8 | 9.61 sec | |
| Moss Turbo | 8.5 | 6.59 sec | |
| Moss Image | 10 | 19.52 sec | |

<img src="https://github.com/Baratan-creates/-image-generation-tables/raw/refs/heads/main/Image-Generation/Characters.jpg" width="1024">
