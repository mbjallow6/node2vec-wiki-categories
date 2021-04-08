# Representation Learning on Wikipedia Categories
Application of node2vec algorithm on Stanford Wikipedia Network of Top Categories dataset

| Filename | Description |
| --- | --- |
| [Data Exploration.ipynb](Data Exploration.ipynb) | Data Preprocessing and Exploration notebook |
| [Analysis and Results.ipynb](Analysis and Results.ipynb) | Analysis and Reporting notebook |

###  Dataset - [SNAP Wikipedia Network of Top Categories](https://snap.stanford.edu/data/wiki-topcats.html)
This is a web graph of Wikipedia hyperlinks where every web page is considered as an article. Every article has a page name and a category associated with it. These categories serve as ground truths for the various communities existing in the network. 
| File Name | Description |
| --- | --- |
| wiki-topcats.txt.gz | Edges of the network |
| wiki-topcats-categories.txt.gz | Webpages belonging to each Category |
| wiki-topcats-page-names.txt.gz | Name of the various webpages |

### Python Libraries 
- **Networkx** - used for creating Network / Graph instance
- **Stellar Graph** - used for performing Biased Random Walks
- **Gensim** - used for Word2Vec implementation
- **Keras** - used for implementing Feed Forward Network
- **Scikit-Learn** - used for tsne, PCA and KMean implementation
- **Bokeh** - used for Visualization
- **Pickle** - used for Checkpointing

### Notes
- Certain operations will be time consuming and could go upto 50 mins
- Check point data files not upload on github as they exceed github size limits
- Update the local file paths while reading and creating the checkpoints. 
- I maintained the following directory structure
    - **./dataset** - for storing the extracted dataset
    - **./checkpoints** - for storing intermediate pickle files
    - **./plots** - for storing visualizations and screenshots 

### References 
- [SNAP Dataset - Wikipedia network of top categories](https://snap.stanford.edu/data/wiki-topcats.html)
- [node2vec: Scalable Feature Learning for Networks](https://cs.stanford.edu/~jure/pubs/node2vec-kdd16.pdf)
- [StellarGraph Machine Learning Library](https://stellargraph.readthedocs.io/en/stable/README.html)
