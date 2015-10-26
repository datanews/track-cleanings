# NYCT Track Cleanings

Data on scheduled and historical track cleanings for New York City subway stations.

## Background

In the New York City Comptroller's May 2015 report, [Audit Report on the New York City Transit Authority's Track Cleaning and Painting of the Subway Stations](http://comptroller.nyc.gov/wp-content/uploads/documents/FM14_071A.pdf), one of the report's recommendations was that the MTA develop a more systematic approach to track cleanings.

In response, the MTA stated that they had used historical data about each station to create a system with six different categories of cleaning frequency.

In May 2015, WNYC submitted a FOIL request for the historical data involved in this calculation and the six categories established.

The data in this repository was received in September 2015.

## Notes

### `cleaning-schedule.csv`

* The six categories (`Weekly`, `Bi-Weekly`, `Tri-Weekly`, `Monthly`, `Quarterly`, and `Semi-Annual`) reflect the scheduled cleaning frequency for April - October 2015.  For example, the Greenpoint Avenue station is categorized as `Bi-Weekly`, so the goal was to clean it every two weeks.
* For the purposes of the six categories, a cleaning counts as a visit by a track cleaning crew.  A visit by a vacuum train does not count.

### `cleanings-vacuum.csv` and `cleanings-manual.csv`

* `cleanings-manual.csv` lists cleanings of the trackbed by a track cleaning crew.
* `cleanings-vacuum.csv` lists cleanings of the trackbed by a vacuum (VakTrak) train.
* These cleanings do not include cleanings of station entrances or platforms.
* The `Track` column lists specific tracks that were cleaned.  The `Tracks Done` column lists the number of tracks clean.  For example, if tracks V4 and V3 were cleaned, the `Track` column would list `V3,V4` and the `Tracks Done` column would list `2`.
* `cleanings-manual.csv` includes data on quantity of debris removed, and exact track footage covered.