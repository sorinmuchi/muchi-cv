# Muchi CV
Sorin Muchi's personal resume, built in LaTeX.

Based on the McDowell CV Template [http://www.careercup.com/resume]. 

## Class Options
 - `calibri` - sets calibri as the main font. Otherwise the default font is Times New Roman since version 1.1.0.

## Commands
The class features the following commands:
 - `\name{name}` - defines the applicant's name to be printed by `\printheader`.
 - `\address{address}` - defines the applicant's address to be printed by `\printheader`.
 - `\contacts{contacts}` - defines the applicant's contacts to be printed by `\printheader`.
 - `\makecvheader` - prints the CV header consisting of the name (see the `\name` command), address (see the `\address` command) and contacts (see the `\contacts` command).
 
## Environments
 - `\begin{cvsection}{sectionname}` - prints a section with a header consisting of the name in bold small caps and a page-wide horizontal line below.
 - `\begin{cvsubsection}[linesnum]{left}{center}{right}{content}` - prints a subsection with header consisting of the `left`, `center` and `right` titles. The optional `linesnum` argument defines the amount of lines in the header. The argument only affects the vertical spacing between the environment header and content thus eliminating the effect of *tabu* package vertical spacing bug.

## Build Command
- `lualatex Muchi_CV.tex`
