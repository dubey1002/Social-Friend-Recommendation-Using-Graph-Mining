# Social-Friend-Recommendation-Using-Graph-Mining

<p style="font-size:32px;text-align:center"> <b>Social network Graph Link Prediction - Facebook Challenge</b> </p>
<h3> Problem statement: </h3>
Given a directed social graph, have to predict missing links to recommend users (Link Prediction in graph)
<h3>Data Overview</h3>
Taken data from facebook's recruting challenge on kaggle https://www.kaggle.com/c/FacebookRecruiting  
data contains two columns source and destination eac edge in graph <br>
    - Data columns (total 2 columns):  <br>
    - source_node         int64  <br>
    - destination_node    int64  <br>
<h3>Mapping the problem into supervised learning problem:</h3>
- Generated training samples of good and bad links from given directed graph and for each link got some features like no of followers, is he followed back, page rank, katz score, adar index, some svd fetures of adj matrix, some weight features etc. and trained ml model based on these features to predict link. <br>
- Some reference papers and videos :  <br>
    - https://www.cs.cornell.edu/home/kleinber/link-pred.pdf <br>
    - https://www3.nd.edu/~dial/publications/lichtenwalter2010new.pdf <br>
    - https://kaggle2.blob.core.windows.net/forum-message-attachments/2594/supervised_link_prediction.pdf <br>
    - https://www.youtube.com/watch?v=2M77Hgy17cg <br>
  
<h3> Business objectives and constraints: </h3> 
- No low-latency requirement. <br>
- Probability of prediction is useful to recommend ighest probability links <br>

<h3>Performance metric for supervised learning:  </h3>
- Both precision and recall is important so F1 score is good choice
- Confusion matrix
