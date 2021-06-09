---
layout: post
title:  "HarvardX Learning: R Basics"
categories: Data_Analysis
---

<div class="message">
  Got RStudio set up and learned about data types and vectors in R. Then learned the basics of indexing, data wrangling, and plotting. Skimmed over the programming basics section.  
</div>

This portion was pretty simple as expected for an introduction. I'll post some snippets in each post to help me recap anything I think I might forget about.

{% highlight r %}
#installing packages
install.packages("name")
library(x)

library(dslabs) #contains datasets that can be used to practice
library(dplyr) #part of Tidyverse, contains functions for data manipulation

#returns indices that are True
which(x)

#tells whether each element in vector x is in vector y
y %in% x
{% endhighlight %}

There was also a section on programming basics. Luckily, I already learned the basics of some other languages so I was able to skim over this section. Though there were still some differences I'll have to keep in mind.

{% highlight r %}
ifelse(cond, a, b) #if true, do a, else do b
result <- ifelse(cond, a, b) #can be applied over an entire vector

any(x) #returns true if any in x are true
all(x) #returns true if all in x are true

a_function <- function(x) {
  #operations on x
  #VALUE
}
#there is no 'return' at the end, the last value is what gets returned
{% endhighlight %}

The professor also mentions that while for loops exist in R, it is typically not used. The apply, sapply, tapply, and mapply functions (apply family) are used instead. Some other widely used functions mentioned are split, cut quantile, reduce, identical, and unique. These aren't covered in the course so I will have to look these functions up.