# pandas-between-method

There are two CSV files.

File 1 = annotated.csv

<img width="197" alt="Screenshot 2023-05-05 at 15 21 11" src="https://user-images.githubusercontent.com/13205577/236469906-12ae49ec-fa4b-4ba5-86d8-befd419b9178.png">

File 2 = haplo.csv

<img width="264" alt="Screenshot 2023-05-05 at 15 27 16" src="https://user-images.githubusercontent.com/13205577/236470350-292fd15f-4861-4aca-8ed4-0ed2be821ddb.png">

annotated.csv has three columns: chr, start, alt and haplo.csv has four column: chr, start, end, score.

haplo.csv file contains regions (start and end columns). In the annotated.csv file has mutations also (start or end column). If a mutation falls within any of the regions in the haplo.csv file, then give it that score of that region.

For example, in annotation.csv file has this mutation: 

chr1-----234-----G 

and in haplo.csv file has those regions:

chr1-----200-----210-----3

chr1-----230-----240-----10

In this case, the mutation falls within the 2nd row of haplo.csv, so append a new colum for the mutation with score 10.
