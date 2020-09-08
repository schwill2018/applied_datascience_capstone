The Data used in this report consists of geospatial neighborhood data for various major cities in North America.
  -The "Master" Dataset that is being recommended on consists of Neighborhood and Foursquare venue data for cities:
      -Toronto, Canada
      -San Francisco, California
      -Chicago, Illinois
      -Manhattan, New York
   -"Ideal" Neighborhood data will be the input to the KMeans prediction and recommendation engine.
      -This data is based on user known neighborhoods and ideal/preferred neighborhoods
      -This data attempts to quantize the user's understanding of "where home is"
   -Neighborhood Data was obtained via various city OpenData portals.
      -Most Neighborhood geospatial data was listed in a polygon format.
      -ArcGIS, a geospatial data tool, was used within free-rate limits to:
        1) Load, preprocess, and manipulate geospatial type files (e.g. GeoJSON, Shape files, etc.)
        2) Convert polygon data to Latitude/Longitude (lat/lng) oordinates.
        3) Find zipcodes of each neighborhood (via reverse-geocoding of the lat/lng coordinates)
        - ArcGIS applications to data found within city folders (see city-specific IPYNB files)
