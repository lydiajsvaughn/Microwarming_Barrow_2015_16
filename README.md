# Microwarming_Barrow_2015_16

Analysis of soil temperature data from field soil warming experiment in Utqiagvik, Alaska

Description of files:

(1)	Microwarming_data_formatting_2015.Rmd compiles, cleans, and computes averages with soil temperature data collected between July and October 2015.  Assigns flags to temperature measurements according to:
  
   mislabeled = raw data trace was improperly assigned to the temperature probe and location
  
   badTrace = poorly functioning temperature probe, based on visual analysis of data output
  
   ramp-up = after heater was turned on,  initial warming period before full 4-degree temperature difference is achieved.  Ramp up periods occur at the start of the season and following heater outages
  
   outlier = for data not flagged as mislabeled or badTrace, either (a) temperature values greater than 20 or less than -5, or (b) temperature values that lie more than 2 standard deviations from the mean over a 1-hour window.


(2)	Microwarming_data_formatting_2016.Rmd compiles, cleans, and computes averages with soil temperature data collected between May and October 2016.  Assigns flags to temperature measurements as with 2015 data.


(3)	Microwarming_fluxtemp_2015_16 merges trace gas flux data with corresponding soil temperature measurements, averaged over the 2 hours leading up to each flux measurement.


(4)	Microwarming_plots_flagged_2015_16 generates graphs from the cleaned temperature data.
