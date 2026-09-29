# Synthetic Sales Analysis

**AI Assistance Declaration:** I used ChatGPT (GPT-5.6 Sol) for
documentation structure, Markdown drafting, wording refinement, and
formatting suggestions. Prompts used are listed in `Appendix_AI.md`. I
verified the written structure and Markdown syntax by review; the
required RStudio/Posit Cloud knit/preview and GitHub preview must be
completed before submission. All final calculations are done by myself.
No real or personal data were uploaded. I am responsible for the
accuracy and originality of this work.

## Overview

This small R project demonstrates a clear documentation workflow for a
simple analysis using a synthetic sales dataset. The project shows how
an R analysis can be documented with a professional README and an R
Markdown file.

The workflow creates synthetic monthly sales data, inspects its
structure, summarizes the revenue variable, and creates a simple
visualization. The emphasis of this assignment is documentation quality
rather than complex analysis.

## Project Structure

``` text
markdown-buddy-ali-beheshtinejad/
├── README.md
├── script_documentation.Rmd
├── Reflection.md
└── Appendix_AI.md
```

## Dependencies

-   R
-   RStudio or Posit Cloud
-   `ggplot2` for visualization

## Installation

1.  Install R and RStudio, or open a Posit Cloud project.
2.  Open the project folder.
3.  Add the four files shown above.
4.  If needed, install `ggplot2`:

``` r
install.packages("ggplot2")
```

## Example Code

``` r
library(ggplot2)

sales <- data.frame(
  month = c("Jan", "Feb", "Mar", "Apr", "May", "Jun"),
  revenue = c(12000, 13500, 12800, 15100, 16000, 17200)
)

summary(sales$revenue)

ggplot(sales, aes(x = month, y = revenue)) +
  geom_col() +
  labs(
    title = "Synthetic Monthly Revenue",
    x = "Month",
    y = "Revenue"
  )
```

## Expected Output

-   A small synthetic dataset stored in R.
-   Summary statistics for the `revenue` variable.
-   A bar chart showing synthetic monthly revenue.

## Documentation and Validation

The README uses common GitHub documentation sections such as Overview,
Installation, Example Code, and License. Markdown headers, lists, fenced
code blocks, and inline code formatting have been checked for
consistency.

Before final submission:

1.  Preview `README.md` on GitHub.
2.  Knit or preview `script_documentation.Rmd` in RStudio or Posit
    Cloud.
3.  Confirm that headings, lists, code blocks, and the chart render
    correctly.
4.  Compare the README structure with a real R repository, such as a
    tidyverse repository.
5.  Make any final corrections identified during preview.

## License

This project was created for BDA400 coursework and is intended for
educational use.

## AI Assistance Disclosure

-   **AI tool used:** ChatGPT (GPT-5.6 Sol)
-   **Date used:** September 22--28, 2026
-   **Main prompts:** The assignment seed, refinement, and critique
    prompts, plus requests to organize and finalize the documentation.
-   **Changes after review:** The draft was simplified, headings were
    standardized, the repository was limited to the required
    deliverables, and verification steps were made explicit.
-   **Validation:** Written content and Markdown structure were
    reviewed. The required RStudio/Posit Cloud knit/preview and GitHub
    preview must still be completed before submission.
