---
layout: post
title:  Flux1
author: rkuo
categories: [ Jekyll, tutorial ]
image: assets/images/flux1.jpg?raw=true
featured: true
hidden: false
---
Flux.1 最強文生圖大模型, Comfyui本地安裝 

---
### [本地部署Flux.1 最強文生圖大模型！ Comfyui 一鍵安裝，簡單又方便](https://www.freedidi.com/13266.html)
Flux.1 是一款免費開源的模型,效能可與Midjourney V6媲美。用戶可透過Comfyui調用Flux.1<br>

#### Flux 模型
Flux 模型總共有3個，分別是：Flux Pro、Flux Dev、Flux Schnell，以下是其表現的對照圖:<br>
![](https://www.freedidi.com/wp-content/uploads/2024/08/uisdc-mj-20240805-2-1030x720.webp)

* [pro] 是最頂級的模型，但是只能透過API 呼叫；
* [dev] 是由[pro]提煉，開源但非商用，品質和效果與[pro]類似；
* [schnell] 是經過蒸餾的4 步驟模型，速度比[dev] 快10 倍，Apache 2 開源授權。

---
### Flux.1 安裝

1. 下載最新版[Comfyui](https://github.com/comfyanonymous/ComfyUI)
目前ComfyUI 已支援此模型，更新至最新版即可使用<br>
`git clone https://github.com/comfyanonymous/ComfyUI`<br>

2. 設定中文語言:[點選下載](https://github.com/AIGODLIKE/AIGODLIKE-ComfyUI-Translation)中文語言包，將ZIP包解壓縮到`ComfyUI\custom_nodes`目錄中

3. 下載Flux 模型： FLUX 模型有四個可選，FLUX.1 [dev] 、FLUX.1 [dev] fp8、FLUX.1 [schnell]、FLUX.1 [schnell] fp8
① FLUX.1 [dev] ：官方版本滿配版，最低顯示需求24G；下載位址：[點選下載](https://huggingface.co/black-forest-labs/FLUX.1-dev/tree/main)<br>
② FLUX.1 [dev] fp8：大佬優化[dev] 後版本，建議選擇此版本，最低12G 顯存可跑 [點選下載](https://huggingface.co/Kijai/flux-fp8/blob/main/flux1-dev-fp8.safetensors)<br>
③ FLUX.1 [schnell]：4 步蒸餾模型，多數顯示 卡可跑。[點選下載](https://huggingface.co/black-forest-labs/FLUX.1-schnell/blob/main/flux1-schnell.safetensors)<br>
④ FLUX.1 [schnell] fp8：最佳化版本，適應較低的顯示卡配置。[點選下載](https://huggingface.co/Kijai/flux-fp8/blob/main/flux1-schnell-fp8.safetensors)<br>

4. 下載CLIP 模型： 需下載t5xxl_fp16.safetensors 或t5xxl_fp8_e4m3fn.safetensors 
(建議選擇fp8 版本，如果你顯存超過32G 可選擇fp16 版本）<br>
還有將 clip_l.safetensors 放到ComfyUI/models/clip/ 目錄中： [點擊前往](https://huggingface.co/comfyanonymous/flux_text_encoders/tree/main)<br>

5. 下載VAE模型存放至ComfyUI/models/vae/ 目錄: [點擊下載](https://huggingface.co/black-forest-labs/FLUX.1-schnell/blob/main/ae.safetensors)

---
### Flux1 使用
[美圖產生提示詞](https://www.freedidi.com/13328.html)<br>
**提示詞：**`Two young Japanese women, one wearing a red top and blue jeans, the other wearing a white top and jeans, both holding umbrellas, walking on the streets of Tokyo`<br>
![](https://www.freedidi.com/wp-content/uploads/2024/08/ComfyUI_00007_.webp)

