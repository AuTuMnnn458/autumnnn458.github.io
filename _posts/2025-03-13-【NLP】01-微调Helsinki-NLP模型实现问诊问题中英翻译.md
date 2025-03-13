---
title: 【NLP】01-微调Helsinki-NLP模型实现问诊问题中英翻译
author: Autumn
date: 2025-03-13 +0800
categories: [NLP]
tags: [NLP, 机器翻译, 微调]
---

## 项目简介
使用Helsinki-NLP模型对数据tico-19进行微调。
- 项目地址： https://github.com/AuTuMnnn458/NLP_project/tree/main/nlp01

### 模型
Helsinki-NLP--opus-mt-zh-en 
- 地址：[Helsinki-NLP--opus-mt-zh-en(hugging face)](https://huggingface.co/Helsinki-NLP/opus-mt-zh-en)
- 简介：一个比较适合做中英翻译的模型，框架跟transformer基本一致，系数给得比较小，轻量化。
### 数据
tico19
- 地址：[tico19-en-zh(hugging face)](https://huggingface.co/datasets/gmnlp/tico19/viewer/en-zh)
- 简介：Covid19期间收集的疫情相关的翻译句子对。除了中英对应的翻译对以外，tico19里还包含非常多其他语言。

## 项目特点/难点
1. 对于`AutoModelForSeq2SeqLM`我使用的比较少，发现它跟`AutoModelForCasualLM`的参数名字差别还是比较大的。
2. 该项目中用的库都是跟`seq2seq`相关的，例如预训练模型`AutoModelForSeq2SeqLM`，参数设置`Seq2SeqTrainingArguments`，数据收集器`DataCollatorForSeq2Seq`， Trainer用的也是`Seq2SeqTrainer`。
3. 训练时间还可以，使用GTX4060，epoch=10跑了14分钟，总步数为3070步。训练出来的模型效果比想象中要好，除了数据集中的原问题可以正确回答，一些比较相关的句子也是可以正常翻译的。我自己做了一个例子：`我觉得我的肺部很痛，无法入睡。`翻译为`i feel a pain in my lungs and can't sleep.`。





