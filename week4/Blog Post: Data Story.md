# What I learned from [Museum Reviews Collected from TripAdvisor](https://www.kaggle.com/annecool37/museum-data)

Have you ever found yourself wondering where to go when you’re on vacation, or what to do on a weekend with some spare time? Chances are you’re not alone. When thinking about going to museums, people often turn to TripAdvisor for ideas and recommendations based on what’s generally popular. But how do you know which ones will be the best for you?
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
