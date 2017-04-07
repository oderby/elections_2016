# Diving into Election Data

This repo is a scratch space I used to collect, transform and analyze recent US
presidential election data. It's all a bit rough around the edges. If you want
to see the finished product, you should check out my blog post on the 2016
election in Pennsylvania.

# Sources

So far, I've only collected data for Pennsylvania elections in this repo. The
data was collected from the following sources:

* 2016 PA general election
  results:
  [Official PA Election Returns](http://www.electionreturns.pa.gov/ENR_New/General/CountyBreakDownResults?officeId=1&districtId=1&ElectionID=undefined&ElectionType=undefined&IsActive=undefined)
* 2000-2012 PA general election results: [Open Election Raw Data](https://github.com/openelections/openelections-results-pa/tree/master/raw)
* 1996 PA general election
  results:
  [The Wilkes University Election Statistics Project](http://staffweb.wilkes.edu/harold.cox/pres/PaPres1996.html)
* 2000-2016 PA voter registration
  statistics:
  [PA DoS Archive](http://www.dos.pa.gov/VotingElections/OtherServicesEvents/VotingElectionStatistics/Pages/Voter-Registration-Statistics-Archives.aspx)
* 1996-2008 PA Population Estimates by
  County:
  [PA Vital Statistics Archive](http://www.statistics.health.pa.gov/HealthStatistics/VitalStatistics/PAVitalStatistics/Pages/PAVitalStatistics.aspx#.WOf1N3XytaM)
* 2012 & 2016 PA Population Estimates by
  County:
  [US Census PEPANNRES: Annual Estimates of the Resident Population: April 1, 2010 to July 1, 2016](https://factfinder.census.gov/faces/tableservices/jsf/pages/productview.xhtml?pid=PEP_2016_PEPANNRES&prodType=table) (Click
  "Add/Remove Geographies" > Select "Geographic Type":"County",
  State:Pennsylvania > Select "All Counties within Pennsylvania")

I automated the processing of the 2000-2016 election results in
the [process_pa_results.ipynb](process_pa_results.ipynb)
notebook. The 1996 results and all voter registration statistics came as tables
that I just copied and renamed the headers.

In my work, I've found a few additional resources that are trying to compile
this data in a central location:

* [Open Elections](http://www.openelections.net/) - long running project, going
  all the way down to the precinct level. Taking a depth-first approach to
  gathering their data - so if they have the data for the state you're
  interested in, they have more detail than you probably
  want.
* [Data for Democracy](https://github.com/Data4Democracy/election-transparency) -
  fairly new project, but seem to be quickly getting all the data (results and
  registrations) at a county level.

# Analysis

All analysis is contained in the [plot_pa.ipynb](plot_pa.ipynb)
notebook.

# Further Resources

http://trends.vera.org/about
http://www.nytimes.com/interactive/2016/11/08/us/politics/election-exit-polls.html?_r=0
http://www.cor.pa.gov/About%20Us/Statistics/Documents/Reports/2014%20Annual%20Statistical%20Report.pdf
http://archives.lib.state.ma.us/handle/2452/40889/discover?filtertype=dateIssued&filter_relational_operator=equals&filter=%5B2000+TO+2014%5D
http://www-personal.umich.edu/~mejn/election/2016/

https://www.brookings.edu/wp-content/uploads/2016/06/04_political_demographics_frey_teixeira.pdf
