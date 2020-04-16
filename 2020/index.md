---
layout: default
title:  "2020 Report"
date:   2020-04-10 00:00:00 -0500
---
# Report (2020)

In 2018 I stumbled upon the Toronto Police Service's published datasets and as an avid cyclist in the city I was naturally curious about the bicycle thefts that happen in the city. I dug through the data (that can be found [here](https://data.torontopolice.on.ca/datasets/bicycle-thefts)) and I wrote a [report on my findings back then.](/TorontoBicycleCrimes/2018)

It's been two years since I last looked at the data and after someone from CycleTO reached out, I thought this would be a great time to make an updated report with data from 2018 and 2019.

Note: the data presented only reflects **reported** crimes, which may not reflect actual bicycle-related crime in the city

## Neighbourhoods
Each crime is listed with the neighbourhood of where the crime occurred! Waterfront Communities - The Island comes in first place with **2271 reported incidents** over 6 years and Maple Leaf comes in last with only **5**. In the 2018 report Waterfront Communities - The Island had less than 1400 crimes and Maple Leaf had 7 (somehow this value decreased by 2)

Below is a plot of number of crimes by neighbourhood -- **_double click to zoom out and drag your mouse to zoom in on a window_**

{% include_relative plots/neighbourhoods.html %}

In the two years since I last looked at the data, it seems **the worst 10 neighbourhoods have not changed** except for their order. Notably: Niagara went from 9th worst to 4th worst and Bay Street Corridor overtook Church-Yonge corridor for 2nd.

Couldn't find the neighbourhood you were interested? [A full list of neighbourhoods can be found here.](tables/full_neighbourhood_list.html)

## Maps
Below is a heatmap of the reported crimes, by neighbourhood
{% include_relative plots/heatmap.html %}

Looking to see if your stolen bicycle was properly reported? Here is a scatter plot of all reported crimes
{% include_relative plots/scatter.html %}

If you guess that your bicycle is safer at home rather than locked on the street somewhere -- you're wrong (if you live in an apartment or condo). **21.2% of all bicycle thefts occur in apartments (and condos) vs. 21% which occur on streets**. Of course, not all thefts are occuring in your apartment/condo unit, it's likely that these thefts are happening in bicycle rooms or racks on premises. **This proportion has increased since the 2018 report where only 17.7% of thefts happened in apartments/condos and 22.7% occured on the street.**

{% include_relative plots/location_type.html %}

## Time Data

The number of thefts that occur per year has increased steadily year by year up until 2019, this could be because: 

1. bicycle thefts have gone down (🎉), 
2. people are reporting fewer thefts, or 
3. not all data has been entered for 2019. 

Either way, these are troubling figures because this means there are **greater than 10 thefts per day on average, every year**
{% include_relative plots/yearly_thefts.html %}

Do you know when your bicycle is most likely to be stolen? You might think your bicycle is less safe locked during the night but that *is not necessarily* be true. 

The plot below shows that there are way more thefts during the day than overnight, however because the data only shows **reported** crimes, this data is skewed to be biased towards daytime crimes. 

There are peaks at around 9 AM, 12 PM and 6 PM (corresponding to morning commute, lunch, and evening commute), this is likely because those are the times when people are most likely to *notice* that their bike has gone missing, again emphasizing the fact that this is only reported data.
_(This distribution has not changed significantly since 2018)_
{% include_relative plots/hourly_thefts.html %}

Bicycle-related thefts spike during the warmer months and slow down during the winter, which makes sense due to lower ridership. 
The 1-month period with the most reported crimes was July 2018 with 642, or about **20 per day!** (up from the previous peak in July 2017 with 591)
It will be interesting to see if the ongoing (as of writing) coronavirus pandemic will have an affect on 2020 numbers.
{% include_relative plots/monthly_thefts.html %}

## Cost
So how much is this theft costing us? Over six years of data, the reported **cost of stolen bikes sums up to $18,804,580** or roughly $3.13 million per year!
With $3.13 million you can:

1. buy 745,238 Big Macs,
2. pay for the City of Toronto's [New Affordable Housing Development budget (twice)](https://www.toronto.ca/legdocs/mmis/2019/bu/bgrd/backgroundfile-123807.pdf), or
3. get 2 Lysol wipes from Pusateri's

{% include_relative plots/yearly_cost.html %}

The **average value of a stolen bike was calculated to be approximately $937.97**, which seems high (up from $907.95 in 2018). This could either mean there are a lot of “low value” bicycle thefts that aren’t being reported by their owners or people may be over-reporting the value of their bikes in hopes that the police will take it more seriously.

Of the $18 million of stolen bicycles, **$176,686.71 has been recovered**, which is quite disappointing and discouraging to find out. 

Below is histogram showing the cost of stolen bicycles throughout Toronto, separated in $100 buckets:


{% include_relative plots/price_histogram.html %}
_double click to zoom out and drag your mouse to zoom in on a window_

## Prevention and Recovery
Now here's the part where I nag at you: 

Do you know what your bicycle's serial number is? Or where to find it? Knowing the serial number to your bicycle is essential to recovering it if it gets stolen. **Between 2014 and 2019 there were approximately 20,000 reported bicycle crimes and only 1.17% of stolen bicycles were able to be recovered** (this has decreased by 0.1% since 2018). Your chances of recovering your stolen bike are very, very slim so don't rely on it!

{% include_relative plots/status.html %}

If you want to have a chance of getting your bike back after it's stolen, please register your bike with the Toronto Police [here](https://www.torontopolice.on.ca/bike/). Your serial number can typically be found on the bottom of your bike, under the [bottom bracket shell](https://www.google.ca/search?q=bottom+bracket+shell). Hopefully Toronto might get something like [Project 529](https://project529.com/garage) where victims can post an alert to fellow cyclists to look out for stolen bikes.

To secure your bike better, consider getting a U-Lock, they are way sturdier than cable locks and are worth it keep your bike safe. Sheldon Brown has a great [webpage on lock-strategy](https://www.sheldonbrown.com/lock-strategy.html). GCN has a [very good video as well](https://www.youtube.com/watch?v=IXNASUSivqg).