# Datasets

The notebooks in this repository were run on Cornell Tech's JupyterHub, where the datasets
were pre-loaded. To keep this repository lightweight and to respect data licensing, **the
dataset files themselves are not committed here** (the `.gitignore` excludes them).

Place any datasets you download into this `data/` folder, then update the file path near the
top of the relevant notebook if needed.

## Datasets referenced across the notebooks

| Dataset (filename in notebooks) | Used in | Description | Where to obtain |
|---|---|---|---|
| `Iris_Data.csv` | Unit 3 (KNN) | Classic 3-class flower dataset | [UCI Iris](https://archive.ics.uci.edu/dataset/53/iris) / bundled with scikit-learn |
| `WHR2018Chapter2OnlineData.csv` | Unit 4 | World Happiness Report 2018 | [World Happiness Report — data](https://worldhappiness.report/archive/) |
| `censusData.csv`, `censusData_missingValues.csv` | Units 2, 5 | 1994 U.S. Census / "Adult" income data | [UCI Adult / Census Income](https://archive.ics.uci.edu/dataset/2/adult) |
| `airbnbListingsData.csv`, `airbnbData*.csv` | Units 2, 5, 6 | NYC Airbnb listings | [Inside Airbnb — NYC](http://insideairbnb.com/get-the-data/) |
| `bookReviewsData.csv`, `bookReviews.csv` | Unit 8 (Capstone) | Book reviews with sentiment labels | Program-provided (Break Through Tech / Cornell Tech) |
| `cell2cell.csv`, `cell2celltrain.csv` | Units 5–6 | Telecom customer-churn dataset | Public "Cell2Cell" telecom churn dataset |
| `spamDataset.csv` | Unit 8 | SMS/text spam classification | [UCI SMS Spam Collection](https://archive.ics.uci.edu/dataset/228/sms+spam+collection) |
| `HousingPrices.csv` | Unit 6 | Housing price regression | Program-provided |
| `FlightInformation.csv` | Unit 2 | Flight records | Program-provided |
| `Top100Restaurants2020.csv` | Unit 2 | Restaurant rankings | Program-provided |
| `ZooData.csv` | Unit 3 | Animal-attribute classification | [UCI Zoo](https://archive.ics.uci.edu/dataset/111/zoo) |

> **Note on program-provided datasets:** a few files were prepared specifically for the
> Break Through Tech / Cornell Tech course and may not be publicly downloadable. Those
> notebooks are still fully readable here because they are committed **with their outputs
> intact** — you can see every result without re-running them.

## Reproducibility tip

Most notebooks load data with a line similar to:

```python
import os
filename = os.path.join(os.getcwd(), "data", "someDataset.csv")
df = pd.read_csv(filename)
```

If your file lives elsewhere, just adjust that path.
