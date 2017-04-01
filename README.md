# Hierarchical Outcomes

I was piqued by the idea of modeling multiple outcome variables as nested within individuals by [this Gelman blog post](http://andrewgelman.com/2016/03/20/my-quick-answer-is-that-i-would-analyze-all-10-outcomes-using-a-multilevel-model/). This kind of model is not doable in lme4, so here we go. Let's do it in Stan.

I've found [this article](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4119868/#SD3), [this gist](https://gist.github.com/khakieconomics/9dd785c241a1ee0b6f32), and [this reference page](http://stats.idre.ucla.edu/r/faq/multivariate-random-coefficient-model/) on the topic.

> Examples of multivariate hypotheses include testing whether outcomes have different average rates of change (Kaysen et al., 2011) or whether change in one outcome is related to change in another (Suvak, Walling, Iverson, Taft, & Resick, 2009).

We can test whether one outcome was more affected than another.

> McDonagh et al. (2005) randomized participants meeting criteria for posttraumatic stress disorder (PTSD) to cognitive-behavioral therapy (CBT), present centered therapy (PCT), and wait-list (WL). In the analysis, the authors examined treatment effects across each outcome (using the group×time interaction in a repeated measures ANOVA and post-hoc tests). The authors found a statistically significant intervention effect for PTSD symptoms but not for depression. The authors interpret the statistical significance for one outcome but not the other as important: “The fact that this treatment [PCT] had more of an impact on PTSD symptoms than on depressive symptoms suggests its mechanism is not simply an antidepressant effect such as has already been demonstrated for problem-solving therapy” (p. 522).
>
> However, comparisons of intervention effects require a statistical test of the difference (cf. Nieuwenhuis, Forstmann, & Wagenmakers, 2011). In other words, we need an explicit test of whether the size of the intervention effect depends upon the outcome type—we need to test the intervention effect by outcome interaction.
