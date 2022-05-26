# KCNA

### Korean Central News Agency
The Korean Central News Agency is the state news agency of North Korea. The agency portrays the views of the North Korean government for both domestic and foreign consumption. It was established on December 5, 1946 and now features internet coverage.

> Owner: Democratic People's Republic of Korea  

> Founded: December 5, 1946  

> Headquarters location: Pyongyang, North Korea  

```{r eval=FALSE}
dim(iris)
```

---
title: "Line graph"
output: html_document
runtime: shiny
---

Choose a time series:
```{r echo = FALSE}
selectInput("data", "",
 c("co2", "lh"))
```
See a plot:
```{r echo = FALSE}
renderPlot({
 d <- get(input$data)
 plot(d)
})
```
