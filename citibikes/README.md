****************************************
For Homework 3 - Assignment 3: Citibike
****************************************

***IMPORTANT: FOR THIS ASSIGNMENT ONLY (UNZIP FUNCTION WAS ADDED FOR HOMEWORK 4, SEE BELOW IN THIS README): Due to size restrictions, the data used in this file could not be uploaded to Git in raw form, but only as a zipped file. In order to run this program, the file must be unzipped in the local directory. Alternatively, you can go here:

http://www.citibikenyc.com/system-data

And download (and unzip) the August 2015 dataset.
Additionally, the 'stations.csv' file must be in the local directory.

COLLABORATORS:
I did this project individually, but borrowed heavily from previous homework assignments and Stack Overflow.

IDEA: People use Citibike to commute across town in Manhattan where public transit is lacking because there are no trains or trains are hard to get to and/or bus routes are congested.

DATA PARAMETERS: This is exploratory, so the stations biked are somewhat arbitrary. A section of Midtown Manhattan, from 14th Street to 59th Street and from East River to Hudson River. Stations were chosen based on reviewing a map -- stations within 1 block of each of these selected streets were chosen.

Error bar graphs indicated the difference in sample proportions would not be significant and indeed a z test for 2 samples demonstrated this.

OUTLIERS:
We see a lot of stations on Broadway that increases the likelihood that a trip will end there. 59th street also had a higher number of trips end at different stations along the street, but could be tourists starting on 59th, traveling through Central Park, and returning to another station on 59th...not necessarily communiting along the street.

RESULTS:
As can be seen by the figures, while the crosstown streets did have a higher ratio of trips that started and ended on the same street, it was not significant. The Null hypothesis was NOT REJECTED at a signficance level of 0.05.

FURTHER RESEARCH:
The scope of the analysis was limited by time. Further research might look into:
- A more analytical way to decide what a "key" street is, perhaps based on other data sets like MTA or traffic.
- A more precise way to identify stations along a street, perhaps based on long/lat
- A look at an entire year of data
- A look into different subsets of the data: subscribers vs one-time users; weekday (specifically during rush hour) vs weekend
- One could even measure the trip length compared to an estimate time for a path between two stations and eliminate trips that are significantly longer than expected (i.e. not commuters, but tourists "looping" around)
- Look not only at start and end stations, but consider direction (east-to-west/west-to-east or uptown-downtown...)

****************************************************************
For Homework 4 - Assignment 1: "Citibikes-compare-distributions"
****************************************************************

This notebook has been set up with a URL pull and unzip function to extract CitiBike data, so no additional downloads or unzipping is needed, just run the code as is.

OVERVIEW
Narrative and descriptions of tests and results is documented in the notebook directly.

COLLABORATORS:
I did this project assignment individually, but I'd like to thank Nate Webber, Michelle He, Maria Ortiz and the others at the MAGNATE "late night crew" table, as well as Graham for some help. I borrowed from previous assignments and Prof B's prompts.
