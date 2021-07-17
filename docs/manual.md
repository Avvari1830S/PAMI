1. [About PAMI](index.html)
   
   Lack of Python libraries to discover hidden patterns in databases motivated us to develop PAMI.

1. [Installation/Update/uninstall PAMI](installation.html)
   
         pip install pami
   
1. [Organization of Algorithms in PAMI](organization.html)
   
   The algorithms in PAMI are organized in a hierarchical structure as follows: 
   
        PAMI.theoriticalModel.basic/maximal/closed/topk.algorithmName
   
1. [Creating Databases](createDatabases.html)
   
    1. [Transactional database](transactionalDatabase.html)
       
       Every transaction contains items seperated by a separator.
       
            format: item1<sep>item2<sep>...<sep>itemN
       Default separator is tab; 
       however, users can override the separator with their choice. 
    1. [Temporal database](temporalDatabase.html)
         Every transaction contains a timestamp followed by items.       

            format: timestamp<sep>item1<sep>item2<sep>...<sep>itemN
    1. [Neighborhood database](neighborhoodDatabase.html)
   
        Every transaction contains a spatial item and its neighboring spatial items seperated by a tab space.
            
            format: spatialItem1<sep>spatialItem3<sep>spatialItem10<sep>...
       
    1. [Utility database](utilityDatabase.html)
       
        Every transaction contains items, their total utility, and their individual utility values.
       
            format: item1<sep>...<sep>itemN:totalUtility:utilityItem1<sep>...<sep>utilityItemN
    
1. [Converting Dataframes to Databases](df2db.html)
   1. [Dense dataframe to database](denseDF2DB.html)
   1. [Sparse dataframe to database](sparseDF2DB.html)
   1. [Spatiotemporal dataframe to databases](stDF2DB.html)
   
1. [Exceuting Algorithms in PAMI](utilization.html)    