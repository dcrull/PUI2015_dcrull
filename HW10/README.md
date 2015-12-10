*************
HW 10
*************

NOTES ON SOURCE DATA:
All the required files are in this directory. The iPython notobook includes codes to unzip and read those files as dataframes in memory. FYI - the notobook also has code to retrieve these from the source server if necessary (it shouldnt be), but 2000 and 2001 must be manually downloaded as there was a formatting issue I didnt fix.

ACKNOWLEDGEMENTS:
I had some basic conceptual discussion with Dara Perl, Nate Webber, Maria Ortiz, and Michelle Ho, but the work here is all mine. Credit to them for telling me about the one-time homework extension policy...which I invoked.

TASK 6: RESULT COMPARISON
2 instances of a K-means algorithm were run: 3 and a 5-cluster initiation.
2 instances of a hierarchical algorithm were also run (Ward linkage methodology): 3 and 5-cluster end-states.
Note that a random seed was not set, so each K-means run would produce different initiation points.

Stationarity:
As this is a timeseries, one technical aspect to consider is stationarity. This was not investigated methodically, but a glance at the plots indicate that only the Agg Cluster-5 produced a clear indication of non-stationarity (#5) with an upward trend. Possibly the Agg Cluster-3 produces one as well (#1). For K-means, only K-means-5 produced a non-stationary timeseries (#3), although a few others may (or they may just have a structural abberation at the end). 

One might guess, that because K-means chooses arbitrary and random starting points, whereas as Agg. Clustering is hierarchical and bottom-up, that the latter would be more likely to group lower and higher zip codes together initially and if since they have more "room" to trend statistically, its more likely to pick up trends at the extreme (low-to-high, or hi-to-low).

K-means 3-cluster appeared to produce stationary clusters (but this was not validated methodically), whereas the K-means 5-cluster looks to have generated at least one cluster (#3) showing an upward trend, and possibly two (#1)...although that may be a structural abberation.

TASK 7: INTERPRETATION

