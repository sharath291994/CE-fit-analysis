
## Overview

**Zacros CE Fit** is a Python utility for performing **cluster expansion fitting analysis** on AmcBvec file of Zacros CE fit utility. The following statisitcal information is provided by the utility: 

- **Correlation Analysis:** Computes Pearson, Kendall, and Spearman correlation matrices with heatmaps.  
- **Frequency Distributions:** Plots histograms of numeric data for quick exploratory analysis.  
- **Statistical Summary:** Generates detailed descriptive statistics including mean, median, mode, variance, skewness, and kurtosis, saved in an Excel file.  

All outputs are organized into **separate folders** in the same directory as the input Excel file.

Kindly note that this is a beta version. The utility is undergoing further tests and the final version would be uploaded soon.

---

### The following plots are generated using the Zacros CE fit utility ###### 

Correlation Heatmap (Pearson)

Frequency Distribution Histogram


Statistical Summary (Excel)
An Excel file with count, mean, median, mode, std, variance, min, max, quantiles, skewness, and kurtosis for each numeric column.

## Installation

### Prerequisites

- Python >= 3.8
- pip

### Install via pip locally

Clone the repository and install:
git clone https://github.com/sharath291994/zacros_ce_fit.git
cd zacros_ce_fit
pip install .

### Install via pip locally
pip install pandas numpy matplotlib seaborn openpyxl scipy

### Usage

Place your Zacros CE utility  AmcBvec in a directory, then run:

zacros-ce-fit path/to/AmcBvec.xlsx --correlation --histograms --stats

python -m zacros_ce_fit.cli path/to/AmcBvec.xlsx --correlation --histograms --stats

### Options

--correlation : Generate correlation matrices and heatmaps.

--histograms : Generate frequency distribution histograms.

--stats : Generate statistical summary in Excel format.

### Output

Running the utility creates the following folders in the same directory as your Excel file:

correlation_matrices/ – contains Excel files and heatmap images of correlation matrices.

frequency_distributions/ – contains histogram images for each numeric column.

statistical_summary/ – contains statistical_summary.xlsx with descriptive statistics.

### Contributing

Contributions are welcome! Please fork the repository, make your changes, and submit a pull request.

### License

This project is licensed under the MIT License.










