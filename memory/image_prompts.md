---
name: stable_diffusion_optimized_prompts
description: 针对 SDXL 和 SD 1.5 模型的正向/负向提示词优化标准
type: image_prompts
---

# SDXL & SD 1.5 提示词优化标准 (v1.0)

## 1. SDXL 系列标准 (Illustrious, Pony, RealVisXL)
**逻辑**：注重语义理解与氛围渲染，负向提示词极简。

### 正面通用模板
```text
(masterpiece, best quality, amazing quality:1.2), ultra-detailed, 8k wallpaper, cinematic lighting, dramatic shadows, depth of field, sharp focus, highly detailed texture, (fine skin texture:1.1), (intricate details:1.1), volumetric lighting, global illumination, ray tracing, [主体描述], vibrant colors, dynamic composition, masterpiece aesthetic.
```

### 负面通用模板
```text
lowres, bad anatomy, bad hands, text, error, missing fingers, extra digit, fewer digits, cropped, worst quality, low quality, normal quality, jpeg artifacts, signature, watermark, username, blurry, artist name, (deformed iris, deformed pupils:1.1), (worst quality, low quality:1.2).
```

## 2. SD 1.5 系列标准 (Realistic Vision, MeinaMix)
**逻辑**：标签堆砌式描述，极度依赖负向提示词防止崩坏。

### 正面通用模板
```text
masterpiece, best quality, ultra-detailed, highres, 8k, absurdres, cinematic lighting, (vivid colors:1.1), (detailed background:1.2), [主体标签], soft lighting, sharp focus, (dynamic angle:1.1), (intricate details:1.2), illustration.
```

### 负面通用模板
```text
(worst quality, low quality:1.4), (bad anatomy), (inaccurate limb), bad hands, missing fingers, extra fingers, (mutated hands and fingers:1.5), (mutation, deformed:1.2), (unclear eyes), (intertwined fingers), text, logo, watermark, signature, username, error, (missing arms, missing legs), jpeg artifacts, lowres, blurry, cropped, (gross proportions), (malformed limbs), (extra limbs), (fused fingers), (too many fingers), (long neck).
```

## 3. 编写原则
- **SDXL**: 推荐使用自然语言短句描述空间关系。
- **SD 1.5**: 必须开启 Hires. fix，质量标签置前。
- **权重**: SDXL 控制在 1.4 以下，SD 1.5 可适当提高核心标签权重。
