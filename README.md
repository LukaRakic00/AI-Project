# Weather Prediction using AI

Ovaj projekat koristi veštačku inteligenciju (AI) i mašinsko učenje (ML) za predviđanje vremenskih uslova, uključujući temperaturu, vlažnost, padavine i druge ključne meteorološke parametre. Koristi se kombinacija istorijskih podataka o vremenu i sofisticiranih algoritama za analizu i prognoziranje budućih vremenskih obrazaca.

## Funkcionalnosti

- Predikcija temperature, vlažnosti i padavina za zadati vremenski period.
- Korišćenje različitih algoritama mašinskog učenja, uključujući Linear Regression, Random Forest i Neural Networks.
- Analiza vremenskih podataka prikupljenih iz različitih izvora (npr. lokalne stanice, open-source vremenske baze podataka).
- Vizualizacija podataka i predikcija putem grafikona.
- Automatsko ažuriranje podataka o vremenu pomoću API-ja za vreme (npr. OpenWeatherMap API).

## Tehnologije korišćene

- **Programski jezik**: Python
- **Biblioteke**:
  - `TensorFlow` - za kreiranje i obuku neuronskih mreža.
  - `scikit-learn` - za primenu algoritama mašinskog učenja.
  - `pandas` i `numpy` - za obradu i analizu podataka.
  - `matplotlib` i `seaborn` - za vizualizaciju podataka.
  - `OpenWeatherMap API` - za prikupljanje trenutnih vremenskih podataka.

## Instalacija

1. **Preuzimanje projekta**:
   - Kloniraj repozitorijum koristeći Git:
     ```bash
     git clone https://github.com/tvoje-korisnicko-ime/weather-prediction-ai.git
     ```

2. **Instalacija zavisnosti**:
   - Pre nego što pokreneš projekat, instaliraj potrebne biblioteke:
     ```bash
     pip install -r requirements.txt
     ```
   - Ako ne postoji `requirements.txt` fajl, dodaj ručno sledeće biblioteke:
     ```bash
     pip install tensorflow scikit-learn pandas numpy matplotlib seaborn
     ```

3. **Postavljanje API ključa**:
   - Prijavi se na [OpenWeatherMap](https://openweathermap.org/) i kreiraj API ključ.
   - U projektu napravi `.env` fajl i postavi API ključ ovako:
     ```bash
     WEATHER_API_KEY=your_api_key_here
     ```

## Korišćenje

1. **Prikupljanje podataka**:
   - Pokreni skriptu za prikupljanje vremenskih podataka koristeći OpenWeatherMap API:
     ```bash
     python fetch_weather_data.py
     ```

2. **Obuka modela**:
   - Pokreni skriptu za obuku modela na prikupljenim podacima:
     ```bash
     python train_model.py
     ```

3. **Predikcija vremena**:
   - Nakon obuke, koristi model za predikciju vremenskih uslova:
     ```bash
     python predict_weather.py --days 5
     ```

4. **Vizualizacija podataka**:
   - Vizuelizuj predikcije vremena pomoću grafika:
     ```bash
     python visualize_predictions.py
     ```

