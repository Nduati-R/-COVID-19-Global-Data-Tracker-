# COVID-19 Global Trends Analysis

This project provides an interactive and comparative analysis of global COVID-19 trends using publicly available data from Our World in Data (OWID). It includes data cleaning, time-series visualizations, choropleth maps, and automated insights generation, implemented in a Jupyter notebook.

## Features

* **Data Loading**: Automatically fetches the latest COVID-19 dataset from OWID.
* **Data Cleaning**: Filters for selected countries, forward-fills missing values, and calculates key metrics such as death rate, cases per million, and vaccination rate.
* **Interactive Visualizations**: Plotly line charts for total cases and hoverable metrics (deaths and vaccination rates).
* **Matplotlib Analysis**: Separate charts for each country showing:

  * Total cases over time
  * Total deaths over time
  * Vaccination rate over time
  * Latest death rates comparison
* **Global Choropleth Map**: Visualize cases per million across all countries.
* **Automated Insights**: Summary of highest case counts, vaccination leaders, highest death rates, and average vaccination rates for the analysis period.

## Getting Started

### Prerequisites

* Python 3.7 or higher
* Jupyter Notebook or JupyterLab

### Installation

1. **Clone the repository**

   ```bash
   git clone https://github.com/your-username/covid-trends-analysis.git
   cd covid-trends-analysis
   ```

2. **Create a virtual environment (optional but recommended)**

   ```bash
   python -m venv venv
   source venv/bin/activate  # macOS/Linux
   venv\Scripts\activate   # Windows
   ```

3. **Install the dependencies**

   ```bash
   pip install -r requirements.txt
   ```

   *(If `requirements.txt` is not provided, the key packages are: pandas, numpy, matplotlib, plotly.)*

### Running the Notebook

1. Launch Jupyter:

   ```bash
   jupyter notebook
   ```

2. Open `covid_trends_analysis.ipynb` and run all cells in order.

## File Structure

```
├── covid_trends_analysis.ipynb   # Main analysis notebook
├── requirements.txt              # Project dependencies
└── README.md                     # Project overview and instructions
```

## Customization

* **Target Countries**: Modify the `target_countries` list in the notebook to analyze different countries.
* **Additional Metrics**: Extend the data cleaning section to compute metrics like ICU rate or positivity rate.
* **Visualization Styles**: Update Plotly themes or Matplotlib settings to suit your preferences.

## Technical Details

* **Data Source**: [Our World in Data COVID-19 Dataset](https://covid.ourworldindata.org/data/owid-covid-data.csv)
* **Data Cleaning**: Forward-fill (`ffill`) to handle missing daily records; filter death rates to valid ranges.
* **Visualization**: Plotly for interactivity; Matplotlib for static charts, each in separate figures to comply with style guidelines.

## License

This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.

---

*Created on May 19, 2025.*
