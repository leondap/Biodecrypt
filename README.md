# Biodecrypt
A set of R functions comparing concave distribution hulls to objectively attribute uncertain occurrence data to two or more cryptic entities



Occurrence records are fundamental to macroecology, mostly in species distribution modelling. Collecting distribution requires an enormous effort, and existing databases have been assembled over decades. Nevertheless, this data suddenly become obsolete with the frequent discovery of cryptic taxa and/or Evolutionary Significant Units (ESU). In most cases, researchers amalgamate the occurrence data, but this ignores a substantial fraction of diversity in terms of identity, distribution, evolution, and ecology. Using aggregate data could lead to inaccuracy in assessing climatic preferences and in predicting the response to climatic changes since  cryptic taxa show significantly diverging climatic niches in the same order of magnitude as the differences among other congeneric species (Platania et al. 2020). Since most cryptic taxa/ESU have parapatric distributions, we implemented a set of R functions (biodecrypt) comparing concave distribution hulls to: 1) Objectively attribute occurrence data previously referring to a single taxon to two or more newly recognized entities, based on a subset of ascertained records.  2) Test the reliability of the attribution by cross-validation. 3) Optimize the parameters used in the algorithm. 


The biodrcrypt functioning is explained in details in Platania et al (2020) but it can be briefly summarised as follows:

The main inputs for the functions are a matrix with longitude and latitude for all the occurrence data and a vector (in the same order) providing their identification. The records identified to species-level (identified records) must be indicated in the vector with a sequential numeric value (1, 2... n), which represents the verified membership to the nth species. The occurrence data with unknown identification (unidentified records) are marked with a 0.



Platania, L., Menchetti, M., Dincă, V., Corbella, C., Kay‐Lavelle, I., Vila, R., ... & Dapporto, L. (2020). Assigning occurrence data to cryptic taxa improves climatic niche assessments: Biodecrypt, a new tool tested on European butterflies. Global Ecology and Biogeography, 29(10), 1852-1865.
