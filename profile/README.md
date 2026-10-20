# Terragrids

We build open tools that measure heat exposure where health data is recorded.

## The terragrids library

[`terragrids`](https://github.com/terragrids/terragrids) is our open Python library,
under the Apache License 2.0. It computes established heat-stress measures, the heat
index, the Universal Thermal Climate Index (UTCI) and the wet-bulb globe temperature
(WBGT), from ERA5. ERA5 is the European Centre for Medium-Range Weather Forecasts'
reconstruction of past weather, hour by hour.

### In development: from the grid to the areas

ERA5 comes as a grid of cells about 25 km across. Health data, such as weekly deaths
or emergency visits, is recorded per administrative area instead: a region, a county,
a city. To compare the two, the heat in each cell has to become one value per area.

A plain average over an area's cells would count an empty mountainside as much as a
city. So the library will weight each cell by how many people live in it, taken from
the population grid of the Global Human Settlement Layer (GHS-POP), which the European
Commission's Joint Research Centre publishes. A cell where nobody lives counts for
nothing.

For example, take an area that covers two cells: a city at 36 °C, where 900,000
people live, and countryside at 30 °C, where 100,000 people live. The plain average is
33 °C. The population-weighted value is 35.4 °C, the heat that nine in ten of the
area's residents were in.

It will work with any boundaries you supply. We will also publish the results for
Europe as an open dataset: the three measures for every day and every NUTS-3 region.
NUTS-3 regions are the statistical areas Eurostat uses, each with roughly 150,000 to
800,000 people.

## Contact

Questions and problem reports are welcome as issues on the library's repository. We
don't take pull requests yet, so please describe a change in an issue instead. You can
also write to terragrids@terragrids.com, or visit [terragrids.com](https://terragrids.com).
