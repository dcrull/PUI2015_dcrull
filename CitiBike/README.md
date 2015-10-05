For Homework 3 - Assignment 3: Citibike

***IMPORTANT: Due to size restrictions, the data used in this file could not be uploaded to Git in raw form, but only as a zipped file. IN order to run this program, the file must be unzipped in the local directory. Alternatively, you can go here:

http://www.citibikenyc.com/system-data

And download (and unzip) the August 2015 dataset.

IDEA: People use Citibike to commute across town in Manhattan where public transit is lacking because there are no trains or trains are hard to get to and/or bus routes are congested.

HYPOTHESIS: Key crosstown streets are more likely to have Citibike trips that start and stop along the same street than avenues with train lines are

DATA PARAMETERS: This is exploratory, so the stations biked are somewhat arbitrary. A section of Midtown Manhattan, from 14th Street to 59th Street and from East River to Hudson River.

    Key crosstown streets sample: 14th, 23rd, 34th, 42nd, 59th
    Selected bc these streets are all primary East-West arteries. They have no trains, or no trains that extend all      the way (such as L on 14th and 7 on 42nd). While crosstown bus routes were meant to link up with uptown/downtown     train stations on these streets, these bus routes are highly congested.

    Key avenues with trains sample: 8th, 7th, 6th, Broadway, Lex/Park
    Selected bc these streets are all primary Uptown/Downtown arteries that have train lines running along them          (A,C,E along 8th, 1,2,3 along 7th, B,D,F,M along 6th, N,Q,R along Broadway, 4,5,6 along Lex/Park.) 


TESTABLE HYPOTHESIS: The ratio of Citibike trips that start along a key crosstown street and end at another station on the same street vs. all trips that start on that street is greater than the ratio of trips that start along a key avenue with a train line and end at another station on the same street vs all trips that start on that street.

NULL HYPOTHESIS: The ratio of Citibike trips that start along a key crosstown street and end at another station on the same street vs all trips that start on that street is the same or smaller than the ratio of trips that start along key avenues with train lines and end at another station on the same street vs all trips that start on that street. With a significance level alpha = 0.05

This is an explora
