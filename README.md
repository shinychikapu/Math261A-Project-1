# Math 261A Project 1

**Author:** Gia Thy Le  
**Date:** September 25, 2026

## Research Question

Is there an association between 11th-grade Math and ELA CAASPP mean scale scores across California schools?

## Project Structure

- `paper/paper.qmd`: Quarto source file for the paper
- `paper/paper.pdf`: Rendered PDF report
- `paper/references.bib`: Bibliography file
- `data/` — Local data files, excluded from GitHub using `.gitignore`
- `Math261A-Project-1.Rproj` — RStudio project file
- `.gitignore` — Files excluded from the repository

## Data

The data come from the California Assessment of Student Performance and Progress (CAASPP) 2024–25 Smarter Balanced Summative Assessments:

<https://caaspp-elpac.ets.org/caaspp/ResearchFileListSB?ps=true&lstTestYear=2024&lstTestType=B&lstCounty=00&lstDistrict=00000&lstFocus=a>

The data are publicly available through the California Department of Education. The raw data are not included in this repository. No separate dataset license was listed on the download page.

## Reproducing the Analysis

### Requirements

- R
- RStudio or another R-compatible editor
- Quarto
- The `tidyverse` R package

### Steps

1. Clone this repository:

```bash
git clone https://github.com/shinychikapu/Math261A-Project-1.git
cd Math261A-Project-1
```

2. Install the required R package:

```r
install.packages("tidyverse")
```

3. Download the 2023–24 CAASPP Smarter Balanced research file from the [California Department of Education](https://caaspp-elpac.ets.org/caaspp/ResearchFileListSB?ps=true&lstTestYear=2024&lstTestType=B&lstCounty=00&lstDistrict=00000&lstFocus=a).

4. Save the downloaded file to the data folder:
   
```text
data/sb_ca2024_1_csv_v1.csv
```
Raw and cleaned external data are not included in this repository. Users must download the data themselves.

5. Open `paper.qmd` and render with RStudio or run individual code blocks manually. No seed is needed because using the same data file and code will reproduce the same results.

## External Resources

I used ChatGPT as an external resource to help debug R and Quarto code, and improve the organization and wording of the
paper. I selected the research question, conducted the analysis, verified the results, and made the final decisions about the code and report.
