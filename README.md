# YZTA-2026---Datathon
Sleep & Cognitive Performance Dataset Analysis
Project Overview

This project focuses on the exploratory analysis of a synthetic tabular dataset designed to investigate the relationship between sleep behavior, lifestyle habits, physiological characteristics, psychological conditions, and cognitive performance levels.

The dataset contains individual-level observations including demographic information, sleep-related measurements, behavioral variables, and health indicators. The primary objective is to examine how different sleep and lifestyle factors may be associated with cognitive performance outcomes.

The target variable of the dataset is:

bilissel_performans_skoru

which represents a continuous cognitive performance score ranging from 0 to 10.

Dataset Structure
Dataset	Rows	Columns
Train	56,000	24
Test	24,000	23
The training dataset contains the target variable.
The test dataset does not contain target information.
Each observation represents one individual participant.
Variable Categories
Demographic Variables

Variables describing participant characteristics:

yas
cinsiyet
ulke
meslek
Sleep-Related Variables

Variables associated with sleep quality and sleep behavior:

rem_yuzdesi
derin_uyku_yuzdesi
uykuya_dalma_suresi_dk
gecelik_uyanma_sayisi
hafta_sonu_uyku_farki_saat
kronotip

These variables describe:

sleep efficiency,
sleep continuity,
sleep fragmentation,
circadian rhythm patterns.
Lifestyle Variables

Variables representing daily behavioral habits:

uyku_oncesi_ekran_suresi_dk
uyku_oncesi_kafein_mg
gunluk_calisma_saati
gunluk_adim_sayisi
gun_tipi

These features provide information regarding:

screen exposure,
caffeine consumption,
work intensity,
physical activity,
weekday/weekend differences.
Physiological and Psychological Variables

Variables describing physical and mental condition:

stres_skoru
ruh_sagligi_durumu
dinlenik_nabiz_bpm
vucut_kitle_indeksi

These variables may reflect:

stress level,
cardiovascular condition,
body composition,
psychological well-being.
Exploratory Data Analysis (EDA)

A comprehensive exploratory data analysis (EDA) process was conducted before preprocessing and modeling stages in order to better understand the statistical and structural properties of the dataset.

The EDA workflow included:

dataset shape examination,
variable type analysis,
descriptive statistics,
duplicate observation checks,
missing value analysis,
numerical distribution analysis,
categorical frequency analysis,
outlier diagnostics,
target variable analysis,
correlation analysis,
train-test consistency analysis.
Data Structure Examination

Initial analysis focused on understanding the overall structure of the dataset.

The following controls were performed:

dataset dimensions,
variable data types,
numerical/categorical feature separation,
duplicate row checks,
train-test feature consistency checks.

The dataset contains a mixture of:

continuous numerical variables,
categorical variables,
binary-type indicators.

No duplicated observations were detected in the training dataset.

Descriptive Statistical Analysis

Descriptive statistics were computed for all numerical variables.

The analysis included:

mean,
median,
standard deviation,
quartiles,
minimum and maximum values.

Several behavioral variables displayed positively skewed distributions, particularly:

uyku_oncesi_kafein_mg
uyku_oncesi_ekran_suresi_dk
sekerleme_suresi_dk

The target variable (bilissel_performans_skoru) showed:

bounded distribution between 0 and 10,
moderate variability,
approximately continuous structure.
Missing Value Analysis

Missing value analysis identified incomplete observations in several variables.

Variable	Approximate Missing Rate
kronotip	~3.5%
vucut_kitle_indeksi	~3.1%
stres_skoru	~3.1%
uyku_oncesi_kafein_mg	~2.6%
meslek	~2.5%
ruh_sagligi_durumu	~2.0%

The analysis included:

feature-level missingness,
row-level missing counts,
missing value co-occurrence patterns,
train-test missing value comparisons.

The overall missingness level remained relatively low. Therefore, row or column deletion strategies were not preferred in order to minimize information loss.

Numerical Distribution Analysis

Distribution analysis was conducted using:

histograms,
kernel density estimation (KDE),
boxplots.

Several variables demonstrated:

non-normal distributions,
positive skewness,
long upper tails.

Behavioral variables related to lifestyle habits showed higher variance compared to demographic variables.

The target variable distribution was also examined to evaluate:

central tendency,
variability,
potential imbalance,
extreme target regions.
Outlier Diagnostics

Potential outlier observations were investigated using:

boxplot visualizations,
IQR-based outlier analysis,
distributional inspection.

Variables with relatively higher outlier ratios included:

Variable	Approximate IQR Outlier Rate
uyku_oncesi_kafein_mg	~6.2%
uyku_oncesi_ekran_suresi_dk	~5.9%
stres_skoru	~1.8%
uykuya_dalma_suresi_dk	~1.0%

The analysis showed that several behavioral variables contained large upper-tail observations.

Outlier analysis was performed diagnostically before preprocessing decisions in order to preserve potentially meaningful behavioral variability.

Correlation Analysis

Pearson correlation analysis was conducted to investigate linear relationships between numerical variables and the target variable.

Variables showing relatively stronger associations with cognitive performance included:

Variable	Approximate Correlation
stres_skoru	-0.59
rem_yuzdesi	0.44
gunluk_calisma_saati	-0.34
derin_uyku_yuzdesi	0.28
gecelik_uyanma_sayisi	-0.27

The analysis suggested that:

higher stress levels,
sleep fragmentation,
longer work duration

were negatively associated with cognitive performance.

In contrast:

higher REM sleep percentage,
higher deep sleep percentage

showed positive associations with cognitive performance scores.

Categorical Variable Analysis

Categorical feature analysis included:

frequency distributions,
category balance examination,
train-test category consistency checks.

The analysis showed that:

category distributions were generally balanced,
train and test datasets shared similar categorical structures,
no major unseen category issue existed between datasets.
Train-Test Consistency Analysis

Train and test datasets were compared to evaluate possible distributional differences.

The comparison included:

KDE distribution comparisons,
missing value pattern comparisons,
categorical level consistency analysis.

The distributions of major numerical variables appeared structurally similar across train and test datasets, indicating the absence of severe distribution shift.

Statistical Characteristics of the Dataset

The dataset exhibits several important statistical properties:

mixed numerical and categorical structure,
moderate missingness,
positively skewed behavioral variables,
bounded continuous target variable,
moderate outlier presence,
potential interaction effects between sleep and lifestyle variables.

The dataset structure is suitable for:

exploratory statistical analysis,
behavioral pattern analysis,
feature engineering,
predictive modeling applications,
multivariate analysis studies.
General Conclusion

The exploratory data analysis demonstrated that the dataset contains meaningful variability across sleep behavior, lifestyle habits, physiological characteristics, and psychological indicators.

The dataset maintains:

relatively low missingness,
manageable outlier levels,
consistent train-test distributions,
moderate feature diversity.

Overall, the dataset provides a statistically rich framework for investigating the relationship between sleep quality, behavioral habits, and cognitive performance outcomes.
