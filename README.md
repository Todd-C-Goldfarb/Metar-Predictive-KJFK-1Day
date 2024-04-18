# Metar-Predictive-KJFK-1Day
Contact: tcgoldfarb@gmail.com

Date: 7/26/2023

NOTE: This was conceptual code I wrote for my internship at Autonomic Solutions. The repository that the data is pulled from no longer exists, so the model no longer has access to the METAR dataset.

This is a METAR-PREDICTIVE-KJFK-1DAY model for the JFK Airport (ICAO CODE KJFK). From what I believe, an RNN network would be ideal for this first experiment (LSTM specific). We will have to pre-process and create our own dataset.

Using .TXT and .CSV files of METAR data related to KJFK, we will isolate the viable inputs and space the answer input by a distance of one day (from the latest METAR given). For example, if we give three months worth of METAR data related to KJFK, we will space it one day off of the lastest day in the three months of data. We will be using 7+ total months of KJFK METAR data.

Ideally, the model takes in about a week's worth of input data, and can give the predictive following day.

(link to the one of the METAR sources, stores historical data but is in .TXT format: http://www.ogimet.com/metars.phtml.en)

This link only accepts 31 days at a time, but we can take multiple chunks. I've taken 7 chunks and put them together on a txt file in my github public data repo.
(link to a dataserver of CSV data, not airport specific, only stores 3 days of data then clears: https://www.aviationweather.gov/dataserver)

Will be great for testing!
