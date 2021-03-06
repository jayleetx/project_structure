Repository Structure Proposal
================
Matthew Yancheff
May 23, 2017

Proposed Structure
------------------

``` r
#/raw-data
#/data
#/sandbox
#/code
#/documents
#/misc
#README.md
#makefile
```

This structure is largely based off of the TIER specifications found at <http://www.projecttier.org/>. The main modifications come from trying to match the directory structure to the data science work flow presented in the Math241/Pol341 course, as well as work done in reproducibility by Thomas Leeper.

![WorkFlow](visualizations/data-science.png)

This structure would be followed for each project in a repo, so a repo with multiple projects would have a single file for every project, and each of these files would then be organized with sub folders in this style.

Raw Data
--------

This folder would contain the raw data files scraped directly from their source and unaltered, as well as the programs used to tidy them. Files that go in here are files that are not used directly in any kind of analysis. For example, in the OMV project, this file would contain the raw voter files as well as the code used to clean it into the format used for the actual analysis.

This file would not appear in projects that focus on reading in and transforming raw data such as the RCV project or the US-elections-reboot. Instead these files would appear in the data and code folders later down the line.

Data
----

This folder would contain all the files used directly in analysis or in the final project.

Sandbox
-------

This folder would contain code and work that is not yet finished, corresponding to the general exploring/understanding phase of the data science work flow. Files in here will typically be code, and will be moved out of this file into the code file as they are completed and working.

Code
----

This folder would contain the code used in any analysis performed in the project. This would include the code to make visualizations, models, and any other analysis done.

Documents
---------

The documents folder would contain the final analysis, or the main deliverable(s) that the repo is dedicated to.

For standard social science projects this folder would contain the final draft of the paper, as well as a visualizations sub folder that would contain image files.

For a project more focused on building a tool, such as an r package, the documents folder would contain a file that shows examples of the code being used.

Miscellaneous
-------------

This would contain any files that don't fit into the descriptions of the above folders.

Other Files (Not a Folder)
--------------------------

The README file will contain the information needed for someone to get a good preliminary understanding of what the project is as well as how the repo is organized. This file should contain the names of people involved, the sources of data, and a general guide for where things are stored in the repo.

Issues
------
