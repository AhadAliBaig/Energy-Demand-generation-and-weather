# Energy Demand, Generation & Weather Analysis

Analysis of Spain's electrical grid data (2015-2018) exploring the relationship between weather patterns, energy demand, and generation sources.

## Dataset

Source: [Kaggle - Energy Dataset](https://www.kaggle.com/datasets/nicholasjhana/energy-consumption-generation-prices-and-weather

- **energy_dataset.csv** — Hourly consumption, generation by source, and pricing
- **weather_features.csv** — Weather data for 5 major Spanish cities

The dataset contains hourly data for:
1. Electrical consumption and generation by source
2. Market prices
3. Weather measurements for five Spanish cities (Madrid, Barcelona, Valencia, Seville, Bilbao)

## Key Findings

### Temperature and Demand Relationship

Temperature affects electricity demand in a non linear pattern. The relationship follows a J curve shape where demand is lowest during mild temperatures (10 to 20 degrees Celsius) and increases sharply during hot weather due to air conditioning usage. Cold weather has a smaller effect on demand compared to hot weather, likely because Spain has mild winters.

The correlation between the five city average temperature and national demand was 0.203. Testing Madrid alone produced a weaker correlation of 0.172, suggesting that averaging across cities captures the overall climate effect better than any single location.

### Seasonal Load Curves

Summer and winter show distinct daily patterns. Both seasons have morning and evening peaks, but winter has a pronounced evening peak around 8 PM reaching approximately 33,500 MW. This is the highest demand point in the dataset. Summer peaks occur earlier, around midday, driven by air conditioning during the hottest hours.

The minimum demand in both seasons occurs between 3 and 4 AM at approximately 23,000 MW.

## Tools Used

Python with pandas, matplotlib, and seaborn for data analysis and visualization.

## Visualizations

### Temperature vs Demand

![Temperature vs Energy Demand](Plots/Temp%20VS%20Energy%20Demand.png)

### Average Demand by Temperature

![Average Demand by Temperature](Plots/Average%20Demand%20by%20Temp.png)

### Seasonal Load Curves

![Load Curve Summer vs Winter](Plots/load%20curve%20winter%20vs%20summer%20wrt%20time.png)

### Price vs Demand

![Price vs Demand](Plots/Price%20vs%20Demand.png)

## Author

Ahad Ali Baig