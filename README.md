# BigData 2025 Template Repository

![TartuLogo](./images/logo_ut_0.png)

Project [Big Data](https://courses.cs.ut.ee/2025/bdm/spring/Main/HomePage) is provided by [University of Tartu](https://courses.cs.ut.ee/).

Students: Anna Maria Tammin, Maria Anett Kaha

## Project 3
### Requirements
Folder for the data called "data" has to be created in the root of the repository. 

<b>data/2009.csv</b>

### Transformations
Project 3 dataset contains records of flights between various airports. Each row represents a direct flight connection between two airports, along with basic information such as the source and destination. 
Each row of the provided dataset represented an edge on the flight graphframe. After reading in the data, we created a dataframe of all the vertices (nodes) in the graph by selecting all source and destination airports from the flight data. Each node represents an airport. We also created a separate dataframe for the edges by renaming the origin and destination columns in the flight dataframe to “src” and “dst” as is needed to create the GraphFrame in Spark. Having created the necessary dataframes, we then combined them using the GraphFrame function to create our flight graph which could then be analysed.

### Queries 
The results of the queries can be seen in the Jupyter Notebook Graphframes.ipynb
1. Statistics in-degree, out-degree, total degree, and triangle count.
2. Total number of triangles in the graph.
3. Graph closeness centrality (natively on Spark using).
4. PageRank algorithm implementation natively on Spark using Graphframes.
5. Group of the most connected airports (largest connected component in the graph).

## Project 4
### Requirements
Folder for the data called "data" has to be created in the root of the repository. The project requires datasets 2009.csv and 2010.csv.
The project can be run using the Docker compose file provided in project_4 subfolder.
