# AdSquare Data Analysis Exercise

The code for each section of the assignment has its own notebook in the ‘notebooks’ folder, any data/visualisations produced via the code can be found in the ‘results’ folder. 

For instructions, findings and thoughts on each section, please see below…

1) Analyze the store visitation by date and affinity profile of store visitors.
- Code: 01_analyse_data.ipynb
- Results: final_full_grouped.csv
- Notes: Looping through the CSV file ‘chunks’ proved to be computationally rather time consuming (especially with the full dataset), this is probably down to the ‘apply’ function. Parts of this section could have almost definitely been done in SQL, but I felt comfier using Python.
- Future improvements: Improve code so that looping through CSV file ‘chunks’ is quicker, create function to deal with looping of CSV file ‘chunks’.

2) Visualize store visits
- Code: 02_visualise_store_visits.ipynb
- Results: unique_store_visits_per_day.png
- Notes: Unsurprisingly, the results show a clear slump in GPS locations flagged as within stores on Sundays. There is an anomaly, but an expected one, as there is also a slump on New Year's Day.
- Future improvements: Improve presentation of bar plot (e.g. different colour bars for each day of the week), look at unique store visits per day by store/brand, analyse the affinity groups of people visiting these stores.

3) Visualize GPS data
- Code: 03_visualise_gps_data.ipynb
- Results: gps_locations_matplotlib.png  & [Tableau]( https://public.tableau.com/profile/paul.musco#!/vizhome/adsquare_sample_gps_flags/AdSquareassignment-GPSLocations)
- Notes: Initially I visualised the GPS data using Matplotlib, but due to the granularity of the data, I decided to also use Tableau. Moving to Matplotlib confirmed my suspicions that the GPS locations were all in/around Berlin.
- Future improvements: Include ALL GPS locations, not just those flagged as within a store. 

4) Visualize stores
- Code: 04_visualise_stores.ipynb
- Results: store_locations_matplotlib.png & [Tableau]( https://public.tableau.com/profile/paul.musco#!/vizhome/adsquare_store_locations/AdSquareassignment-StoreLocations) 
- Notes: Similarly to section 3, at first I visualised the GPS data using Matplotlib, but due to the granularity of the data, I decided to also use Tableau.
- Future improvements: 