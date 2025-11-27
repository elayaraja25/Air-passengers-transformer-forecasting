# 🚀 Transformer Time Series Forecasting (AirPassengers Dataset)

This project implements a **Transformer-based deep learning model** for **time series forecasting** using the classic **AirPassengers** dataset.  
It includes a complete workflow from **data preprocessing → model training → attention visualization → prediction output generation**.  
The entire project is designed to run smoothly inside **Google Colab**.

---

## 📦 Key Features

### ✅ Transformer Encoder Model  
- Self-attention mechanism  
- Positional encoding  
- Multi-head attention  
- Suitable for univariate & multivariate forecasting  

### ✅ Time Series Dataloader  
- Automatic sequence window generation  
- Uses:  
  - **12 months** history  
  - Predict **6 months** ahead  

### ✅ Attention Visualization  
- Extracts attention weights from every encoder layer  
- Saves a heatmap as `attention_map.jpg`  
- Also stores top-weighted indices in `attention_top_indices.txt`

### ✅ Output Files  
After training, the following files are generated:

| File | Description |
|------|-------------|
| `model_best.pth` | Best saved Transformer model |
| `predictions.txt` | Forecasted values |
| `attention_map.jpg` | Attention heatmap |
| `attention_top_indices.txt` | Top attention values |

---

## 📊 Dataset — AirPassengers

This project uses the classic aviation dataset:

| Column Name | Meaning |
|-------------|---------|
| `Month` | Monthly date (YYYY-MM) |
| `#Passengers` | Number of air passengers |

Make sure your dataset is uploaded inside Colab as:

