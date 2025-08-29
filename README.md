# 🏠 House Price Prediction -- Regression Models

Dieses Projekt untersucht das **King County Housing Dataset** (Seattle,
USA) und zeigt, wie man mit Python und gängigen
Machine-Learning-Methoden Hauspreise vorhersagen kann.\
Es kombiniert **explorative Datenanalyse (EDA)**,
**Korrelationsanalyse** und **lineare / polynomiale Regression**.

------------------------------------------------------------------------

## 📂 Inhalt

-   **Datenbereinigung**: Entfernen irrelevanter Spalten, Auffüllen
    fehlender Werte (`bedrooms`, `bathrooms`).
-   **Explorative Analyse**: Scatterplots, Boxplots, Heatmaps zur
    Untersuchung von Zusammenhängen mit dem Preis.
-   **Feature Selection**: Pearson-Korrelation als Kriterium zur Auswahl
    signifikanter Features.
-   **Modelle**:
    -   Lineare Regression (`LinearRegression`)
    -   Polynomiale Regression mit Ridge-Regularisierung (Pipeline:
        `StandardScaler` → `PolynomialFeatures` → `Ridge`)
-   **Evaluierung**:
    -   Cross-Validation Scores auf Trainingsdaten
    -   R²-Score auf Testdaten
-   **Visualisierung**:
    -   KDE-Plots der Vorhersagen vs. tatsächliche Preise
    -   Heatmaps der Korrelationen

------------------------------------------------------------------------

## ⚙️ Installation

### 1. Repository klonen

    git clone https://github.com/deinusername/house-price-prediction.git
    cd house-price-prediction

### 2. Virtuelle Umgebung erstellen (optional, empfohlen)

    python -m venv venv
    source venv/bin/activate   # Linux/Mac
    venv\Scripts\activate      # Windows

### 3. Abhängigkeiten installieren

    pip install -r requirements.txt

------------------------------------------------------------------------

## 📊 Verwendung

    python house_price_regression.py

-   Das Skript lädt die Daten aus `house_data.csv`.
-   Führt Bereinigung, Analyse und Modelltraining durch.
-   Zeigt Plots & Modell-Performance im Terminal an.

------------------------------------------------------------------------

## 📦 Benötigte Libraries

-   pandas\
-   numpy\
-   matplotlib\
-   seaborn\
-   scikit-learn\
-   scipy

------------------------------------------------------------------------

## 🖼 Beispielplots

-   Scatterplots & Regressionslinien für numerische Features
-   Heatmap der Korrelationen\
-   Vergleich der Modellvorhersagen per KDE-Plot

------------------------------------------------------------------------

## 🚀 Nächste Schritte / Ideen

-   Erweiterung der Feature-Engineering-Strategie (z. B.
    log-Transformation von `price`).
-   Hyperparameter-Tuning (GridSearchCV für `alpha`, `degree`).
-   Mehr Modelle testen (Random Forest, Gradient Boosting).
-   Deployment als Web-App (z. B. Streamlit).

------------------------------------------------------------------------

## 📜 Lizenz

Dieses Projekt steht unter der **MIT Lizenz**.
