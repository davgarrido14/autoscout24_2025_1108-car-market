# 🚗 Used Car Market Analysis — Autoscout24 (Dataset: 2025‑11‑08)
A data exploration project by David

📌 Overview
This project analyzes 118,382 used car listings from Autoscout24, collected on 2025‑11‑08. The goal is to understand pricing patterns, brand behavior, vehicle age distribution, fuel types, and broader market dynamics. The analysis combines statistical methods, visual exploration, and data cleaning to uncover meaningful trends in the European used‑car market.

## 📊 Key Findings
1. Price Distribution (after removing top 1%)
The price distribution is right‑skewed, even after trimming the top 1% of extreme luxury outliers. Most cars fall between €10,000 and €40,000, with frequency dropping steadily as prices rise.

This suggests:

The market is dominated by mid‑range vehicles.

Luxury cars exist but represent a small fraction of listings.

Removing the top 1% gives a much clearer view of the “real” market.

## 2. Year Distribution
The dataset is heavily concentrated in recent model years, with a sharp rise starting around 2000 and peaking around 2023.

This reflects:

The used‑car market is dominated by relatively new vehicles.

Very old cars (pre‑1980) are rare and likely represent collector or specialty listings.

The dataset aligns with typical consumer behavior: buyers prefer newer models with modern features.

## 3. Fuel Consumption Distribution
Fuel consumption clusters strongly between 0 and 20 L/100km, with a clear peak in the lower end of that range.

Interpretation:

Most vehicles are reasonably fuel‑efficient.

Extremely high consumption values exist but are rare (likely SUVs, sports cars, or data errors).

The distribution supports the idea that efficiency remains a key factor in the used‑car market.

## 4. Fuel Category Breakdown
Gasoline and Diesel dominate the dataset:

Gasoline: ~50k listings

Diesel: ~37k listings

Electric and hybrid categories appear but remain a minority.

LPG, CNG, and Ethanol are niche.

This mirrors the current European market, where electrification is growing but still far from overtaking traditional fuel types in the used‑car segment.

## 5. Car Brand Frequency
The most common brands in the dataset are:

BMW

Porsche

Mercedes‑Benz

Audi

These brands dominate the platform, suggesting:

Strong resale markets

High listing turnover

Strong brand loyalty and demand

Smaller brands appear but with much lower frequency.

## 6. Price Distribution by Brand
Boxplots reveal massive differences between brands:

Bugatti, Rolls‑Royce, Maybach sit at the extreme high end.

Porsche, Aston Martin, Maserati show wide price ranges with many outliers.

Volkswagen, Hyundai, Suzuki, Renault cluster in the lower to mid‑range.

BMW, Audi, Mercedes‑Benz show broad distributions, reflecting diverse model lineups.

Using a logarithmic scale makes these differences interpretable without letting ultra‑luxury brands distort the entire plot.

## 7. Top 12 Brands — Focused Price Comparison
When limiting the analysis to the 12 most common brands, the price distributions become much clearer:

Aston Martin and Porsche still show high‑end outliers.

BMW, Audi, Mercedes‑Benz remain mid‑to‑high range with wide spreads.

Hyundai, Suzuki, Opel cluster tightly at lower prices.

This filtered view avoids distortion from rare luxury brands and highlights mainstream market behavior.

## 8. Price vs. Year by Brand
Plotting price against year for each brand shows:

Newer cars tend to be more expensive (expected).

Some brands (e.g., Porsche, Aston Martin) retain high value even for older models.

Budget brands show tighter, more predictable depreciation curves.

Luxury brands show extreme variance — older models can still command high prices.

This reinforces the idea that brand identity strongly influences depreciation.

## 9. Market Share Treemap
A treemap of listing counts shows:

BMW, Porsche, Mercedes‑Benz, Audi dominate the dataset.

Mid‑tier brands like Ford, Volvo, Suzuki, Honda occupy smaller but meaningful portions.

Niche brands appear as tiny rectangles.

This visualization makes the market structure immediately clear.

## 🧠 Statistical Insight: Brand Matters — A Lot
An ANOVA test comparing price across brands produced:

Code
F = 4534.41  
p = 0.0
This means:

Price differences between brands are statistically significant.

Brand is one of the strongest predictors of price in the dataset.

The effect size is extremely large.

## 🚀 Next Steps
Planned additions to the project:

Regression modeling to predict price

Clustering to identify market segments

Outlier detection for suspicious listings

Country‑level comparisons (if data becomes available)

Interactive dashboards (Plotly or Streamlit)

# 🎯 Summary
Your analysis paints a clear picture of the used‑car market:

The market is dominated by recent, mid‑priced, gasoline/diesel vehicles.

Brand identity is one of the strongest drivers of price.

Luxury brands create extreme outliers that require careful handling.

The dataset reflects real‑world trends: electrification is growing but not yet dominant.
