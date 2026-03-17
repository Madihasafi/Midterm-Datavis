# Midterm-Datavis

# Flight Delay Analysis: Airline Punctuality & Airport Performance

This project explores flight delay data from the Bureau of Transportation Statistics to answer two key questions:

- Which years were airlines most punctual?
- Which airports experience the worst (and best) delays?

Using interactive Plotly visualizations, we uncover trends in delay causes over two decades and rank airports by security delays and average delay length.

## 📁 Datasets

The analysis uses two datasets:

1. **Flight Delays Complete Analysis 2003–2025 Detailed.csv**  
   Aggregated yearly data showing the percentage of delays attributed to:
   - Air Carrier
   - Aircraft Arriving Late
   - National Aviation System
   - Security
   - Extreme Weather
   - Total Weather Share

2. **Flight Delays Complete Analysis 2003–2025 Detailed (1).csv** (airport summary)  
   Contains airport‑level metrics:
   - Security delays per 1,000 flights
   - Average delay length (minutes)
   - Airport names and codes

## 🔍 Analysis Steps

1. **Data Cleaning**  
   - Removed empty columns and descriptive rows.  
   - Renamed columns for clarity.  
   - Extracted 3‑letter airport codes.  
   - Handled missing values.

2. **Visualization**  
   - **Line charts** for yearly trends of each delay category (2003–2023).  
   - **Bar charts** for top/bottom airports by security delays and average delay length.  
   - All charts are interactive (hover, zoom, pan) using Plotly.

3. **Key Insights**  
   - **Air carrier delays** peaked in 2019 (33.49%) and were lowest in 2012 (28.12%).  
   - **Late‑arriving aircraft delays** peaked in 2012 (42.29%), lowest in 2004 (37.04%).  
   - **Security delays** are negligible (≤0.01%) across all years.  
   - **Weather delays** varied widely: highest 49.92% (2003), lowest 27.14% (2023).  
   - **Most punctual airport (security)**: Miami (MIA) with 2.5 delays/1000 flights.  
   - **Least punctual airport (security)**: Honolulu (HNL) with 7.0 delays/1000 flights.  
   - **Shortest average delay**: Fort Lauderdale (FLL) at 31.9 minutes.  
   - **Longest average delay**: Seattle (SEA) at 57.8 minutes.

## 🛠️ Requirements

- Python 3.8+
- pandas
- plotly
- numpy

Install with:
```bash
pip install pandas plotly numpy
