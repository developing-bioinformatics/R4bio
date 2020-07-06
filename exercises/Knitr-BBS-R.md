---
layout: exercise
topic: Knitr
title: Reproducible Breeding Bird Survey Analysis
language: R
---

You are interested in understanding how the biodiversity of birds varies in
response to environmental variables and decide to conduct your analysis in a
reproducible manner using `knitr` and `rmarkdown`. Specifically you want to know
how species richness (the number of species seen at a site) varies in response
to the mean annual temperature and the mean annaual precipitation.

1. Start a new `Rmd` document with a title and author and set the output format
   to `html_document`.
2. Add a markdown chunk that describes the question you are going to ask.
3. Add a code chunk that loads the required packages. Hide the output from
   loading packages using `message = FALSE`.
4. Add a header related to downloading and importing the data.
5. Add a text section briefly describing the two datasets you are going to use.
6. Download and unzip the routes data from the Breeding Bird Survey from the FTP site: [ftp://ftpext.usgs.gov/pub/er/md/laurel/BBS/DataFiles/routes.zip](ftp://ftpext.usgs.gov/pub/er/md/laurel/BBS/DataFiles/routes.zip)

```
download.file('ftp://ftpext.usgs.gov/pub/er/md/laurel/BBS/DataFiles/routes.zip', 'routes.zip')
unzip('routes.zip')
routes = read.csv('routes.csv')
```

7. Add a code chunk to load the routes tables into R and display the top few rows. 
8. Make a map of the locations of all of the Breeding Bird Survey routes,
   including an outline the North America landmass. Add a header above this map
   describing what it shows. You can get a world map useing
   `usmap = map_data("world")`, which you can then plot using `geom_polygon`.
   To only show this data in the region of the Breeding Bird Survey routes add
   the following to you `ggplot` command:

   ```
   scale_x_continuous(limits = c(min(routes$longitude), max(routes$longitude))) +
   scale_y_continuous(limits = c(min(routes$latitude), max(routes$latitude)))
   ```

9. Write a brief figure legend about what the map figure shows.
10. Return to the data section of your document and add citations for the
    dataset. You will need to create a `.bib` file to hold your bibtex
    citations. You can obtain bibtex for the citations by searching Google
    Scholar for "Breeding Bird Survey", clicking on the `"`
    icon, and selecting `bibtex`. You should also add a `References` header at
    the bottom of your document since the references will appear at the end.
