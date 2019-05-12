# Data Description
### Kaggle Dataset: Museum Reviews Collected from TripAdvisor

## The Data

#### **What’s in it?**
This dataset contains data of >1500 museums scraped from TripAdvisor, for both US and world museums. The data includes general museum information, including: museum name, address, latitude and longitude, rank, number of reviews, average rating, and number of times featured by Trip Advisor. Additional data is provided per museum describing traveler and review information, including: the detailed ratings and traveler types, museum categories, and tag clouds.
Information on fees and typical length of visit are also described in the dataset, but are vastly incomplete and therefore of little value for analysis purposes.
I have also incorporated an additional dataset with continent and subregion information by country, in order to facilitate regional analysis.

##### What can we do with it?
I see several opportunities that exist within this data:
-	Identify factors that result in a higher rating, or increased attendance
  -	Insights from this analysis could be leveraged to provide potential solutions for underperforming museums to increase attendance or exposure
-	Identify regional variances between museums and correlations between attributes (categories, traveler types, attendance, ratings)
  -	Insights from this analysis could be leveraged to design an application for traveler museum selection (with detailed filters, and geolocation mapping), a recommendation system, or a more sophisticated trip planning application

## Some Preliminary Analyses

#### Museums around the world
The first thing I looked at was the distribution of museums around the world. The figure below shows some interesting findings:\

![alt text](https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Logo Title Text 1")

As you can see, **nearly two thirds of the museums are in North America (specifically, the US)**. This was surprising to me – so I looked it up. According to Wikipedia, there are around 55,000 museums in the world, and approximately 33,000 of those are in the US – so the proportions in this data set are actually reasonable. From the data, about one quarter of the museums are located in Europe, about six percent in Asia, and only a handful in Australia/New Zealand and Africa.

#### Top types of museums
Next, I looked at the top types of museums:\

![alt text](https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Logo Title Text 1")

From the data, speciality museums account for about half of all museums, followed by art and history museums, while the rest are split between a variety of types. Although this chart only shows the top 15, **there were actually 83 distinct museum categories** – a much larger variety than expected. This analysis can also be broken down further by region:\

![alt text](https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Logo Title Text 1")

Looking at the data side-by-side below, we can get a better sense of how the top types compare across the world:\

![alt text](https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Logo Title Text 1")

Here, we see that **the types of museums are proportionately similar worldwide**, though differing in scale. However there are a few notable exceptions:
- Clearly, the Americas has proportionately more nature and parks attractions, as well as children's museums.
- Asia has proportionately few natural history museums, but more science museums.
- Oceania (i.e. Australia and New Zealand) has proportionately more natural history museums.

#### Most-rated museums
Finally, let’s take a look at the museums in each region with the highest number of reviews (which I presume reflects the attendance, or popularity):\

![alt text](https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Logo Title Text 1")

It looks like the top museums in Europe are very highly visited compared to those in Australia or Africa.

## Final thoughts
So, based on these data summaries, it seems that **the US or Europe are the places to go for the most museums**, and the collection of top-most-reviewed ones would probably be a good place to start.
