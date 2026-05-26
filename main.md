# User guide for this template

[DO NOT submit papers containing LaTeX error
messages.]{style="color: red"} If you see any error messages, please fix
them before submission. Please read the following guidelines carefully.

The copy editor is Junzi alone for the moment; any time saved for him is
time saved for you :).

## Title

The title should be in Title Case. Keep it concise and informative,
ideally within 12 words. Avoid abbreviations in the title unless they
are widely recognized.

## Single main file

[DO NOT use external .tex files]{style="color: red"}, like `\input{}` or
`\include{}`. Place all content in `main.tex`.

## Keep the original file names

[DO NOT rename filenames]{style="color: red"} including `main.tex`, the
`figures` folder, or `reference.bib`, to ensure compatibility with the
automated copyediting process.

## References

Add your bibliography entries to `reference.bib` and cite them using
`\cite{}`. Here is an example citation on diamond open access
[@fuchs2013diamond]. Since many of you are using the OpenSky data, here
is another example [@schafer2014bringing].

## Footnotes

Use footnotes sparingly. They should be used for additional information
that is not essential to the main text. Use the `\footnote{}` command to
create footnotes.[^1]

## Tables

Use the standard `tabular` environment. [Avoid custom or complex table
designs]{style="color: red"} to ensure compatibility for the web
version. Table [1](#tb:example_table){reference-type="ref"
reference="tb:example_table"} shows an example that always works.

::: {#tb:example_table}
  **Parameter**   **Notation**   **Remarks**
  --------------- -------------- --------------------------
  name            \-             engine common identifier
  manufacture     \-             name of the manufacturer
  bpr             $\lambda$      bypass ratio
  pr              \-             pressure ratio
  thrust          $T_0$          maximum static thrust

  : Example table
:::

## Figures

Store all figures in the **figures** folder. Use concise, space-free,
and lowercase filenames.

Ensure that the figure is in a compatible format (.png or .pdf) and is
appropriately sized (not too large or too small).
Figure [1](#fig:example){reference-type="ref" reference="fig:example"}
shows an example of how to include a figure.

![An Example Figure](example-image){#fig:example width="40%"}

If you need subfigures, [DO NOT use the `subfloat`
package]{style="color: red"}. You are recommended to use the `subfigure`
package instead. Figure [2](#fig:subfig_example){reference-type="ref"
reference="fig:subfig_example"} shows an example of how to use
subfigures.

<figure id="fig:subfig_example">

<figcaption>An Example of subfigures</figcaption>
</figure>

Attention: in your text, use `Figure \ref{fig:example}`, NOT
`Fig. \ref{fig:example}`.

## Equations

Use the `equation` environment for numbered equations. You must avoid
customized variable names. Otherwise, the HTML version will not be
generated properly.

For example, Equation
[\[eq:cauchy_momentum\]](#eq:cauchy_momentum){reference-type="ref"
reference="eq:cauchy_momentum"} shows an example equation.

$$\label{eq:cauchy_momentum}
\rho\frac{\mathrm{D} \mathbf{u}}{\mathrm{D} t} = - \nabla p + \nabla \cdot \boldsymbol \tau + \rho\,\mathbf{g}$$

## Abbreviations

Use the `\abbreviations{}` command to define abbreviations. Only use
abbreviations if the term is used more than ten times throughout the
paper. Otherwise, write them in full.

# Sections

Organize your paper using standard sectioning commands (`\section`,
`\subsection`, etc.).

Some standard sections are:

-   Introduction

-   Methods

-   Results

-   Discussion

-   Conclusion

You can add or remove sections as needed.

Use `Appendix` for supplementary material. The appendix should be used
for additional information that is not essential to the main text but
may be useful for some readers. Remove this section if you do not have
any supplementary material.

# Supplementary figures

# Supplementary tables

# Acknowledgement {#acknowledgement .unnumbered}

Include your acknowledgements in this section.

# Author contributions {#author-contributions .unnumbered}

If the paper has more than one author, the CRediT section must be
included. See example usage at <https://casrai.org/credit/>

-   First Author: Conceptualization, Data Curation, Formal Analysis,
    Funding Acquisition, Investigation, Methodology, Project
    Administration, Resources, Software, Supervision, Validation,
    Visualization, Writing (Original Draft), Writing (Review and
    Editing)

-   Second Author: Data Curation, Writing - Original Draft

-   Third Author: Visualization, Investigation

# Funding statement {#funding-statement .unnumbered}

When applicable, please specify the funding information for this
research.

# Open data statement {#open-data-statement .unnumbered}

[Mandatory section!]{style="color: red"}

Include DOI and a short description of supplementary data.

# Reproducibility statement {#reproducibility-statement .unnumbered}

[Mandatory section!]{style="color: red"}

Information on how to reproduce this research, including access to: 1)
source code related to the research, 2) source code for the figures, 3)
source code/data for the tables when applicable.

[^1]: This is an example footnote that works.
