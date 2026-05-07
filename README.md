# Swap — AI-Powered Second-Hand Goods Exchange Platform

A Flutter mobile app with a Python backend that automates secondhand 
item listings using computer vision — users upload one photo and the 
platform fills in name, category, color, and brand automatically.

National Chengchi University · MIS Department · 2023 · Team 8A

## Problem

Existing secondhand platforms require manual input for every listing, 
have poor UX, and lack trust mechanisms — discouraging casual users 
from participating.

## Solution

Swap reduces listing friction to a single photo upload by chaining 
three AI models in sequence:

1. **YOLO v5 object detection** — localizes and classifies the item, 
   extracting category and product name
2. **K-Means color clustering** — samples dominant pixel clusters 
   from the detected region to identify item color
3. **AILOGO recognition** — matches brand logos against a trained 
   classifier to fill in brand name

All three outputs auto-populate the listing form before the user 
sees it.

## Tech Stack

| Layer | Technology |
|---|---|
| Mobile Frontend | Flutter (Dart) |
| Backend API | Python |
| Object Detection | YOLOv3 |
| Color Extraction | K-Means clustering (OpenCV) |
| Brand Recognition | AILOGO classifier |
| Auth | University student account verification |
| Database | NoSQL (unstructured data support) |

## Key Design Decisions

- **Student-only auth** — verified school accounts reduce fake 
  listings and fraud without complex KYC
- **English-first UI** — targets international students on campus 
  who are underserved by Chinese-language platforms
- **Card swipe interface** — reduces cognitive load vs. 
  traditional list-based secondhand apps

## Team & Responsibilities

| Member | Role |
|---|---|
| Huang Yun-Chien (Athena) | Machine Learning , Product Manager |
| Yang Juan-Tzu | App Frontend & Backend, Database |
| Huang Hui-Ju | App Frontend & Backend |
| Hua Chiao-Chen | Image Recognition, Database |
| Huang Jen-Chien | App Frontend & Backend |

## Motivation

Existing secondhand platforms (Facebook groups, Carousell) suffer 
from poor UX, lengthy listing processes, and security concerns. 
Swap addresses all three while promoting sustainable consumption 
aligned with UN SDG 12.5.

---

## 中文簡介

Swap 是一個結合 AI 圖像辨識技術的二手物品交換平台，專為大學生設計。
使用者上傳商品照片後，系統會自動辨識品項名稱、顏色與品牌，免除手動填寫。
前端使用 Flutter 開發，後端結合 YOLO 物件偵測、K-Means 色彩分群與 AILOGO 品牌辨識。
