# YZTA-2026---Datathon

# 🧠 YZTA 2026 Datathon  
## Sleep & Cognitive Performance Analysis

---

## 📌 Project Overview

This project investigates the relationship between:

- sleep behavior,
- lifestyle habits,
- physiological characteristics,
- psychological conditions,
- cognitive performance levels

using a synthetic tabular dataset.

The dataset contains individual-level observations including demographic information, sleep-related measurements, behavioral variables, and health indicators.

### 🎯 Target Variable

`bilissel_performans_skoru`

| Property | Description |
|---|---|
| Variable Type | Continuous Numerical |
| Range | 0 – 10 |
| Meaning | Cognitive performance score |

---

# 📂 Dataset Structure

| Dataset | Rows | Columns |
|---|---:|---:|
| Train | 56,000 | 24 |
| Test | 24,000 | 23 |

### Notes
- The training dataset contains the target variable.
- The test dataset does not contain target information.
- Each observation represents one individual participant.

---

# 🧩 Variable Categories

## 👤 Demographic Variables

Examples:

- `yas`
- `cinsiyet`
- `ulke`
- `meslek`

These variables describe general participant characteristics.

---

## 😴 Sleep-Related Variables

Examples:

- `rem_yuzdesi`
- `derin_uyku_yuzdesi`
- `uykuya_dalma_suresi_dk`
- `gecelik_uyanma_sayisi`
- `hafta_sonu_uyku_farki_saat`
- `kronotip`

These variables provide information regarding:

- sleep efficiency,
- sleep fragmentation,
- sleep continuity,
- circadian rhythm patterns.

---

## 🏃 Lifestyle Variables

Examples:

- `uyku_oncesi_ekran_suresi_dk`
- `uyku_oncesi_kafein_mg`
- `gunluk_calisma_saati`
- `gunluk_adim_sayisi`
- `gun_tipi`

These variables capture:

- screen exposure,
- caffeine consumption,
- work intensity,
- physical activity,
- weekday/weekend behavioral differences.

---

## ❤️ Physiological & Psychological Variables

Examples:

- `stres_skoru`
- `ruh_sagligi_durumu`
- `dinlenik_nabiz_bpm`
- `vucut_kitle_indeksi`

These variables may reflect:

- stress level,
- cardiovascular condition,
- body composition,
- psychological well-being.

---

# 📊 Exploratory Data Analysis (EDA)

The exploratory analysis process included:

- dataset structure examination,
- descriptive statistical analysis,
- missing value analysis,
- outlier diagnostics,
- numerical distribution analysis,
- categorical variable analysis,
- correlation analysis,
- train-test consistency checks.

---

# 📈 Descriptive Statistical Analysis

The following statistical summaries were computed for numerical variables:

- mean,
- median,
- standard deviation,
- quartiles,
- minimum & maximum values.

Several behavioral variables exhibited positively skewed distributions, especially:

| Variable |
|---|
| `uyku_oncesi_kafein_mg` |
| `uyku_oncesi_ekran_suresi_dk` |
| `sekerleme_suresi_dk` |

The target variable displayed:
- bounded distribution,
- moderate variability,
- approximately continuous structure.

---

# ❗ Missing Value Analysis

Variables containing missing observations:

| Variable | Approximate Missing Rate |
|---|---:|
| `kronotip` | ~3.5% |
| `vucut_kitle_indeksi` | ~3.1% |
| `stres_skoru` | ~3.1% |
| `uyku_oncesi_kafein_mg` | ~2.6% |
| `meslek` | ~2.5% |
| `ruh_sagligi_durumu` | ~2.0% |

### Missing Value Investigation

The analysis included:

- feature-level missingness,
- row-level missing counts,
- missing value co-occurrence patterns,
- train-test missingness comparison.

Because missingness remained relatively low, row or column deletion strategies were avoided to minimize information loss.

---

# 📦 Outlier Diagnostics

Outlier analysis was performed using:

- IQR-based diagnostics,
- boxplots,
- distribution visualizations.

## Variables with Higher Outlier Ratios

| Variable | Approximate IQR Outlier Rate |
|---|---:|
| `uyku_oncesi_kafein_mg` | ~6.2% |
| `uyku_oncesi_ekran_suresi_dk` | ~5.9% |
| `stres_skoru` | ~1.8% |
| `uykuya_dalma_suresi_dk` | ~1.0% |

The analysis showed that several behavioral variables contained long upper-tail distributions.

---

# 🔗 Correlation Analysis

Pearson correlation analysis was conducted between numerical variables and the target variable.

## Variables Showing Stronger Relationships with Cognitive Performance

| Variable | Correlation |
|---|---:|
| `stres_skoru` | -0.59 |
| `rem_yuzdesi` | 0.44 |
| `gunluk_calisma_saati` | -0.34 |
| `derin_uyku_yuzdesi` | 0.28 |
| `gecelik_uyanma_sayisi` | -0.27 |

### Observations

Negative associations:
- stress level,
- sleep fragmentation,
- long work duration.

Positive associations:
- REM sleep percentage,
- deep sleep percentage.

---

# 🔍 Train-Test Consistency Analysis

Train and test datasets were compared using:

- KDE distribution comparisons,
- categorical level checks,
- missing value pattern comparisons.

The analysis indicated:
- structurally similar numerical distributions,
- no severe distribution shift,
- consistent categorical levels across datasets.

---

# 🧪 Statistical Characteristics of the Dataset

The dataset exhibits:

- mixed numerical and categorical structure,
- moderate missingness,
- skewed behavioral variables,
- bounded continuous target distribution,
- moderate outlier presence,
- potential interaction effects between sleep and lifestyle variables.

---

# ✅ General Conclusion

The exploratory analysis demonstrated that the dataset contains meaningful variability across:

- sleep behavior,
- lifestyle habits,
- physiological characteristics,
- psychological indicators,
- cognitive performance levels.

Overall, the dataset provides a statistically rich framework for investigating the relationship between sleep quality, behavioral patterns, and cognitive performance outcomes.
