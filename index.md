# Report

The Toronto Police Service publishes interesting datasets on their [public safety data portal](http://data.torontopolice.on.ca/) and I found a nice dataset on [bicycle-related crimes](http://data.torontopolice.on.ca/datasets/91af6347ff08458e9fa4e06b2acc4e1d_0) that was recently published and I thought it was interesting enough to write about. I have had a bike stolen in the city and it's a horrible feeling -- maybe this data can help you avoid having your bike stolen too.

Note: the data presented only reflects **reported** crimes, which may not reflect actual bicycle-related crime in the city

## Heat Maps
Think your bike is safe? Check the heat map to see where bike thefts are reported.

Unsurprisingly, the one place where there are no reported bicycle related crimes is the Bridle Path. 
<div class="tab">
  <button id="crime" class="tablinks" onclick="generate_heatmap('crime')">All crimes</button>
  <button id="theft" class="tablinks" onclick="generate_heatmap('theft')">Thefts</button>
  <button id="be" class="tablinks" onclick="generate_heatmap('be')">Breaking & Entering</button>
  <button id="ebike" class="tablinks" onclick="generate_heatmap('ebike')">E-Bike crimes</button>
</div>

<div class="folium-map" id="heatmap" style="width: 100%; height: 400px"></div>
<script type="text/javascript" src="script/heatmaps.js"></script>
<script type="text/javascript">initial_map()</script>

Most thefts seem to occur on large streets and public places, but it doesn't mean your bike is safe on private property. About a third of thefts/crimes happen at houses and apartments/condos. 

![location types](plots/locationtype.png)
<p style="text-align: center;" markdown="1">*[Full list here](tables/full_locationtype.html)*</p>

## Neighbourhoods
Each crime is listed with the neighbourhood of where the crime occurred! Waterfront Communities - The Island comes in first place with almost 1400 reported incidents over 4 years and Pleasant View comes in last with only **5**.

Below the top 10 neighbourhoods for having the most crimes. Click on the tabs to see how things have changed over the years.
<div class="tab">
  <button id="total" class="tablinks active" onclick="change_image(event,'worst_neighbourhoods.png')">Total</button>
  <button id="stack" class="tablinks" onclick="change_image(event,'worst_stack.png')">Stack</button>
  <button id="2017" class="tablinks" onclick="change_image(event,'2017worst.png')">2017</button>
  <button id="2016" class="tablinks" onclick="change_image(event,'2016worst.png')">2016</button>
  <button id="2015" class="tablinks" onclick="change_image(event,'2015worst.png')">2015</button>
  <button id="2014" class="tablinks" onclick="change_image(event,'2014worst.png')">2014</button>
</div>
<img id="worst_neighbourhood" src="plots/worst_neighbourhoods.png" style="width:100%">

The worst 4 neighbourhoods: *Waterfront Communities - The Island, Church-Yonge Corridor, Bay Street Corridor and the Annex* are consistently the worst places to be a bicycle owner. 

Over the four years, the other neighbourhoods in the top 10 move around and swap with each other without any particular trend. 

Rosedale-Moore Park receives the **most improved award** for being in the top 10 in 2014 and 2015 but not being in the top 10 for 2014 - 2017 (although, still 11th overall)! 

South Riverdale gets the *least improved award* for making the top 10 (2014 - 2017) despite only being in the top 10 for 2016 and 2017.

![best neighbourhoods](plots/best_neighbourhoods.png)


## Yearly Data

The data shows that the number of reported bicycle crimes have increased in 2016 and 2017 compared to 2014 and 2015. This could be due to the [increase in ridership levels throughout 2016 and 2017 due to better cycling infrastructure](https://www.cycleto.ca/news/major-increase-torontonians-biking-work-34-some-neighbourhoods). The unfortunate reality is that an increase in cyclists also means an increase in bicycle thefts.

![yearly plot](plots/yearly.png)

Bicycle-related crimes (mostly theft) spike during the warmer months and slow down during the winter, which makes sense due to lower ridership:

![monthly plot](plots/monthyear.png)

## Prevention and Recovery

Do you know what your bicycle's serial number is? Or where to find it? Knowing the serial number to your bicycle is essential to recovering it if it gets stolen. Between 2014 and 2017 there were approximately 14,000 reported bicycle crimes and only around 1.27% of stolen bicycles were able to be recovered.

![recovery stats](plots/recovery.png)

If you want to have a chance of getting your bike back after it's stolen, please register your bike with the Toronto Police [here](https://www.torontopolice.on.ca/bike/). Your serial number can typically be found on the bottom of your bike, under the [bottom bracket shell](https://www.google.ca/search?q=bottom+bracket+shell). Hopefully Toronto might get something like [Project 529](https://project529.com/garage) where victims can post an alert to fellow cyclists to look out for stolen bikes.
