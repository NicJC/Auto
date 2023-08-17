# Auto
Auto mpg

The data is gotten from UCI Machine Learning Repository

Quinlan,R.. (1993). Auto MPG. UCI Machine Learning Repository. https://doi.org/10.24432/C5859H.

@misc{misc_auto_mpg_9,
  author       = {Quinlan,R.},
  title        = {{Auto MPG}},
  year         = {1993},
  howpublished = {UCI Machine Learning Repository},
  note         = {{DOI}: https://doi.org/10.24432/C5859H}
}

data available here:

[data](https://raw.githubusercontent.com/NicJC/Auto/main/autoMPG.csv)

---

    library(GGally)
    ggpairs(autoMPG[,c(1,6,7)],
        mapping = ggplot2::aes(color = model_year),
        upper = list(continuous = wrap("density", alpha = 0.5), combo = "box_no_facet"))+ggplot2::labs(title = "AutoMPG")  + 
     theme(axis.text.x = element_text(color="steelblue", 
                                   size=12, angle=90),
        axis.text.y = element_text( color="steelblue", 
                                    size=12))
---                                    

![](https://github.com/NicJC/Auto/blob/main/matrixPlot.png)
