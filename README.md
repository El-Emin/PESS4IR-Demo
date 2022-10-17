# PESS4IR-Demo
Demo for PESS4IR approach
 
Usage: retrieveRanking.py [indexFileName] [queriesFileName] [path/to/Folder/] [meanScore]


1)	indexFileName : The file name of inverted index file.
In this demo, data/robustCollectionIndex.txt is inverted index corresponding to the Standard Collection Robust04, annotated by our entity linking method (EL4DT).

2)	queriesFileName: The file name of annotated entities. 
In the demo, is the annotated entities of Robust04 query set, which are annotated by two entity linking methods, namely REL and DBpedia Spotlight (bumchQ_REL_Annotations.txt and bumchQ_Spotlight_Annotations.txt, respectively).

3)	meanScore: The mean score of entities annotation score corresponding to the given query. It should be between 0 and 1.

Execution Requirements:
-	At least python 3.6.8 

Execution example:
python retrieveRanking.py robustCollectionIndex.txt bumchQ_REL_Annotations.txt PESS4IR-Demo/data/ 0.75
python retrieveRanking.py robustCollectionIndex.txt bumchQ_Spotlight_Annotations.txt PESS4IR-Demo/data/ 0.95
