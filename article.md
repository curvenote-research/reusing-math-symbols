## Abstract

We present an example to demonstrates inheritance of math macros and other project information from a separate file. This functionality is presented through MyST (https://mystmd.org) and provides the ability to share configuration between projects. This can be used for authors, affiliations site config, etc. In this example, we are interested in reuse of math macros, which in many domains define the way that you can refer to equations and concepts in the literature.

## Example

> The residual is the predicted data for the model, $\dpred{m}$, minus the observed data, $\dobs$. You can also calculate the predicted data for the reference model $\dpred{\mref}$.

## How it works

:::{literalinclude} myst.yml
:start-line: 1
:end-line: 3
:linenos:
:::

:::{literalinclude} math-macros.yml
:::

## Acknowledgements

The work was completed by Franklin and Rowan in MyST and funded by John's Hopkins Open Source Program Office Grant awarded to Alan Lujan.
Chris Carroll provided many LaTeX macros and examples for inspiration.
