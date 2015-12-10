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

Because the Ward linkage was used (which seeks to minimize sum a squared differences overall), it is similar to K-means, which seeks to miniimize sum of squared differences within clusters. The subtle difference means the K-means clusters may be tighter -- and aside from a couple outliers (Agg Cluster-5 #5 is pretty tight), the plots seem to bear this out.

Stationarity:
As this is a timeseries, one technical aspect to consider is stationarity. This was not investigated methodically, but a glance at the plots indicate that only the Agg Cluster-5 produced a clear indication of non-stationarity (#5) with an upward trend. Possibly the Agg Cluster-3 produces an upward trend as well (#1). For K-means, only K-means-5 produced a non-stationary timeseries (#3), although a few others may or they may just have a structural abberation at the end. 

One might guess, that because K-means chooses arbitrary and random starting points, whereas as Agg. Clustering is hierarchical and bottom-up, that the latter would be more likely to group lower and higher zip codes together initially and if since they have more "room" to trend statistically, its more likely to pick up trends at the extreme (low-to-high, or hi-to-low).

Event detection:
Both instances of both algorithms indicate events in 1999 and 2007, namely that they are years of far greater variance among zip codes within clusters. 1999 in particular is interesting as both alogrithms indicate divergence, with strong upticks for some clusters and strong downticks for others that year. Since it's bottom up, I'm not sure if Agg Clustering is more likely to capture spatial correlation, since surely there is some among zip codes. That may be one reason it seems to more clearly show this divergence in 1999, assuming a geographical relationship.

Volatility:
Agg Clustering, particularly the 5-cluster instance, seems to capture volatility quite a bit more, parciuarlly in the late 90s to early 2000s. Perhaps this is because it captures spatial autocorrelation (as noted above) better than K-means through it's bottom-up approach. This is a stretch...but perhaps bc Ward linkage seeks to minimize overall variance (not just within clusters), it over-weights year-to-year change (since its possible those economics affect ALL zip codes and minimizing variance means following this macro-economic change), whereas K-means will over-weight longitudinal similarities within clusters, even if those clusters vary a lot between them as a consequence of year-to-year changes.

TASK 7: INTERPRETATION

