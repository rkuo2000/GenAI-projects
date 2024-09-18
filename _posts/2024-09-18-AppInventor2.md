---
layout: post
title:  AppInventor2
author: rkuo
categories: [ Jekyll, tutorial ]
image: assets/images/ai2-with-mitai.png?raw=true
featured: true
hidden: true
---

AppInventor2 手機App & 開發環境

---
## App : Gemini_Speak

**使用模型：** Gemini-1.5-Flash <br>

**主要功能：** 呼叫大型語言模型 <br>
**次要功能：** 支援語音輸入和語音輸出<br>

(Google 雙子星為一個多模態大型語言模型, 具備視覺能力）<br>

---
### Enter MIT AppInventor2
use Chrome to open [ai2.appinventor.mit.edu](https://ai2.appinventor.mit.edu/)<br>

![](https://github.com/rkuo2000/GenAI-projects/blob/master/assets/images/ai2_appinventor.png?raw=true)

---
### Import project
* 載入計畫 [Gemini_Speak.aia](https://github.com/rkuo2000/GenAI/blob/main/Gemini_Speak.aia)<br>

![](https://github.com/rkuo2000/GenAI-projects/blob/master/assets/images/ai2_import_project.png?raw=true)
<br>

---
### Project Designer
App版面佈局<br>

![](https://github.com/rkuo2000/GenAI-projects/blob/master/assets/images/ai2_Gemini_Speak.png?raw=true)<br>

---
### Project Blocks 
拼圖式程式設計<br>

![](https://github.com/rkuo2000/GenAI-projects/blob/master/assets/images/ai2_Gemini_Speak_Blocks_starting.png?raw=true)<br>

1. 至 https://aistudio.google.com/app/apikey
2. 產生金鑰 (Create API Key)
3. 複製轉貼至global API_Key變數

---
### Project Build
![](https://github.com/rkuo2000/GenAI-projects/blob/master/assets/images/ai2_Gemini_Speak_build_apk.png?raw=true)<br>

---
### generated APK
![](https://github.com/rkuo2000/GenAI-projects/blob/master/assets/images/ai2_Gemini_Speak_APK_QR.png?raw=true)<br>
Download .apk to install on Android Phone/Tablet

---
### App running
<p><img width="50%" height="50%" src="https://github.com/rkuo2000/GenAI-projects/blob/master/assets/images/ai2_Gemini_Speak_running.jpg?raw=true"></p>

---
## 後續開發

* Chain-of-Thoghts for Reasoning

* Integration with smartphone features, such as Google Maps, Pedometer, IMU, GPS, Camera, ...

---
### Reasoning
```
我在杯子裡放一個草莓
把杯子倒過來放在桌上
再把杯子放到微波爐裡
請問草莓在哪？
```

![](https://github.com/rkuo2000/AI-course/blob/main/images/Reasoning_Gemini_App.jpg?raw=true)

---
### Chain-of-Thought Prompting
**Paper:** [Chain-of-Thought Prompting Elicits Reasoning in Large Language Models](https://arxiv.org/abs/2201.11903)<br>
![](https://ar5iv.labs.arxiv.org/html/2201.11903/assets/x1.png)

---
### [ReAct Prompting](https://react-lm.github.io/)
![](https://react-lm.github.io/files/diagram.png)

---
### [Chain-of-Thought Prompting](https://www.promptingguide.ai/techniques/cot)
![](https://www.promptingguide.ai/_next/image?url=%2F_next%2Fstatic%2Fmedia%2Fcot.1933d9fe.png&w=1080&q=75)

1. **Zero-shot COT Prompting**
![](https://www.promptingguide.ai/_next/image?url=%2F_next%2Fstatic%2Fmedia%2Fzero-cot.79793bee.png&w=1080&q=75)

2. **Automatic Chain-of-Thought (Auto-CoT)**
![](https://www.promptingguide.ai/_next/image?url=%2F_next%2Fstatic%2Fmedia%2Fauto-cot.642d9bad.png&w=1200&q=75)

---
### [Chain of thought and ReAct — SQL Agent](https://abvijaykumar.medium.com/prompt-engineering-chain-of-thought-and-react-sql-agent-85fa42575c06)

