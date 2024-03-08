# King-County-Washington-House-Sales Analysis

### Project Overview

Barcelona, a captivating city steeped in history, culture, and vibrant energy, has long captivated the hearts of travelers and potential residents alike. However, the allure of Barcelona often comes with a hefty price tag, particularly in the realm of housing costs. To shed light on Barcelona’s rental market, we delve into the “Barcelona Price Rent From 2014 to 2022” dataset, exploring trends, patterns, and potential factors influencing rental prices.

Examining the dataset’s data from 2014 to 2022, a clear upward trend emerges in both average rent and average price for apartments in Barcelona. This indicates a consistent increase in rental costs across the city over the analyzed period. 

### Exploring the Dimensions of a House Rent Price Dataset

In the realm of real estate analysis, understanding the factors that influence property values is crucial for making informed investment decisions. the key features often included:
- The Year
- Trimester
- District
- Neighbourhood


Year: The Year feature captures the time period in which the house was built. This information is essential for understanding how market conditions have evolved over time. For instance, a dataset spanning several years can reveal how property values have fluctuated in response to economic cycles, government policies, and other external factors. By analyzing year-over-year changes, we can identify periods of growth or decline and gain insights into the overall health of the housing market.

Trimester: The Trimester feature categorizes the house price data into three-month intervals, allowing us to investigate seasonal patterns in property values.

District: The District feature divides the dataset into distinct geographical areas, enabling us to analyze how house prices vary across different regions.

Neighbourhood: The Neighbourhood feature goes a step further by segmenting the data into even smaller geographical areas, providing a more granular view of house price variations.


### Data Sources
The data for this dashboard was collected from a variety of sources, including Idealista, Fotocasa, and Numbeo
[Donwload](https://www.kaggle.com/datasets/salaudeentaofeek/barcelona-price-rent-dataset-from-2014-2022)

### Methodology
The data was cleaned and preprocessed on Jupyter Notebook before being used to create the visualizations. The visualizations were created using PowerBi.


### Tools
- Python for Analysis
- Power Bi for Visualizatiob


### Data Overview with Python on Jupyter Nootbook.

```sql
# Checking out the data 
df.head()

Year	Trimester	District	Neighbourhood	Average _rent	Price
0	2014	1	Ciutat Vella	el Raval	average rent (euro/month)	589.55
1	2014	1	Ciutat Vella	Gothic Quarter	average rent (euro/month)	712.79
2	2014	1	Ciutat Vella	la Barceloneta	average rent (euro/month)	540.71
3	2014	1	Ciutat Vella	Sant Pere, Santa Caterina i la Ribera	average rent (euro/month)	673.44
4	2014	1	Eixample	Fort Pienc	average rent (euro/month)	736.09
```

```sql
# Checking the categorical unique values in "Year"
df["Year"].unique()

array([2014, 2015, 2016, 2017, 2018, 2019, 2020, 2021, 2022])
```
```sql
# Checking the categorical unique values in "Trimester"
df["Trimester"].unique()

array([1, 2, 3, 4])
```
```sql
df['Year'].value_counts()

2015    552
2016    552
2014    546
2017    546
2018    540
2021    540
2019    538
2020    538
2022    270
Name: Year, dtype: int64
```

```sql
# Checking if there are any null values 
df.isnull().sum()

Year             0
Trimester        0
District         0
Neighbourhood    0
Average _rent    0
Price            0
dtype: int64
```

```sql
df.describe().T

count	mean	std	min	25%	50%	75%	max
Year	4622.0	2017.745565	2.462828	2014.00	2016.0	2018.00	2020.0000	2022.0
Trimester	4622.0	2.440502	1.116377	1.00	1.0	2.00	3.0000	4.0
Price	4622.0	416.457594	442.872305	3.18	12.1	81.82	777.2075	2034.0
```

### Data Insight
1. The Top 10 District in Barcelona with the Highest House Rent: This is crucial for understanding the influence of local factors such as infrastructure, proximity to amenities, and crime rates on property values. By comparing prices across districts, we can identify areas that offer higher returns on investment or that may be more affordable for potential buyers or Rentals.


2. This image shows the minimum and maximum price house rent from 2014 to 2022 and it can be deduced that 2015 has the longest margin between minimum and maximum house rent per year.

3. The Population of Neighbourhood: This information is particularly valuable for understanding the impact of neighborhood-specific factors such as schools, parks, and community characteristics on property values. By comparing prices across neighborhoods, we can identify areas that offer unique amenities or desirable lifestyles, potentially influencing buyer preferences and driving up prices.

This image shows the percentage of the most populated neighborhood. the moat populated environment is Can Baro and Ciuta Meridiana having 29.57% each, Canyelles with 27.83%, Baro de Viver with 8.70% and Can Paguera with 4.35%.

4. This image shows the overall average House rent from 2014 to 2022 by Year in (€)

### Recommendations
- Tenants should consider the district, neighborhood, and size of the property when making a decision about where to rent.
- Landlords should consider the average rent in the district and neighborhood when setting their rental prices.

### Limitation
The data for this dashboard is limited to rental properties in Barcelona. The data may not be representative of all rental properties in Spain.



I hope this dashboard is informative. Comment and please let me know if you have any questions.

![Capture01](https://github.com/SalaudeenTaofeek/King-County-Washington-House-/assets/123555622/a16e3ec9-a6a7-4180-9009-5aad4b2adb6a)




