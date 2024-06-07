## Abstract

We present an example to demonstrates inheritance of math macros and other project information from a separate file. This functionality is presented through MyST (https://mystmd.org) and provides the ability to share configuration between projects. This can be used for authors, affiliations site config, etc. In this example, we are interested in reuse of math macros, which in many domains define the way that you can refer to equations and concepts in the literature.

## Example

In the example below we are writing content that references math macros that are from a shared configuration, which could be part of a shared or curated repository.

> The residual is the predicted data for the model, $\dpred{m}$, minus the observed data, $\dobs$. You can also calculate the predicted data for the reference model $\dpred{\mref}$.

The macros are quite commonly used in Geophysics, and could be shared between one or more teams.

## How it works

:::{literalinclude} myst.yml
:start-line: 1
:end-line: 3
:linenos:
:::

:::{literalinclude} math-macros.yml
:::

## Acknowledgements

The work was completed by Franklin and Rowan in MyST in June 2024. Funding was provided by John's Hopkins Open Source Program Office Grant awarded to Alan Lujan.
Chris Carroll provided many LaTeX macros and examples for inspiration.
