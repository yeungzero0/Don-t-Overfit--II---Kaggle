# Don't Overfit! II - Kaggle Competition  
**Avoiding Overfitting in High-Dimensional Small Dataset**

[![Python](https://img.shields.io/badge/Python-3.11-blue)](https://www.python.org/)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-1.x-orange)](https://scikit-learn.org/)
[![XGBoost](https://img.shields.io/badge/XGBoost-2.x-green)](https://xgboost.ai/)
[![Kaggle](https://img.shields.io/badge/Kaggle-Competition-red)](https://www.kaggle.com/competitions/dont-overfit-ii)

這是 **POLYU CS 學生** 的學習練習，參加 Kaggle 「Don’t Overfit! II」  
目標是在只有 **250 筆訓練資料、300 個特徵** 的高維小資料集上，建構不會過擬合（Overfitting）的模型，最終以 **AUC-ROC** 作為評分標準。

---

## ⚠️ 免責聲明 (Disclaimer)

**本專案純粹用於學習與課程用途**。

- 此專案是 **POLYU CS 學生** 的學習練習，主要目的是理解與對抗 Overfitting 問題。
- **嚴禁商業使用**：本專案**不得**用於任何商業活動、產品開發或生產環境。
- **僅供參考與教育**：所有產出的 submission 檔案與結果僅供個人學習與測試之用。
- **無任何保證**：作者不對使用本專案所產生的任何輸出、Kaggle 分數或後果承擔任何責任。

> **總之：這只是我在 POLYU 學習如何避免 Overfitting 的練習專案，不是專業解決方案。**

---

## 專案特色

- 使用 **Older Dataset for Don’t Overfit II Challenge**（250 筆訓練資料 + 19,750 筆測試資料）
- 探索三種經典模型：
  - Logistic Regression（含特徵過濾、正則化參數 C 調優）
  - Random Forest（調整 max_depth 控制樹深度）
  - **XGBoost**（Gradient Boosting，最佳模型）
- 針對小資料集設計多種防過擬合策略：
  - VarianceThreshold 特徵過濾
  - 標準化（StandardScaler）
  - 強正則化（低 C 值、低 max_depth）
  - 基於 AUC-ROC 進行超參數調優
- 最終 Private Score：**0.766**（XGBoost）

![image](https://github.com/yeungzero0/Don-t-Overfit--II---Kaggle/blob/main/Overfit2025_Timg.png)

---
