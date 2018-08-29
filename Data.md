## Data for the project

Now when we have the execution path for our idea, we can start to search the appropriate data sources for each step and gather it all together. 

1. Get the Dataset with Brooklyn's Neighborhoods and their coordinates.
   The file with coordinates of all 5 boroughs of New York and their corresponding neighborhoods is available for free on                    https://geo.nyu.edu/catalog/nyu_2451_34572
   We need to download it, open and transform into data frame.
   After that we clean our data: extract only the neighborhoods of borough Brooklyn and their coordinates. 
   For better overview we can visualise it with help of Folium Libraries.
   
  2. In order to provide the further analysis we will use mainly Foursquare location data with help of following call requests:
  
    - search particular venues in neighborhoods: 
      url='https://api.foursquare.com/v2/venues/aearch?&client_id={}&client_secret={}&v={}&ll={},{},query={}'
    
    - explore particular venues in neighborhoods: 
      url='https://api.foursquare.com/v2/venues/explore?&client_id={}&client_secret={}&v={}&ll={},{}&radius={}&limit={}'
    
    - explore trending venues (that have the highest foot traffic): 
    url='https://api.foursquare.com/v2/venues/trending?&client_id={}&client_secret={}&v={}&ll={}'
    
   3. In addition to Foursquare we will use some other datasets in order to make our analysis more complex and versatile.
      Thanks to free source NYC Open Data https://opendata.cityofnewyork.us/ we have at our disposal following useful datasets that can       help us to refine the decision-path in our project:
      
      
      Business Improvement Districts of New York:
      https://data.cityofnewyork.us/Business/Business-Improvement-Districts/ejxk-d93y
      
     
      Primary Commercial Zoning of New York:
      https://data.cityofnewyork.us/Business/Primary-Commercial-Zoning-by-lot/pwhj-ikym
      
      
      Summary of Neighborhood Sales for Brooklyn for Class 1-, 2- and 3-Family homes - 2009Housing & Development:
      (this dataset can be useful to cluster Brooklyn Neighborhoods by living standarts)
      https://data.cityofnewyork.us/Housing-Development/DOF-Summary-of-Neighborhood-Sales-for-Brooklyn-for/nbun-a9vi
   
