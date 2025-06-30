# Kontext

# Quant Comparison
## fp8 vs gguf_q4_km
In this comparison we will compare image quality and generation time. We will start with an image generated with Flux.Dev and use Kontext to convert it to pixel-art.

____Original____

<img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation\Kontext\original.png?raw=true" width="256">

## Step Comparison

| @3.5 Flux Guidance | 20 Steps (Default) | 24 Steps | 28 Steps |
|:-:|:-:|:-:|:-:|
| fp8 Generation Time | 96.13 sec | 107.94 sec | 2.08 min |
| fp8 image | <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation\Kontext\fp820.png?raw=true" width="256"> | <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation\Kontext\fp824.png?raw=true" width="256"> | <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation\Kontext\fp828.png?raw=true" width="256"> |
| gguf_q4_km Generation Time | 102.70 sec | 100.22 sec| 118.02 sec | 
| gguf_q4_km Image | <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation\Kontext\q420.png?raw=true" width="256"> | <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation\Kontext\q424.png?raw=true" width="256"> | <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation\Kontext\q428.png?raw=true" width="256"> |

## Flux Guidance Comparison

| @24 Steps | 1.5 Flux Guidance | 2.5 Flux Guidance | 3.5 Flux Guidance (Default) |
|:-:|:-:|:-:|:-:|
| fp8 Generation Time | 107.81 sec | 105.09 sec | 116.45 sec |
| fp8 image | <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation\Kontext\fp815fg.png?raw=true" width="256"> | <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation\Kontext\fp825fg.png?raw=true" width="256"> | <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation\Kontext\fp835fg.png?raw=true" width="256"> |
| gguf_q4_km Generation Time | 116.58 sec | 96.50 sec| 98.69 sec | 
| gguf_q4_km Image | <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation\Kontext\q415fg.png?raw=true" width="256"> | <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation\Kontext\q425fg.png?raw=true" width="256"> | <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation\Kontext\q435fg.png?raw=true" width="256"> |
| gguf_q4_km Image | <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation\Kontext\15fg.png?raw=true" width="256"> | <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation\Kontext\25fg.png?raw=true" width="256"> | <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation\Kontext\35fg.png?raw=true" width="256"> |

## Sampler Comparison

| Euler / Simple | LCM / Beta |
|:-:|:-:|
| <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation\Kontext\euler_simple.png?raw=true" width="256"> | <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation\Kontext\lcm_beta.png?raw=true" width="256"> |
| <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation\Kontext\euler_simple2.png?raw=true" width="256"> | <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation\Kontext\lcm_beta2.png?raw=true" width="256"> |
| <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation\Kontext\euler_simple3.png?raw=true" width="256"> | <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation\Kontext\lcm_beta3.png?raw=true" width="256"> |
| <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation\Kontext\euler_simple4.png?raw=true" width="256"> | <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation\Kontext\lcm_beta4.png?raw=true" width="256"> |
| <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation\Kontext\euler_simple5.png?raw=true" width="256"> | <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation\Kontext\lcm_beta5.png?raw=true" width="256"> |


# Conclusion
The differences between the gguf quant and the default fp8 is minimal in both generation time and resultant image. Furthermore, the difference between steps and Flux Guidance Scale are more pronounced with too low guidance scale producing a lower quality image.