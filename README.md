# Intro to ggplot 2 Lab

In this lab, we're going to use what you learned in our last lessons and try to re-create one of the images from your capstone project with ggplot2.

## Learning Objectives

By the end of the lesson, you will have:

* [ ] Synthesized what you learned in about `dplyr` and `ggplot2` to recreate a data visualization you made with Python, in R! 

## Guidelines

Now since this lab is going to be different for every person, what we have done here is provide a template to help you think through what this process will look like.

Do you best to think to stick to this workflow and make sure to use as many of the resources you can find along the way to help you.

### Resources

* [ggplot2 Chapter in R for Data Science](https://r4ds.had.co.nz/)
* [tidytuesday](https://github.com/rfordatascience/tidytuesday)
* [R for Data Science Online Learning Community](https://www.rfordatasci.com/)
* [gglot2 Flipbook](https://evamaerey.github.io/ggplot_flipbook/ggplot_flipbook_xaringan.html#1) 

## Organizing the Problem

The first thing that you need to do is get your data in a tidy format!
You could import in the data that you might have used with something like `matplotlib` or `seaborn`, but we suggest that since you already know the steps you have taken in Python to clean up the data, you should try to do this again with `dplyr` so that you only need to focus on the new R syntax.

Try to follow this checklist to get going after you've imported your data:

First just look at the differences between the code and the data!

* [ ] Try to find a some `ggplot2` code that already exists for the type of data viz you want to make
* [ ] Compare and contrast the code used for this data viz with the code you wrote for yours
* [ ] Compare and contrast the data used for this data viz with the format your data was in to make your chart

Next just worry about the format of the data and making it match what you used in `pandas` to clean it.
For example, you might want to... 

* [ ] Use `select()` to grab any variables you know you need for the data viz
* [ ] Use `filter()` to get any rows you need
* [ ] String together these commands using as many pipes `%>%` as you need.

```{r}
library(tidyverse)

data <- read_csv("path/to/your/data.csv")

data %>%
  select(your, columns, here) %>%
  filter(your, rows, here) %>%
  filter(maybe, it's, more, complex)
  
```

```{r}
# your r code here! 

```

Once the format of your data using `dplyr` matches that of the data used in the example code you found, it's then time to start ggplotting! 

From here, you can either keep the pipes going and pipe right into `ggplot2` like we did before, or save a new object with the `<-` operator. 
The choice is yours!

The next part is going to be a bit more guess and check based on what you know, but as you do this, think about what you have learned

* [ ] Figure out what data needs to be mapped to what aesthetic
* [ ] Get the data on the ggplot first before adding titles and labels
* [ ] Only once all the data is showing up on the ggplot, then start to add layers like title, legend, and begin to manipulate the axes. 
* [ ] You're probably going to do a lot of stack-overflowing here so you'll feel right at home with Python! 

```{r}
# your code here! 

```

If you get stuck, maybe use this as an opportunity to reach out the the #rstats community.
On Twitter, there are a lot of people tweeting on the `#rstats` hashtag and there's a big community of people learning everything in the tidyverse that you can find tweeting about `#tidytuesday`, a [weekly chance for people of any skill level to make plots using tidyverse principles](https://github.com/rfordatascience/tidytuesday), as well as a whole [R for Data Sciencecommunity](https://www.rfordatasci.com/) set up to help people get familiar with the tidyverse.

Welcome to the world of R!