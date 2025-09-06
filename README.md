
## Overview

**Zacros CE Fit** is a Python utility for performing **cluster expansion fitting analysis** on AmatBvec file of Zacros CE fit utility. The following statisitcal information is provided by the utility: 

- **Correlation Analysis:** Computes Pearson, Kendall, and Spearman correlation matrices with heatmaps.  
- **Frequency Distributions:** Plots histograms of numeric data for quick exploratory analysis.  
- **Statistical Summary:** Generates detailed descriptive statistics including mean, median, mode, variance, skewness, and kurtosis, saved in an Excel file.  

All outputs are organized into **separate folders** in the same directory as the input Excel file.

Kindly note that this is a beta version. The utility is undergoing further tests and the final version will be uploaded soon.

---

### The following plots are generated using the Zacros CE fit utility ###### 

### Correlation Matrix
![Correlation Example](examples/correlation_pearson.png)

### Frequency Distribution
![Histogram Example](examples/frequency_plot.png)
Statistical Summary (Excel)

### Prerequisites
- Python >= 3.8
- pip

### Installation procedure
Clone the repository and install:
git clone https://github.com/sharath291994/Zacros_CE_fit.git
pip install .

### Install via pip locally
pip install pandas numpy matplotlib seaborn openpyxl scipy

### Usage
Please follow the following steps to generate the results using the Zacros CE utility: 
1) Place your Zacros CE utility  AmatBvec in a directory.
2) In the Windows command window, run the command: zacros-ce-fit path/to/AmatBvec.xlsx --correlation --histograms --stats
3) Alternatively, you can run the following command: python -m zacros_ce_fit.cli path/to/AmcBvec.xlsx --correlation --histograms --stats

### Options
The following options are available in the utility: 
--correlation : Generate correlation matrices and heatmaps.
--histograms : Generate frequency distribution histograms.
--stats : Generate statistical summary in Excel format.

### Output
Running the utility creates the following folders in the the directory where your AmatBvec.xlsx file is stored:
correlation_matrices/ – contains Excel files and heatmap images of correlation matrices.
frequency_distributions/ – contains histogram images for each numeric column.
statistical_summary/ – contains statistical_summary.xlsx with descriptive statistics.

### Contributing
Contributions are welcome! Please fork the repository, make your changes, and submit a pull request.

### License
This project is licensed under the MIT License.
















