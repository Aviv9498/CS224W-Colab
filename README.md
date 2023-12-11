# CS224W-Colab
## Solutions for Stanford CS224W (Machine Learning with Graphs) Colab, Winter 2021

http://snap.stanford.edu/class/cs224w-2020/

http://web.stanford.edu/class/cs224w/

- In Colab 0 we get familiar with the basic concepts of graph mining and Graph Neural Networks.
In this Colab, we will introduce two packages, NetworkX and PyTorch Geometric. This is a tutorial based on  https://colab.research.google.com/github/jdwittenauer/ipython-notebooks/blob/master/notebooks/libraries/NetworkX.ipynb#scrollTo=zA1OO6huHeV6 and  https://colab.research.google.com/drive/1h3-vJGRVloF5zStxL5I0rSy4ZUPNsjy8?usp=sharing#scrollTo=ci-LpZWhRJoI 

- In Colab 1, we will write a full pipeline for learning node embeddings. We will go through the following 3 steps.
To start, we will load a classic graph in network science, the Karate Club Network. We will explore multiple graph statistics for that graph.
We will then work together to transform the graph structure into a PyTorch tensor, so that we can perform machine learning over the graph.
Finally, we will finish the first learning algorithm on graphs: a node embedding model
- In Colab 2, we will construct our own graph neural network by using PyTorch Geometric (PyG) and apply the model on two of Open Graph Benchmark (OGB) datasets. Those two datasets are used to benchmark the model performance on two different graph-related tasks. One is node property prediction, predicting properties of single nodes. Another one is graph property prediction, predicting the entire graphs or subgraphs.
At first, we will learn how PyTorch Geometric stores the graphs in PyTorch tensor.
We will then load and take a quick look on one of the Open Graph Benchmark (OGB) datasets by using the ogb package. OGB is a collection of realistic, large-scale, and diverse benchmark datasets for machine learning on graphs. The ogb package not only provides the data loader of the dataset but also the evaluator.
At last, we will build our own graph neural networks by using PyTorch Geometric. And then apply and evaluate the models on node property prediction and grpah property prediction task.
- In Colab 3 we will implement the GraphSAGE (Hamilton et al. (2017)) and GAT (Veličković et al. (2018)) layers directly. Then we will run our models on the CORA dataset, which is a standard citation network benchmark dataset.
We will then use DeepSNAP, a Python library assisting efficient deep learning on graphs, to split the graphs in different settings and apply dataset transformations.
At last, using DeepSNAP transductive link prediction split functionality, we will construct a simple GNN model on the edge property predition (link prediction) task.
- In Colab 4 , we will shift our focus from homogenous graphs to heterogeneous graphs. Heterogeneous graphs extend the traditional homogenous graphs that we have seen before by specifically incorperating different node and edge types. This additional information allows us to extend the graph neural nework models that we have worked with before. Namely, we can apply heterogenous message passing, where different message types now exist between different node, edge type relationships.
At first, we will learn how to transform NetworkX graphs into DeepSNAP representations. Additionally, we will dive deeper into how DeepSNAP stores and represents heterogeneous graphs as PyTorch Tensors.
Then, we will build our own heterogenous graph neural netowrk models using PyTorch Geonetric and DeepSNAP on node property prediction task. To evaluate these models, we will use our model on the heterogeneous ACM dataset.
- Colab 5 is also a tutorial. we will experiment on scaling up GNNs using PyTorch Geometric, DeepSNAP and NetworkX.
At first, we will use PyTorch Geometric NeighborSampler to scale up the training and testing on OGB arxiv dataset.
Then, using the DeepSNAP and NetworkX, we will implement a simplified version of NeighborSampler and run experiments with different smapling ratios on the Cora graph.
At last, we will partition the Cora graph into clusters by using different partition algorithms and then train the models in the way of vanilla Cluster-GCN.
