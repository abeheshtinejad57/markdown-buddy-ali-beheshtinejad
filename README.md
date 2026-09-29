# Synthetic Sales Analysis

**AI Assistance Declaration:** I used ChatGPT (GPT-5.6 Sol) for
documentation structure, Markdown drafting, wording refinement, and
formatting suggestions. Prompts used are listed in `Appendix_AI.md`. I
verified outputs by reviewing the Markdown structure, previewing the
README on GitHub, and knitting the R Markdown file in Posit Cloud. All
final calculations are done by myself. No real or personal data were
uploaded. I am responsible for the accuracy and originality of this
work.

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
3.  Add the four assignment files shown above.
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
code blocks, and inline code formatting were reviewed for consistency.

Verification completed: - `README.md` was previewed on GitHub to confirm
that headings, lists, and code blocks render correctly. -
`script_documentation.Rmd` was knitted successfully in Posit Cloud and
its rendered HTML was reviewed. - The documentation structure was
checked against common professional R-project README conventions. - Only
synthetic data are used.

## License

This project was created for BDA400 coursework and is intended for
educational use.

## AI Assistance Disclosure

-   **AI tool used:** ChatGPT (GPT-5.6 Sol)
-   **Dates used:** September 22--28, 2026
-   **Main prompts:** The assignment seed, refinement, and
    critique/validation prompts, plus requests to organize and finalize
    the documentation.
-   **Changes after review:** Headings were standardized, wording was
    simplified, code blocks were formatted consistently, the repository
    was limited to the assignment deliverables, and validation notes
    were updated after previewing.
-   **Validation:** The README was previewed on GitHub and the R
    Markdown document was successfully knitted and reviewed in Posit
    Cloud. The student remains responsible for the final work.
