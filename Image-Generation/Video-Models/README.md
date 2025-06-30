# Video Models

# Wan 2.1

## Text-to-Video (T2V)

### LORA Comparison
Comparing Wan Native (no LORA) with speed-up (turbo) LORAS. Comparing generation time with output quality. Native generation is 20-steps per frame. LORA generation is 4-steps per frame. CFG is always 1.

| 5-second video | 20 Steps (Default) | CausVid | FusionX | lightx2v | lcm_r16 |
|:-:|:-:|:-:|:-:|:-:|:-:|
|  Generation Time | 11.68 min | 2.45 min | 2.40 min | 2.40 min | 2.39 min |
| FPS/Frames| 16/81 | 24/121 | 24/121 | 24/121 | 24/121 |
| Video | <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation\Video-Models\native.webp?raw=true" width="256"> | <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation\Video-Models\causvid.webp?raw=true" width="256"> | <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation\Video-Models\fusionx.webp?raw=true" width="256"> | <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation\Video-Models\lightx2v.webp?raw=true" width="256"> | <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation\Video-Models\lcm_r16.webp?raw=true" width="256"> |

| 5-second video | lightx2v+lcm_r16 | FusionX+CausVid | FusionX+lightx2v | FusionX+lcm_r16 |
|:-:|:-:|:-:|:-:|:-:|
|  Generation Time | 2.45 min | 2.40 min | 2.42 min | 2.42 min |
| FPS/Frames| 24/121 | 24/121 | 24/121 | 24/121 | 24/121 |
| Video | <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation\Video-Models\lightx2v_lcm_r16.webp?raw=true" width="256"> | <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation\Video-Models\FusionX_CausVid.webp?raw=true" width="256"> | <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation\Video-Models\FusionX_lightx2v.webp?raw=true" width="256"> | <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation\Video-Models\FusionX_lcm_r16.webp?raw=true" width="256"> |

### Sampler Comparison
Comparing turbo LORAS while using LCM/Beta vs the default Euler/Simple.

| 5-second video | Euler / Simple | LCM / Beta |
|:-:|:-:|:-:|
| CausVid | <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation\Video-Models\causvid.webp?raw=true" width="256"> | <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation\Video-Models\lcm_causvid.webp?raw=true" width="256"> |
| CausVid + FusionX | <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation\Video-Models\FusionX_CausVid.webp?raw=true" width="256"> | <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation\Video-Models\lcm_causvid_fusionx.webp?raw=true" width="256"> |
| FusionX + LightX2v | <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation\Video-Models\FusionX_lightx2v.webp?raw=true" width="256"> | <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation\Video-Models\lcm_fusionx_lightx.webp?raw=true" width="256"> |
| FusionX + LCM_r16 | <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation\Video-Models\FusionX_lcm_r16.webp?raw=true" width="256"> | <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation\Video-Models\lcm_fusionx_lcm.webp?raw=true" width="256"> |

### Video-Step Comparison
Using turbo LORAs, comparing generation time and output quality depending on video-step parameters. Tested video-steps are 4-steps per frame, 8-steps per frame and 12-steps per frame. All generations are with CFG: 1.
| 5-second video | 4-Steps per frame | 8-Steps per frame | 12-Steps per frame |
|:-:|:-:|:-:|:-:|
| CauseVid | 2.45 min | 4.33 min | 6.42 min |
| FusionX + CauseVid | 2.40 min | 4.54 min | 6.52 min |
| FusionX + LightX2v | 2.42 min | 4.51 min | 6.48 min |
| FusionX + LCM_r16 | 2.42 min | 4.45 min | 6.46 min |

## Image-to-Video (I2V)