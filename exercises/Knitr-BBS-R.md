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
6. Download and place the Breeding Bird Survey data from the course eLearn page
   into the directory where you are saving this Rmarkdown file. Unzip the folder 
   and look for the files: routes.zip (unzip this) --> routes.csv
   
   OR: Add a  code chunk to download the Breeding Bird Survey 
   data using the `rdataretriever` package. Instructions for installing this package 
   and the associated Python package are available on the [Data Retriever website](https://www.data-retriever.org/). It will take a long time to download 
   and convert this data into a set of useable CSV files (~30 minutes), so add 
   a conditional statement that checks to see if the necessary files have already 
   been created and only install they data if they have not. Don't show the output 
   for this chunk.
7. Add a code chunk to load the species, counts, and routes tables into R and
   display the top few rows of each table.
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
