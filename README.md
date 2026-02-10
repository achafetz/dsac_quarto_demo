# DSAC Quarto Demo

Demo on how to utilize Quarto in DSAC workflow

## About the Project 
This repository is used to demonstrate some of the benefits and features of leveraging Quarto for R/python analyses and how it can then be published to GitHub Pages.

### View Live Site

- [General overview](about.html) of Quarto
- [Slides](slides.html)
- [Base demo version](demo_base.html) version of an analysis done in Quarto
- [Fancy demo version](demo_fancy.html) an analysis done in Quarto


## Local Development
Install required packages:
- R >= 4.0
- Quarto >= 1.3
- tidyverse

Download the data:
[Download the Medicare Monthly Enrollment data](https://data.cms.gov/summary-statistics-on-beneficiary-enrollment/medicare-and-medicaid-reports/medicare-monthly-enrollment) and unzip directly into the project folder.

### Rendering
Run `quarto render` to build the site locally.


## Repository Structure

Below is the folder structure for this repository, run with `r fs::dir_tree(recurse = 0)`.

```
.
├── COMMUNITY.md
├── CONTRIBUTING.md
├── Data
├── LICENSE.md
├── README.md
├── SECURITY.md
├── _quarto.yml
├── _site
├── about.qmd
├── demo_base.qmd
├── demo_fancy.qmd
├── dsac-theme.css
├── images
├── index.qmd
├── presentation-styles.css
├── repolinter.json
└── slides.qmd
```

## Coding Style and Linters

```r
lintr::use_lintr(type = "tidyverse")

lintr::lint_dir()

# usethis::use_github_action("lint-project")
```

## Core Team

A list of core team members responsible for the code and documentation in this repository can be found in COMMUNITY.md.

## Policies 
 
### Open Source Policy 
We adhere to the [CMS Open Source Policy](https://github.com/CMSGov/cms-open-source-policy). If you have any questions, just [shoot us an email](mailto:opensource@cms.hhs.gov). 
 
 ### Security and Responsible Disclosure Policy 
*Submit a vulnerability:* Vulnerability reports can be submitted through [Bugcrowd](https://bugcrowd.com/cms-vdp). Reports may be submitted anonymously. If you share contact information, we will acknowledge receipt of your report within 3 business days.
For more information about our Security, Vulnerability, and Responsible Disclosure Policies, see [SECURITY.md](SECURITY.md). 
 
 ## Public Domain 
This project is in the public domain within the United States, and copyright and related rights in the work worldwide are waived through the [CC0 1.0 Universal public domain dedication](https://creativecommons.org/publicdomain/zero/1.0/) as indicated in [LICENSE](LICENSE).
All contributions to this project will be released under the CC0 dedication. By submitting a pull request or issue, you are agreeing to comply with this waiver of copyright interest.
 
 ### Software Bill of Materials (SBOM) 
A Software Bill of Materials (SBOM) is a formal record containing the details and supply chain relationships of various components used in building software.
In the spirit of [Executive Order 14028 - Improving the Nation's Cyber Security](https://www.gsa.gov/technology/it-contract-vehicles-and-purchasing-programs/information-technology-category/it-security/executive-order-14028), a SBOM for this repository is provided here: https://github.com/{repo_org}/{repo_name}/network/dependencies.
For more information and resources about SBOMs, visit: https://www.cisa.gov/sbom.

## Contributing

Thank you for considering contributing to an Open Source project of the US Government! For more information about our contribution guidelines, see CONTRIBUTING.md.