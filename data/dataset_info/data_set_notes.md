# Key Notes on the Dataset
___
## Graph Features
| Feature      | Description |
| ----------- | ----------- |
| Node      | Twitter User       |
| Edge   | Follower Relationship        |
| subgraph | All of the retweeters of a specific source tweet (e.g. a misinformation source tweet)|

## Dataset Structure
- __5G__ 
	- conspiracies about 5G causing COVID
- __Other__
	- Any other COVID conspiracy tweets
- __Non-Conspiracy__
	- Informational COVID-19 and 5G related tweets (from authorities)
---
### Node Properties
### Key Points
- The graphs are located individually in folders that are numbered in ascending order. 
- Each folder contains three files. 
- The edges.txt file contains a directed edge list,  source-id  -> target-id, 
- the file nodes.csv contains an assignment from the node id to its properties  
- the plot.png file contains a plot of the
corresponding subgraph

### Additional Notes
- subgraphs are limited to 100 nodes
- The number of nodes in the nodes.csv file does not necessarily match the number of nodes included in the edges.txt because nodes without any edges are not contained in the latter. The friends and followers counts are rounded to the next power of two to preserve anonymity.

## References
1. [Highlighted Research Paper](Wico_Graph_Scroeder.pdf)
2. [Simula Wico-Graph Dataset](https://datasets.simula.no/wico-graph/)
