# IEAP-Series04-RStudio

Team assignment on linear and non-linear regressions, for the Python, Git and RStudio course (Master IEAP, Université de Montpellier).

**Authors:** Zoé Sauge, Gaia Gassiole, Jeanne Le Roux

## Content

1.  **Effect of random noise on linear regression**, using simulated data.
2.  **Mathematical model of heart rate recovery after exercise**, comparing linear, mono-exponential and bi-exponential models on two real recordings.

## Repository structure

## Repository structure

``` text
├── data/
│   ├── pulse_3h.csv              # heart rate, 3h10 recording
│   ├── acceleration_3h.csv       # acceleration, 3h10 recording
│   ├── pulse7m30.csv             # heart rate, 7m30 recording
│   └── acceleration7m30.csv      # acceleration, 7m30 recording
├── .gitignore
├── IEAP-Series04-RStudio.Rproj   # RStudio project
├── IEAP-Series04-Rstudio.qmd     # master document
├── IEAP-Series04-Rstudio.md      # Markdown version, readable on GitHub
├── LICENSE
├── README.md
├── _git-workflow.qmd             # analysis of our Git workflow
├── _problem1.qmd                 # problem 1: effect of noise
├── _problem2-3h.qmd              # problem 2: literature and 3h10 recording
├── _problem2-7m.qmd              # problem 2: 7m30 recording
├── _problem2-conclusion.qmd      # problem 2: general conclusion
├── apa.csl                       # APA citation style
└── references.bib                # bibliography
```

## How to reproduce the report

1.  Clone this repository and open `IEAP-Series04-RStudio.Rproj` in RStudio.

2.  Install the required packages, if needed:

    ``` r
    install.packages(c("tidyverse", "lmtest"))
    ```

3.  Open `IEAP-Series04-Rstudio.qmd` and click **Render**.

Always render the master document, because the libraries are loaded there and not in the sub-documents.

## Data

The heart rate and acceleration files come from two public [Aidlab](https://www.aidlab.com) recordings, of 3h10 and 7m30. Timestamps are in Unix milliseconds.

## License

See [LICENSE](LICENSE).
