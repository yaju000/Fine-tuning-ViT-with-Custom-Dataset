# VIT Smoke Classification

本專案使用 Vision Transformer (ViT) 進行煙霧影像分類，支援二分類：「no smoke」與「smoke」。

## 目錄結構

```
fficss_project/
└── VIT/
    ├── trainer.py
    ├── requirements.txt
    └── data/
        ├── train/
        │   ├── no_smoke/
        │   └── smoke/
        └── test/
            ├── no_smoke/
            └── smoke/
```

## 安裝需求

請先安裝以下套件：

```bash
pip install torch torchvision transformers datasets scikit-learn matplotlib Pillow
```

## 資料準備

- 請將訓練資料放在 `data/train/no_smoke` 和 `data/train/smoke` 目錄下。
- 測試資料放在 `data/test/no_smoke` 和 `data/test/smoke` 目錄下。

## 執行訓練

```bash
python trainer.py
```

- 預設會訓練 20 個 epoch，並將模型輸出存至 `vit-smoke-output` 目錄。
- 訓練結束後會自動在測試集上預測並繪製混淆矩陣。

## 主要功能

- 使用 ViT 進行影像二分類。
- 支援自訂資料集路徑。
- 訓練結束後自動評估並繪製混淆矩陣。# Fine-tuning-ViT-with-Custom-Dataset
Fine-tuning a ViT model on a custom dataset, which is a smoke dataset
