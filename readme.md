# Analysis of Moscow City Duma 2024 E-voting

The original data were acquired from the official portal for e-voting observers observer.mos.ru by e-voting observer Alexander Isavnin. The data consisted of all of the transactions that have entered the system. The raw data are stored [here](https://data.deg.observer/2024/msk-autumn/), in the format of multiple JSON files, hourly downloaded from the portal.

The raw data were processed by data journalist and researcher Alesya Sokolova to get a .csv file convenient for the analysis, it can be found in **results.csv.zip**. It consists of decrypted votes. The decryption was realized by the Moscow DIT (Department of Information Technology) -- the developer of the Moscow e-voting system. The file consists of the following columns:

- *timestamp* - time of storing the ballot
- *candidate* - the name of the candidate
- *Io* - number of a constituency

There were 45 constituencies in Moscow. The numbers in the data from observer.mos.ru do not match the numbers of the constituencies used in the official reports and announcements. The mapping to the official names of the constituencies can be found in a separate file **constituencies_mapping.json**. 

The file **Data processing.ipynb** consists of the processing of the raw data to the final .csv table and the code to produce data for the visualizations used for the [publication in Novaya Gazeta Europe](https://novayagazeta.eu/articles/2024/09/10/nedokrutili). **_Additionally, the plots for candidates' results dynamics in all 45 constituencies are presented in this file._**

