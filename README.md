# 🌍 Solar Data Analysis – West Africa (MoonLight Energy Solutions)

This repository contains exploratory and performance analysis of solar PV data from three West African locations:

- 🇧🇯 **Benin**
- 🇸🇱 **Sierra Leone – Bumbuna**
- 🇹🇬 **Togo – Dapaong_QC**

Each notebook contains:
- Data cleaning and non-null summary
- GHI, DNI, and DHI time series analysis
- Panel performance before and after cleaning (ModA, ModB)
- Correlation heatmaps
- Scatter plots between irradiance and module temperature

---

## Country Summaries

### 🇧🇯 Benin
- Partial data, with moderate gaps
- Significant impact from cleaning on ModA and ModB
- Strong correlations between GHI and panel output
- Moderate seasonal variability

### 🇸🇱 Sierra Leone – Bumbuna
- Clean ~12-month dataset with low noise
- Very strong correlation between irradiance and module temperatures
- Cleaning produced >100% gain in output
- Low-to-moderate climate volatility

### 🇹🇬 Togo – Dapaong_QC
- Full, high-quality dataset (525,600 rows)
- Strong and consistent correlations (GHI ~0.90+)
- Cleaning effect doubled module output
- Stable seasonal trends and ideal for modeling

---

## 📊 Comparison Highlights

| Country     | Data Quality | Cleaning Effect | Correlation Strength | Best for Modeling |
|-------------|--------------|-----------------|----------------------|-------------------|
| Benin       | Moderate     | ✅✅             | ✅✅                  | Somewhat          |
| Sierra Leone| Good         | ✅✅✅           | ✅✅✅                | Strong            |
| Togo        | Excellent    | ✅✅✅           | ✅✅✅                | ✅✅✅             |

---

## 📁 Structure

```plaintext
📂 data/
    benin/
    sierraleone-bumbuna/
    togo-dapaong_qc/

📂 notebooks/
    benin-analysis.ipynb
    sierraleone-bumbuna-analysis.ipynb
    togo-dapaong_qc-analysis.ipynb

📂 images/
    cleaned_plots/
    scatter_plots/
    correlation_maps/
