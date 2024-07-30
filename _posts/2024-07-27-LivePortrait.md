---
layout: post
title:  LivePortrait
author: rkuo
categories: [ Jekyll, tutorial ]
image: assets/images/liveportrait_showcase.gif?raw=true
featured: true
hidden: true
---
LivePotrait

### [LivePortrait](https://liveportrait.github.io/)
![](https://github.com/KwaiVGI/LivePortrait/blob/main/assets/docs/showcase2.gif?raw=true)

Pipeline of the first stage: base model training.<br>
![](https://liveportrait.github.io/src/img/pipeline_first_stage.jpg)
Pipeline of the second stage: stitching and retargeting modules training.<br>
![](https://liveportrait.github.io/src/img/pipeline_second_stage.jpg)


---
### [https://github.com/KwaiVGI/LivePortrait](https://github.com/KwaiVGI/LivePortrait)
1. Install
`sudo apt install ffmpeg`<br>

```
git clone https://github.com/KwaiVGI/LivePortrait
cd LivePortrait

# create env using conda
conda create -n LivePortrait 
conda activate LivePortrait

# install dependencies
pip install -r requirements.txt
```

2. Download pretrained weights
```
# first, ensure git-lfs is installed, see: https://docs.github.com/en/repositories/working-with-files/managing-large-files/installing-git-large-file-storage
git lfs install
# clone and move the weights
git clone https://huggingface.co/KwaiVGI/LivePortrait temp_pretrained_weights
mv temp_pretrained_weights/* pretrained_weights/
rm -rf temp_pretrained_weights
```

3. Inference
* source input is an image
```
python inference.py -s assets/examples/source/s9.jpg -d assets/examples/driving/d0.mp4
```

* source input is a video
```
python inference.py -s assets/examples/source/s13.mp4 -d assets/examples/driving/d0.mp4
```

---
### WebUI
`python app.py`<br>
![](https://github.com/rkuo2000/GenAI-projects/blob/master/assets/images/liveportrait_app.png?raw=true)

**http://127.0.0.1:8990**<br>
![](https://github.com/rkuo2000/GenAI-projects/blob/master/assets/images/liveportrait_app_webui.png?raw=true)

---
### Demo 影片
<iframe width="315" height="560" src="https://www.youtube.com/embed/HYllSDxbKkI" title="LivePortrait s7--d20" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

<iframe width="315" height="560" src="https://www.youtube.com/embed/sVAxE-0tIpI" title="Hedra 深夜情歌" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

<iframe width="698" height="393" src="https://www.youtube.com/embed/wBO0VsiWC2s" title="LivePortrait ~ Kai Trump" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

