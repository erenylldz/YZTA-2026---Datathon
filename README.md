# YZTA-2026---Datathon
YZTA 2026 Datathon
Sleep & Cognitive Performance Analysis
Project Overview

This project investigates the relationship between sleep behavior, lifestyle habits, physiological conditions, psychological characteristics, and cognitive performance levels using a synthetic tabular dataset.

The dataset includes:

demographic variables,
sleep-related measurements,
behavioral indicators,
physiological variables,
psychological variables.
Target Variable

bilissel_performans_skoru

Continuous numerical variable
Range: 0–10
Higher values indicate better cognitive performance
Dataset Structure
Dataset	Rows	Columns
Train	56,000	24
Test	24,000	23
Notes
The training dataset contains the target variable.
The test dataset does not include target information.
Each row represents one individual observation.
Variable Categories
Demographic Variables

Examples:

yas
cinsiyet
ulke
meslek
Sleep-Related Variables

Examples:

rem_yuzdesi
derin_uyku_yuzdesi
uykuya_dalma_suresi_dk
gecelik_uyanma_sayisi
hafta_sonu_uyku_farki_saat
kronotip

These variables describe:

sleep efficiency,
sleep continuity,
circadian rhythm tendencies,
sleep fragmentation.
Lifestyle Variables

Examples:

uyku_oncesi_ekran_suresi_dk
uyku_oncesi_kafein_mg
gunluk_calisma_saati
gunluk_adim_sayisi
gun_tipi

These variables capture:

caffeine consumption,
screen exposure,
work intensity,
physical activity,
weekday/weekend differences.
Exploratory Data Analysis (EDA)

The exploratory analysis included:

dataset structure examination,
descriptive statistical analysis,
missing value analysis,
outlier diagnostics,
distribution analysis,
correlation analysis,
train-test consistency checks.
Missing Value Analysis

Variables containing missing observations:

Variable	Approximate Missing Rate
kronotip	~3.5%
vucut_kitle_indeksi	~3.1%
stres_skoru	~3.1%
uyku_oncesi_kafein_mg	~2.6%
meslek	~2.5%
ruh_sagligi_durumu	~2.0%
Analysis Steps
Feature-level missingness examination
Row-level missing count analysis
Missing value co-occurrence analysis
Train-test missing pattern comparison
Distribution Analysis

The following visualization techniques were used:

Histograms
KDE plots
Boxplots

Variables such as:

uyku_oncesi_kafein_mg
uyku_oncesi_ekran_suresi_dk
sekerleme_suresi_dk

showed positively skewed distributions and long upper tails.

Outlier Diagnostics

Outlier analysis was performed using:

IQR-based diagnostics,
boxplots,
distribution visualizations.
Variable	Approximate IQR Outlier Rate
uyku_oncesi_kafein_mg	~6.2%
uyku_oncesi_ekran_suresi_dk	~5.9%
stres_skoru	~1.8%
uykuya_dalma_suresi_dk	~1.0%
Correlation Analysis

Pearson correlation analysis was conducted between numerical variables and the target variable.

Variable	Correlation with Target
stres_skoru	-0.59
rem_yuzdesi	0.44
gunluk_calisma_saati	-0.34
derin_uyku_yuzdesi	0.28
gecelik_uyanma_sayisi	-0.27
Statistical Characteristics

The dataset contains:

numerical and categorical variables,
moderate missingness,
skewed behavioral variables,
bounded target distribution,
moderate outlier presence,
potential interaction effects between sleep and lifestyle variables.
General Conclusion

The dataset provides a statistically rich structure for analyzing the relationship between:

sleep quality,
behavioral habits,
physiological condition,
psychological state,
cognitive performance outcomes.
