# IAU Projekt: Detekcia Malware na Mobilných Zariadeniach

Projekt z predmetu Inteligentná analýza údajov (IAU) zameraný na predikciu malware-related-activity na Android mobilných zariadeniach pomocou techník strojového učenia.

## 📋 O Projekte

Cieľom projektu je osvojiť si základné koncepty a techniky analýzy dát, pochopiť fungovanie strojového učenia a získať intuíciu pre ich aplikáciu pri objavovaní znalostí v dátách. Projekt sa zameriava na detekciu malvéru v mobilných zariadeniach na základe systémových logov z Android zariadení zachytených pomocou Rapid7 agenta.

### Predikčná úloha
Predikcia závislej premennej **"mwra"** (malware-related-activity) v časovom intervale na základe systémových charakteristík mobilného zariadenia.

## 🗂️ Štruktúra Repozitára

```
.
├── README.md                   # Tento súbor
├── zadanie1.ipynb              # Fáza 1: Prieskumná analýza
├── zadanie2.ipynb              # Fáza 2: Predspracovanie údajov  
├── zadanie3.ipynb              # Fáza 3: Strojové učenie
├── quest.ipynb                 # Bonusová úloha (Image/Time-series)
├── dataset82/                  # Pôvodný dataset
│   ├── *.csv                   # Surové dátové súbory
│   └── ...
└── dataset82_edited/           # Predspracovaný dataset
    ├── *.csv                   # Očistené dátové súbory
    └── ...
```

## 🚀 Fázy Projektu

### Fáza 1: Prieskumná analýza (15 bodov)
- **Základný opis dát**: Analýza štruktúry, typov a charakteristík dát
- **EDA s vizualizáciou**: Distribúcie atribútov, párová analýza, závislosti
- **Identifikácia problémov**: Duplicitné záznamy, chýbajúce hodnoty, outliers
- **Štatistické testovanie**: Formulácia a overenie hypotéz o dátach

**Súbor**: `zadanie1.ipynb`

### Fáza 2: Predspracovanie údajov (15 bodov)  
- **Príprava dát**: Rozdelenie na train/test, encoding kategorických premenných
- **Feature engineering**: Scaling, transformácie, výber atribútov
- **Pipeline**: Replikovateľné predspracovanie pomocou sklearn.pipeline
- **Feature selection**: Identifikácia najinformatívnejších atribútov

**Súbor**: `zadanie2.ipynb`

### Fáza 3: Strojové učenie (20 bodov)
- **ID3 klasifikátor**: Implementácia vlastného rozhodovacieho stromu
- **Porovnanie algoritmov**: Stromové vs. nestromové metódy
- **Optimalizácia**: Hyperparameter tuning, ensemble learning
- **Validácia**: Cross-validation, detekcia overfittingu/underfittingu

**Súbor**: `zadanie3.ipynb`

### Quest: Bonusová úloha (10 bodov)
Riešenie jednej z dvoch úloh:
- **Q1**: Image classification
- **Q2**: Time-series forecasting

**Súbor**: `quest.ipynb`

## 🛠️ Použité Technológie

- **Python 3.x**
- **Jupyter Notebook**
- **Pandas** - manipulácia s dátami
- **NumPy** - numerické výpočty  
- **Scikit-learn** - strojové učenie
- **Matplotlib/Seaborn** - vizualizácia
- **SciPy** - štatistické testy
- **Statsmodels** - štatistické modelovanie

## 📊 Dataset

Dataset obsahuje logy z Android mobilných zariadení zachytené pomocou **Rapid7** agenta. Dáta sú čiastočne predspracované pre účely projektu.

- **Závislá premenná**: `mwra` (malware-related-activity)
- **Nezávislé premenné**: Rôzne systémové metriky a charakteristiky
- **Formát**: CSV súbory s časovými radmi

### Predspracovanie
- **Pôvodný dataset**: `dataset82/`
- **Predspracovaný dataset**: `dataset82_edited/`

## 👥 Autori

- **Matúš Totcimak**
- **Róbert Šafár**

*Slovenská Technická Uviverzita*  
*Fakulta informatiky a informačných technológií*  
*Bc. štúdium*