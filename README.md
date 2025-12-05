# Smiley Real Estate Analysis
A compact data-analysis project that explores a large-scale view of sales performance through most of 2025 and residential real estate trends. Provides reproducible scripts and notebooks for cleaning, analysis, and visualization.

## Instructions
**Final deliverable**
      <br> The primary deliverable for this submission is a single HTML report. Reviewers can open the HTML in a browser with no code execution required.

**Quick instructions**
    <br>*Open the HTML file (no R required)*
1. Find the HTML file in the repository (Clever-Real-Estate-Working-Interview-Project.html)
2. Download and open locally:
    - Option A: Click the file in GitHub, click "Raw", then Save As to download the `.html` file. Double-click the saved file to open in your browser.
    - Option B: click the download icon in the top right. Double-click the downloaded file to open in your browser.

*Run the R Markdown (if you need to re-render the HTML)*
<br>Prerequisites
- R (>= 4.0 recommended) installed: https://cran.r-project.org/
- (Optional) RStudio for an IDE with a Knit button: https://posit.co/download/
- Required R packages: `rmarkdown`, `readr`, `tidyverse`, `rlang`, `purrr`, `plotly`, `knitr`, `kableExtra`, `scales`, `stringr`

Render from R (recommended) <br>
Open R or RStudio and run:
```r
rmarkdown::render("path/to/report.Rmd")
```

Render from the command line
```bash
Rscript -e "rmarkdown::render('path/to/report.Rmd')"
```

Make a single self-contained HTML
If you want one file that contains all resources (CSS, JS, images), render with:
```r
rmarkdown::render("path/to/report.Rmd", output_options = list(self_contained = TRUE))
```
Note: self_contained = TRUE can increase file size.


## Repository Contents
| File Name | Description | Purpose |
| :--- | :--- | :--- |
| **README.md** | (This file) | Overview of the repository and project. |
| **agents.csv** | Raw dataset that provides information on real estate agents in the Smiley Real Estate network. | Input data for agent analysis. |
| **best_agents_per_market.csv** | Full dataset with all top agents per market. | Full list of top agents for stakeholder interest. |
| **calls.csv** | Raw dataset that indicates the times at which each customer called the company and the outcome of that call. | Input data for call analysis. |
| **customers.csv** | Raw dataset that lists basic information about each customer - a unique ID, name, address, etc. | Input data for customer analysis. |
| **markets.csv** | Raw dataset that provides information on the fifty markets served by Smiley Real Estate. | Input data for market analysis.|
| **sales.csv** | Raw dataset that indicates the time of a successful sale, identifying the CustomerID, the time of the sale, and the value of the property sold. | Input data for sales analysis. |
| **Clever Real Estate Working Interview Project.Rmd** | The **R Markdown** script containing all data cleaning, scoring models, visualizations, and conclusions. | The executable source code for the entire analysis and the final deliverable. |
| **Clever-Real-Estate-Working-Interview-Project.html** | The **HTML** report generated from the R Markdown file containing all visualizations and conclusions. | The final deliverable for the stakeholders. |
