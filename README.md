# YZTA-2026---Datathon
Dataset Overview

This dataset is a synthetic tabular dataset designed to investigate the relationship between individuals’ sleep habits, lifestyle characteristics, physiological and psychological conditions, and cognitive performance levels. Each observation in the dataset represents a single individual and includes a combination of demographic, behavioral, sleep-related, and health-related variables.

The primary objective of the dataset is to analyze how different sleep behaviors and daily lifestyle patterns may influence cognitive performance. The target variable of the dataset is bilissel_performans_skoru, a continuous numerical variable representing an individual’s cognitive performance score on a scale between 0 and 10.

The dataset consists of:

Training set: 56,000 observations
Test set: 24,000 observations

The training dataset includes the target variable, whereas the test dataset does not contain target information.

Variable Categories

The dataset contains variables belonging to several different categories.

Demographic Variables

These variables describe the general characteristics of individuals.

Examples:

yas
cinsiyet
ulke
meslek
Sleep-Related Variables

These variables describe sleep quality and sleep behavior patterns.

Examples:

rem_yuzdesi
derin_uyku_yuzdesi
uykuya_dalma_suresi_dk
gecelik_uyanma_sayisi
hafta_sonu_uyku_farki_saat
kronotip

These variables provide information regarding:

sleep efficiency,
sleep fragmentation,
circadian rhythm tendencies,
recovery quality.
Lifestyle Variables

These variables reflect daily routines and behavioral habits.

Examples:

uyku_oncesi_ekran_suresi_dk
uyku_oncesi_kafein_mg
gunluk_calisma_saati
gunluk_adim_sayisi
gun_tipi

These features help evaluate:

screen exposure before sleep,
caffeine consumption,
physical activity levels,
work intensity,
weekday/weekend behavioral differences.
Physiological and Psychological Variables

These variables represent physical and mental health indicators.

Examples:

stres_skoru
ruh_sagligi_durumu
dinlenik_nabiz_bpm
vucut_kitle_indeksi

These variables may reflect:

stress levels,
cardiovascular condition,
body composition,
psychological well-being.
Exploratory Data Analysis (EDA)

An extensive exploratory data analysis (EDA) process was conducted in order to better understand the structural characteristics of the dataset before preprocessing and modeling stages.

The EDA process included:

dataset shape and variable type examination,
missing value analysis,
duplicate observation checks,
distribution analysis of numerical variables,
categorical variable frequency analysis,
outlier detection,
train-test distribution consistency checks,
target variable analysis,
correlation analysis,
feature relationship exploration.
Missing Value Analysis

Missing value analysis showed that several variables contained a relatively small proportion of missing observations. The columns with missing values were:

kronotip
vucut_kitle_indeksi
stres_skoru
uyku_oncesi_kafein_mg
meslek
ruh_sagligi_durumu

The missing value ratios were generally between approximately 2% and 4%, indicating that the dataset remained largely complete.

During EDA, both numerical summaries and visual inspections were performed to understand missingness patterns across variables. In addition, row-level missing value counts were examined to determine whether missing observations accumulated in specific records.

Because the missing value proportions were relatively low, row or column deletion strategies were not preferred in order to avoid unnecessary information loss.

Outlier Analysis

Potential outlier observations were examined particularly for numerical variables related to:

caffeine consumption,
screen time before sleep,
stress score,
sleep latency,
nap duration.

Boxplots and distribution visualizations were used to identify extreme observations and investigate distributional skewness. The analysis showed that some behavioral variables exhibited right-skewed distributions and contained unusually large values.

At the exploratory stage, outlier analysis was performed diagnostically rather than directly removing observations. This approach allowed the preservation of potentially meaningful behavioral variability while still identifying variables that might require preprocessing adjustments later.

Distribution Analysis

The distributions of numerical variables were analyzed using:

histograms,
kernel density plots,
boxplots.

These analyses revealed that several variables displayed non-normal and skewed distributions, particularly variables associated with lifestyle behaviors and sleep habits.

The target variable, bilissel_performans_skoru, was also examined to understand its overall distribution and variability across observations.

Correlation and Relationship Analysis

Correlation analysis was conducted to investigate linear relationships between numerical variables and the target variable.

The analysis particularly focused on variables associated with:

stress,
sleep quality,
sleep disruption,
physical activity,
recovery indicators.

Additionally, feature relationship exploration was performed through pairwise visualizations and grouped analyses to better understand possible interactions between behavioral and physiological variables.

Train-Test Consistency Analysis

Train and test datasets were compared to evaluate potential distributional differences between the two sets.

This analysis included:

numerical distribution comparisons,
categorical level consistency checks,
missing value pattern comparisons.

The results indicated that the train and test datasets generally shared similar structural properties, suggesting that no major distribution shift existed between the two datasets.

General Characteristics of the Dataset

Overall, the dataset provides a rich multivariate structure containing:

numerical variables,
categorical variables,
behavioral indicators,
physiological measurements,
psychological factors.

The dataset combines information from multiple domains related to sleep, health, and lifestyle, making it suitable for comprehensive exploratory analysis and predictive modeling studies focused on cognitive performance.
