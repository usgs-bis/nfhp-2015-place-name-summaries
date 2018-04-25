*** DRAFT *** Code Used to Summarize the National Fish Habitat Partnership's National Inland Assessment of Fish Habitat Condition (2015) 
to Ecological and Jurisdictional units.
===============================================================================================================

-----------
Contact:
-----------
Daniel Wieferich (dwieferich@usgs.gov)


-----------
Collaborators:
-----------
Dana Infante: Aquatic Landscape Ecology Lab; Fisheries and Wildlife Department Michigan State University		  
Kyle Herreman: Aquatic Landscape Ecology Lab; Fisheries and Wildlife Department Michigan State University		  
Arthur Cooper: Aquatic Landscape Ecology Lab; Fisheries and Wildlife Department Michigan State University		  
Wesley Daniel: Cherokee Nation contracted to US Geological Survey		  
National Fish Habitat Partnership 		



-----------
Purpose:
-----------
This repository contains IPython Notebooks and Python files documenting methods that summarize and visualize the National Fish Habitat Partnership's (NFHP) National Inland Assessment of Fish Habitats (2015)
to ecological and jurisdictional boundaries that may be relevant to conservation decisions (e.g. National Park Boundaries, Hydrological Units, States).  

Often biologist, park managers and other decision makers are confronted with the need to prioritize funding of conservation and restoration efforts with limited resources and information to make these decisions.
These summaries of NFHP data are intended to give a user an additional set of information helping them better understand implications of fish habitat condition within their jurisdiction and associated ecological units. 
More specificly this information is anticipated to help ensure the user is considering appropriate disturbances at appropriate spatial scales when making decisions about fish habitat. A few more directed use cases are described below.

For smaller spatial units and jurisdictions, managers are likely to be aware of specific disturbances and associated issues with fish habitat, but
landscape level influences may be less intuitive and harder to quantify.  These users can use the NFHP summaries to help understand a quick overview of disturbances and spatial scales (e.g. especially network disturbances) to further 
investigate through exploring NFHP's catchment level information (i.e. habitat condition scores, significant disturbance metrics, and disturbance summaries) and other finer resolution sources of information that may be available.
  
In cases where several ecological units are within a larger jurisdiction a decision maker can quickly compare overall risk of fish habitat degredation and influencing disturbances.  Again these findings can be further 
investigated by exploring NFHP's catchment level information (i.e. habitat condition scores, significant disturbance metrics, and disturbance summaries) and other finer resolution sources of information that may be available.
  


-----------
Additional Details:
-----------
The source data include habitat condition indicies and select landscape disturbances (having nationaly consistent coverage) that influence fish habitat at 4 spatial scales (i.e. local catchment, network catchment, local catchment buffer, and 
network catchment buffers) for over 2 million stream segments of the National Hydrography Plus Version 1 datasets within the conterminous United States. Use this link to find out more about the 
NFHP source data being used in these efforts: https://doi.org/10.5066/F73R0R1P.    
  
This repository currently provides methods of summarizing information to spatial units of interest in the notebook: nfhp-2015-hci-summarized-using-midpoint.ipynb
Curent summarization methods take NFHP data (at the stream reach scale) and summarize it to the spatial unit of interest.  A stream reach is included in a summary if it's midpoint falls within
the spatial unit.  Habitat condition indicies are then summarized using a length-weighted average.  Disturbance variables for each of the four spatial scales are summarized by combining lists
of disturbances from individual stream reaches into a common list of unique values.   
  
This repository currently provides methods of visualizing summarized NFHP data in the following ways.	  
	1. Display total kilometers of NHDPlusV1 streams being scored by NFHP within a spatial unit (nfhp-2015-hci-total-stream-km-scored-per-spatial-unit.ipynb)	  
	2. Display length-weighted averages of fish habitat condition indicies for a given spatial unit. (nfhp-2015-place-name-summaries.ipynb)	  
	3. Display disturbance variables that influenced fish habitat condition within a given spatial unit. (nfhp-2015-table-of-significant-disturbances-per-spatial-unit.ipynb)	  



This software is preliminary or provisional and is subject to revision. It is being provided to meet the need for timely best science. 
The software has not received final approval by the U.S. Geological Survey (USGS). 
No warranty, expressed or implied, is made by the USGS or the U.S. Government as to the functionality of the software and related material nor shall the fact of release constitute any such warranty. 
The software is provided on the condition that neither the USGS nor the U.S. Government shall be held liable for any damages resulting from the authorized or unauthorized use of the software. 

-----------
Audiences:
-----------
National Fish Habitat Partnership, Natural Resource Managers, Conservation Decision Makers, Environmental Policy Makers


-----------
Development Status:
-------------------
Software documented in this repository are unpublished and will be under continual development.  Collaborative efforts to help improve code and analyses are welcomed.


----------------------
Copyright and License:
---------------------
This USGS product is considered to be in the U.S. public domain, and is licensed under
[CC0 1.0](https://creativecommons.org/publicdomain/zero/1.0/).

Although this software program has been used by the U.S. Geological Survey (USGS), no warranty, expressed or implied,
is made by the USGS or the U.S. Government as to the accuracy and functioning of the program and related program
material nor shall the fact of distribution constitute any such warranty, and no responsibility is assumed by the
USGS in connection therewith.
