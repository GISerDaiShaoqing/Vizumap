
<!-- README.md is generated from README.Rmd. Please edit that file -->

# Vizumap <img src='man/figures/Vizumap_Hex.png' align="right" height="138.5" />

## An R package for visualizing uncertainty in spatial data.

## Installation

You can install a development version of the Vizumap package from
[GitHub](https://github.com/lydialucchesi/Vizumap)

    # install.packages("devtools")
    devtools::install_github(repo = "lydialucchesi/Vizumap", build_vignettes = TRUE, force = TRUE)

## Authors

Lydia Lucchesi, Australian National University & CSIRO Data61, Email:
<Lydia.Lucchesi@anu.edu.au>

Petra Kuhnert, CSIRO Data61, Email: <Petra.Kuhnert@data61.csiro.au>

## About the Package

Approaches for visualizing uncertainty in spatial data are presented in
this package. These include the three approaches developed in [Lucchesi
and Wikle
(2017)](http://faculty.missouri.edu/~wiklec/LucchesiWikle2017Stat) and a
fourth approach presented in [Kuhnert et
al. (2018)](https://publications.csiro.au/publications/#publication/PIcsiro:EP168206).

### Bivariate Maps

In these bivariate choropleth maps, two colour schemes, one representing
the estimates and another representing the margins of error, are blended
so that an estimate and its error can be conveyed on a map using a
single colour.

### Map Pixelation

In this novel approach, each map region is pixelated, and then each
pixel is filled with a colour from the gradient that falls within the
estimate’s margin of error. Regions that appear visually as a solid
colour reflect smaller margins of error, while more pixelated regions
indicate greater uncertainty. These maps can be animated using
visuanimation techniques to provide a novel uncertainty visualisation
experience.

### Glyph Rotation

In this method, glyphs located at region centroids are rotated to
represent uncertainty. The colour filling each glyph corresponds to the
estimate.

### Exceedance Probability Maps

The final map-based exploration is through exceedance probabilities,
which are visualised on a map to highlight regions that exhibit varying
levels of departure from a threshold of concern or target.

## Examples

A vignette for the Vizumap package is available and contains examples
relating to each of the visualization methods.

    vignette("Vizumap")

## How to Reference

Vizumap: An R package for visualizing uncertainty in spatial data, DOI:
10.5281/zenodo.1013930,
<https://zenodo.org/record/1479951#.Xnr_Qy1L2L8>.

## License

Vizumap version 1.1.0 is licensed under GPLv3.

## References

<strong>Kuhnert, P.M.</strong>, Pagendam, D.E., Bartley, R., Gladish,
D.W., Lewis, S.E. and Bainbridge, Z.T. (2018) Making management
decisions in face of uncertainty: a case study using the Burdekin
catchment in the Great Barrier Reef, Marine and Freshwater Research, 69,
1187-1200, <https://doi.org/10.1071/MF17237>.

<strong>Lucchesi, L.R.</strong> and Wikle C.K. (2017) Visualizing
uncertainty in areal data with bivariate choropleth maps, map pixelation
and glyph rotation, Stat, <https://doi.org/10.1002/sta4.150>.
