---
title: 'PRAC2'
author: "Autor: Luis Leandro Jiménez y Edna Espejos"
date: "Diciembre 2020"
output:
  html_document:
    highlight: default
    number_sections: yes
    theme: cosmo
    toc: yes
    toc_depth: 2
    includes:
      in_header: 75.584-PEC-header.html
  word_document: default
  pdf_document:
    highlight: zenburn
    toc: yes
---

```{r setup, include=FALSE}
knitr::opts_chunk$set(echo = TRUE)
```



```{r echo=TRUE, message=FALSE, warning=FALSE}
# Cargamos los paquetes R que vamos a usar
library(ggplot2)
library(dplyr)

# Cargamos el fichero de datos
totalData <- read.csv('winequality-red.csv',stringsAsFactors = FALSE)
filas=dim(totalData)[1]

# Verificamos la estructura del conjunto de datos
summary(totalData)
```
