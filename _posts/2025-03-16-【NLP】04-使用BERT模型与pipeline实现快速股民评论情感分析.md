---
title: 【NLP】04-使用BERT模型与pipeline实现快速股民评论情感分析
author: Autumn
date: 2025-03-16 +0800
categories: [NLP, NLP项目]
tags: [NLP, 文本分类]
---

## 项目简介
使用BERT模型的pipeline快速实现股民评论的情感分类。

## 模型
BertForSequenceClassification
- [BertForSequenceClassification(hugging face)](https://huggingface.co/michaelfeil/BertForSequenceClassificationTesting/tree/main)，用于序列分类的BERT模型

## 数据
- 数据从 [https://guba.eastmoney.com/list,601901_1.html](https://guba.eastmoney.com/list,601901_1.html) 爬取
- 本项目的数据并非最新，为2023年12月左右的评论数据

## 项目特点/难点
1. 这个项目是比较简单的，pipeline很好用很方便，但是由于原生BERT没有做SFT，所以分类的效果并不是特别好。


