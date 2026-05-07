# Swap — AI-Powered Second-Hand Goods Exchange Platform

A mobile platform that combines AI object recognition with a 
card-based exchange interface, making secondhand trading faster, 
safer, and more engaging for university students.

National Chengchi University · MIS Department · 2023 Project Presentation · Team 8A

## Overview

Swap simplifies the secondhand listing process using AI — users 
upload a photo and the platform automatically fills in item name, 
category, color, and brand, eliminating manual input entirely.

## Features

- **Auto-tagging** — YOLO object detection identifies item category 
  and name from photos
- **Color recognition** — K-Means clustering detects item color 
  automatically
- **Brand detection** — AILOGO recognition identifies brand from images
- **Student account verification** — reduces fake accounts and fraud
- **English interface** — designed to be accessible to international students
- **Card-based UI** — swipe-style design built for Gen Z users

## Tech Stack

| Layer | Technology |
|---|---|
| Frontend | Flutter |
| Backend | Python |
| Image Recognition | YOLO, K-Means, AILOGO |
| Database | Supports unstructured data |

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
