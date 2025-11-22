# Pansharpening-WorldView3
"Deep learning-based pansharpening of WorldView-3 satellite imagery using CBAMParallelUNet and EnhancedCBAMTransformerUNet"

## Project Overview
- **Dataset:** WorldView-3 satellite imagery
- **Models:** CBAMParallelUNet, EnhancedCBAMTransformerUNet
- **Key Results:** 34.34 dB PSNR (9.04 dB over baseline)

## Models

### CBAMParallelUNet
- Dual parallel encoders (PAN + MS)
- CBAM attention modules
- Parameters: 2.01M

### EnhancedCBAMTransformerUNet
- Transformer bottleneck with multi-head attention
- CNN encoder/decoder with skip connections
- Parameters: 2.14M
- **Best Performance:** 34.34 dB PSNR, 0.925 SSIM, 0.164 SAM

## Metrics
| Model | PSNR (dB) | SSIM | SAM (rad) |
|-------|-----------|------|-----------|
| CBAMParallel | 27.54 | 0.736 | 0.330 |
| **Transformer** | **34.34** | **0.925** | **0.164** |
| Baseline (Bilinear) | 25.28 | 0.620 | - |

## Requirements

