#The Master Dataset
[Download the Master Dataset 17-18 GB .csv file](https://www.dropbox.com/s/c1lcdjp8x66fehe/taxi_2013.csv?dl=0)

##Big Query code
	select tuid, count(*) from [taxitest.taxi5]  where type='d' group each by tuid having count(*) >1

##Latest Maps
###Taxi 2013 Distance from Roadbed by Census Block 2010 & Taxi 2013 Count Taxi Pickup and Dropoffs by Census Block 2010
[![Click here for CartoDB Map on IPython Notebook](img/cartodb_screenshot.png)](http://nbviewer.ipython.org/github/nygeog/taxi/blob/master/tasks/201504_stat4701/12-map-plots.ipynb)

#Working Maps and Code
##Maps
![map1](https://raw.githubusercontent.com/stat4701-edav-gps/gps-taxi/master/img/bldg_distance.png)

![map2](https://raw.githubusercontent.com/stat4701-edav-gps/gps-taxi/master/img/midtown_20130101.png)

![leg_map2](https://raw.githubusercontent.com/stat4701-edav-gps/gps-taxi/master/img/midtown_20130101_legend.png)

![Steve Map](img/gps_map_v02.png)
##Concept
###Google Earth screenshot
![img/ge.png](img/ge.png)
###Building and neighborhood geography
![img/3dbldg.png](img/3dbldg.png)
###Building Volume Spread over the entire neighborhood
![img/bulk.png](img/bulk.png)


##Plots
![plot_1](https://raw.githubusercontent.com/stat4701-edav-gps/gps-taxi/master/img/plot_1.png)

##Input Spatial Data
###[Roadbed Data](https://data.cityofnewyork.us/City-Government/Roadbed/xgwd-7vhd)

##Code and Repo's
* [Emilie's Repo](https://github.com/embruze/edav/blob/gh-pages/_posts/2015-03-30-redsproject.md)

* [Danny's old repo](https://github.com/nygeog/gps_urban)

* [201408_descriptive_stats](https://github.com/nygeog/taxi/tree/master/tasks/201408_descriptive_stats) See link for code. 

* [201409_roadbed_centerline](https://github.com/nygeog/taxi/tree/master/tasks/201409_roadbed_centerline) See link for code. 

* [201504_stat4701](https://github.com/nygeog/taxi/tree/master/tasks/201504_stat4701)

	* [00-combine-orig-with-pickup-dropoff-roadbed-distances.ipynb](http://nbviewer.ipython.org/github/nygeog/taxi/blob/master/tasks/201504_stat4701/00-combine-orig-with-pickup-dropoff-roadbed-distances.ipynb)
	* [01-split-xy-for-pickups-and-dropoffs.ipynb](http://nbviewer.ipython.org/github/nygeog/taxi/blob/master/tasks/201504_stat4701/01-split-xy-for-pickups-and-dropoffs.ipynb)
	* [02-bring-csv-to-shp.ipynb](http://nbviewer.ipython.org/github/nygeog/taxi/blob/master/tasks/201504_stat4701/02-bring-csv-to-shp.ipynb)
	* [03-csv-xy-intersect.ipynb](http://nbviewer.ipython.org/github/nygeog/taxi/blob/master/tasks/201504_stat4701/03-csv-xy-intersect.ipynb)
	* [04-ogr-shp-to-csv.ipynb](http://nbviewer.ipython.org/github/nygeog/taxi/blob/master/tasks/201504_stat4701/04-ogr-shp-to-csv.ipynb)
	* [05-combine-tables.ipynb](http://nbviewer.ipython.org/github/nygeog/taxi/blob/master/tasks/201504_stat4701/05-combine-tables.ipynb)
	* [06-concat-master.ipynb](http://nbviewer.ipython.org/github/nygeog/taxi/blob/master/tasks/201504_stat4701/06-concat-master.ipynb)
	* [07-collapse-geoid.ipynb](http://nbviewer.ipython.org/github/nygeog/taxi/blob/master/tasks/201504_stat4701/07-collapse-geoid.ipynb)
	* [10-plots.ipynb](http://nbviewer.ipython.org/github/nygeog/taxi/blob/master/tasks/201504_stat4701/10-plots.ipynb)
	* [11-plots-2.ipynb](http://nbviewer.ipython.org/github/nygeog/taxi/blob/master/tasks/201504_stat4701/11-plots-2.ipynb)
	* [12-map-plots.ipynb](http://nbviewer.ipython.org/github/nygeog/taxi/blob/master/tasks/201504_stat4701/12-map-plots.ipynb)
	
#Completed Maps and Code

#Data
###[Sample January 1, 2013 Pickups Only](https://github.com/stat4701-edav-gps/gps-taxi/blob/master/data/p_20130101_avg_dist.csv)	
![data_shot](https://raw.githubusercontent.com/stat4701-edav-gps/gps-taxi/master/img/data_shot.png)
	
###[Richie's Data](https://github.com/stat4701-edav-gps/gps-taxi/tree/master/data/rc_data/Archive)
	
#To Do:

* Consider no longer using Census Blocks as larger bocks have a tendency to have larger distances. Perhaps this should in fact be an overlayed GRID. 

###DS 
Create flag for Census Block as either Park or no buildings.


EB, RC, SG, DS

Sankara, Emilie and I met yesterday and here are next steps. Is this possible to be done over the weekend?:

1. Richie - Pull one day's worth of data and try to do some clustering. Let's use what Danny posted for Feb 26, 2013
2. Danny - Use that data to plot on a map. Danny, did you have ideas on what specifically will be useful? We thought we'd like to see how the plot would look if overlaid and how popular some places are.
3. Emilie/Sankara - Write up the plan.

Let me know if I missed anything. Let's reconvene Tuesday.

#Outline:
1) Front Matter

* Title page (page 1)
* Executive summary (page 1)
* Table of contents (page 2)
* Lists of figures and tables (page 2)

2) Introduction

* Statement of the research problem
* Project purpose, background, and context
* Main objectives and contributions of the study
* Spatial questions and hypotheses
* Study area description, location, and context

3) Research Design

* Literature Review (at least 3 scholarly)
* Conceptual framework and definition of key terms
* Description of concepts

4) Methods

* Description and operationalization of data
* Data analysis and modeling (bulleted)


5) Results & Discussion

* Results of data analyses
* Presentation of results in text, figures, and tables
* Review of results in relation to spatial hypotheses and research problem
* Discussion of results in the context of the project background
* Conclusions and recommendations based on results
* Recommendations for future studies

6) References	

* Data Source References (last page)
* Works Cited
* Appendices (if neccessary)