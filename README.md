# Hierarchical Outcomes

I was piqued by the idea of modeling multiple outcome variables as nested within individuals by [this Gelman blog post](http://andrewgelman.com/2016/03/20/my-quick-answer-is-that-i-would-analyze-all-10-outcomes-using-a-multilevel-model/). This kind of model is not doable in lme4, so here we go. Let's do it in Stan.

I've found [this article](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4119868/#SD3), [this gist](https://gist.github.com/khakieconomics/9dd785c241a1ee0b6f32), and [this reference page](http://stats.idre.ucla.edu/r/faq/multivariate-random-coefficient-model/) on the topic.
