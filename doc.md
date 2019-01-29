---
title: Templating Organization of Scientific Research for Reproducibility at Project Inception
author: 
    name: Griffin Chure
    department: Department of Biology and Biological Engineering
    univ: California Institute of Technology, Pasadena, CA, USA 
    email: gchure@caltech.edu
    orcid: 0000-0002-2216-2057
email: gchure@caltech.edu
geometry: margin=0.75in, footskip=0.85in
fignos-cleveref: true
fignos-plus-name: "Fig."
reference-section-title: References 
bibliography: library.bib
classoption: twocolumn
link-citations: true
monofont: Ubuntu Mono 
sansfont: Cabin Regular
mainfont: Source Sans Pro
header-includes:
    \usepackage{microtype}
    \usepackage{sectsty}
    \usepackage{caption}
    \sectionfont{\sffamily\sffamily}
    \subsectionfont{\sffamily}
    \subsubsectionfont{\normalfont\sffamily\itshape}
    \captionsetup[figure]{name={\bfseries\sffamily\selectfont Fig.}}
    \captionsetup[figure]{labelsep=colon}
abstract:
    blah
---

"There is a reproducibility crisis in science" is a sentence guaranteed to
illicit a strong response from whomever it is inflicted upon. Regardless of
whether such a crisis exists (cite), it is an objective truth that
improvements can be made in how science is performed, presented, and reviewed
such that other scientists, whether a savant or a neophyte, could reproduce
the analysis, generation, and interpretation of your research findings, assuming
they have the means to.

All fields of science are becoming more quantitative and, as a consequence,
relying on computation in the generation, processing, interpretation, and
presentation of data. In my experience, the programs written to perform the
aforementioned tasks are tailor-made to fit that particular problem.
Unfortunately, these bits of code are typically closer to a Frankenstein
creature than a tailor-made suit. Hardcoded numbers, ambiguously named
variables, and absent (or flat-out wrong) documentation are the most common
afflictions found lurking in the code base. While this writing is not meant to
educate on how to write scientific software, merely organizing the codebase by 
separating the *executed* code from the *defined functions*

As of this writing, I am nearing the end of my PhD and find myself reflecting
on what I've learned, and more importantly, what I could
have done better. Over the course of my graduate research, I've had the immense
privilege to be involved in projects so-called "scientific socialism" where first
authorship of our work was split amongst five graduate students
[@Razo-Mejia2018]. It was during this first collaboration (and my very first
scientific paper) that I began to put together what I thought would the "ideal"
layout to keep our data, processing scripts, and statistical analysis. What we
developed was far from ideal, but a good first step. Over the next several
projects, I adapted and tuned this organizational scheme to something that was
much closer to ideal. What follows is a summary of this layout and the rationale
behind it.

# A Field-Agnostic Project Architecture

![A template for reproducible scientific research](figs/project_architecture.pdf)

## Execution of code

**`processing`**

**`analysis`**

**`exploratory`**

**`figures`**

## Storage and organization of (not big) data

## Implementation and validation of home-grown software

## Making the technical human readable

## Making life easy

## Protecting your work and staking your claim

# Discussion

## Separation of human-readable & machine-readable

## Separation of execution and definition of code

## "It Tolls For Thee"

> "Perchance he for whom this bell tolls may be so ill, as that he knows not it tolls for him; and perchance I may think myself so much better than I am, as that they who are about me, and see my state, may have caused it to toll for me, and I know not that.

John Donne

# Acknowledgements
Justin Bois, Rob Phillips, Manuel Razo-Mejia, Shyam Saladi, Zofii Kaczmarek,
Nathan M. Belliveau, Stephanie L. Barnes, (Ask Gail Clement, Tom Morell,
Victoria Stodden, Dave VanValen, Quincey Justman for comment).