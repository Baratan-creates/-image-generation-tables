# Kontext

## Quant Comparison
### fp8 vs gguf_q4_km
In this comparison we will compare image quality and generation time. We will start with an image generated with Flux.Dev and use Kontext to convert it to pixel-art.

____Original____

<img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation\Kontext\original.png?raw=true" width="256">

| | 20 Steps | 24 Steps | 28 Steps |
|:-:|:-:|:-:|:-:|
| fp8 Generation Time | 96.13 sec | 107.94 sec | 2.08 min |
| fp8 image | <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation\Kontext\fp820.png?raw=true" width="256"> | <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation\Kontext\fp824.png?raw=true" width="256"> | <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation\Kontext\fp828.png?raw=true" width="256"> |
| gguf_q4_km Generation Time | 102.70 sec | 100.22 sec| 118.02 sec | 
| gguf_q4_km Image | <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation\Kontext\q420.png?raw=true" width="256"> | <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation\Kontext\q424.png?raw=true" width="256"> | <img src="https://github.com/Baratan-creates/-image-generation-tables/blob/main/Image-Generation\Kontext\q428.png?raw=true" width="256"> |

