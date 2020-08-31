---
yout: post
title:  "Final Evaluation phase"
date:   2020-08-30 20:00 +0530
categories: jekyll update
---
Hello, everyone! 

I have reached the end of final coding period and it's time for the Final evaluation. In these last weeks of final coding phase I worked on changing the functions that they now work successfully now. Tests have been made for these functions. I would say one thing that I underestimated the importance of processing and cleaning data. I started giving importance to code style during this journey. 

As this is the final blog post, this is what happened during this whole program with the details of the project.

### Data Retriever: Add support for more raw data formats:
The Data Retriever handles tabular data and spatial data forms. The goal of the project was to add support that will enable the Data Retriever platform to have the capability of ingesting other forms of raw data. The project introduce the support for raw data formats of XML, JSON, NetCDF, HDF, Excel, SQlite and Geojson data sources.

1. The First part of the project mainly comprised of adding functions for converting raw data sources. These raw data sources were XML, JSON, NetCDF, HDF, Excel, SQlite and Geojson. This included searching for the raw data sources in the respective formats.
2. The second part comprised of testing unit functions for the ability to transform the raw data into ready to ingest data. Scripts were also made to test these functions and to also set out the rules for writing the data packages. The data packages specified the type of raw data to be converted. 
3. In the final part, all the scripts used for testing were shifted to [retriever-recipies](https://github.com/weecology/retriever-recipes). 
4. Documentations were added for these functions. 
5. We decided to leave out NetCDF to csv conversion function as most of the datasets of NetCDF contain a more complex structure. Some of the tables have complex arrays that need much more processing to do. To compensate the exclusion of NetCDF to csv function, we worked on HDF5 engine which is working without any issues currently. 
6. I made the necessary changes to the two Retriever wrapper repositories: [Retriever.jl](https://github.com/weecology/Retriever.jl) and [rdataretriever](https://github.com/ropensci/rdataretriever).

During the course of the project, I mainly contributed to two repositories: retriever and retriever-recipes. The list of commits made in the two repositories:
* [Commits in retriever](https://github.com/weecology/retriever/commits?author=ashishpriyadarshiCIC)
* [Commits in retriever-recipies](https://github.com/weecology/retriever-recipes/commits?author=ashishpriyadarshiCIC)

### List of major pull requests made for the project:
* [JSON Support](https://github.com/weecology/retriever/pull/1507)
* [XML Support](https://github.com/weecology/retriever/pull/1506)
* [SQlite Support](https://github.com/weecology/retriever/pull/1505)
* [GeoJSON Support](https://github.com/weecology/retriever/pull/1504)
* [HDF5 Support](https://github.com/weecology/retriever/pull/1512)
* [HDF5 Engine](https://github.com/weecology/retriever/pull/1514)
* [Documentation](https://github.com/weecology/retriever/pull/1513)

I also wrote a number of blogs writing about the work done and experience during the program [here](https://ashishpriyadarshicic.github.io/)
 
In the end, I would like to thank my mentors [Henry Senyondo](https://github.com/henrykironde), [Apoorva Pandey](https://github.com/apoorvaeternity) and [Ethan White](https://github.com/ethanwhite) for giving me this opportunity to work with them. I would also like to thank [Harshit Bansal](https://github.com/harshitbansal05), [Ratin Kumar](https://github.com/DumbMachine) and [Bo zheng](https://github.com/coolalexzb) as their contributions helped me with some of the work. A special thanks to Henry Senyondo for his constant support and guidance. I might have lost focus to complete this project without his guidance. 

During this program I learned a lot of things like debugging code, processing & cleaning special data types like HDF5, GeoJSON etc and making tests. I also learned a lot about Docker and Travis CI. I've started giving more importance to open source when I had to use open source tools and library while working on the project.

I plan to continue contributing to the project in future as well as other Open source projects. Thank You everyone.
