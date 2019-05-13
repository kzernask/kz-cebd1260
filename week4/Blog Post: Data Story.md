# What I learned from [Museum Reviews Collected from TripAdvisor](https://www.kaggle.com/annecool37/museum-data)

Have you ever found yourself wondering where to go when you’re on vacation, or what to do on a weekend with some spare time? Chances are you’re not alone. When thinking about going to museums, people often turn to TripAdvisor for ideas and recommendations based on what’s generally popular. But how do you know which ones will be the best for *you*? And what if you have kids??

To better understand this problem, I started analysing a collection of museum data scraped from TripAdvisor.

### Who goes to museums, anyways?

Naturally, the first question I set out to answer was what the demographic of museum-goers looked like overall. What I found was that **most people tend to visit museums as a couple (38%) or with their families (30%)**.

<p align="center">
   <img src="https://github.com/kzernask/kz-cebd1260/blob/master/week4/images/traveler_types.png">
</p>

### Are different types of museums better suited to different types of travelers?

While it was interesting to know the overall demographic, I next started wondering, did these numbers vary between different types of museums? (Spoiler alert: they do!) Here is a summary of the breakdown of museum-goers across the top museum categories:

![alt text](https://github.com/kzernask/kz-cebd1260/blob/master/week4/images/traveler_types_by_category.png)

Looking at the breakdowns per museum type, families and couples still made up the majority of museum-goers in all cases, but there was a noticeable variation between these two categories. It appeared as though in many cases, **museums are either popular for couples or families** (exceptions being military museums and parks). The data shows **families prefer children’s museums, science, and natural history museums, whereas couples prefer history and art museums, and landmarks**.

This got me thinking – were these distributions consistent across museums in each category? So, I computed the correlations between the percentages of traveler types and museum categories. The strongest relationships are shown below:

![alt text](https://github.com/kzernask/kz-cebd1260/blob/master/week4/images/correlation_categories_travelers.png)

As could be expected, there was a relatively strong correlation between families and children’s museums, and weaker correlations with science and natural history museums. Interestingly enough, the data also showed a correlation between business travelers and factory tours, and a weak correlation between couples and history museums. The most surprising outcome however was that **in general, museums preferences for families are opposite those of all other traveler types**.

### Do different attributes attract different traveler types?

Based on this insight, I started to wonder whether there were certain attributes that made museums more attractive to families versus other types of travelers. I thus computed the correlations between traveler types and tags, with the following results:

![alt text](https://github.com/kzernask/kz-cebd1260/blob/master/week4/images/correlation_tags_travelers.png)

Similar to museum categories, the data showed that **attribute preferences for families are opposite those of other travelers**!!

### Ok, so families go to different places than everyone else - now what?

Given the apparent distinction between families and other travelers regarding both museum types and attributes, there may be an opportunity to develop a family-centric recommendation system for museum selection. The next steps are to further understand and characterize the key factors (and combinations thereof) that make a museum family-friendly.


### Final Thoughts

In general, if you're looking for a museum to visit with your family, looks for museums for all ages, or with features such as interactive exhibits. If you're going as a couple, stay away from these, and check out an art or history museum. Regardless of your choice however, you will probably learn something!
