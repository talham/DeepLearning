# finalproject
## DATA622 Project

- Assigned on November 1, 2019
- Due on December 15, 2019 11:59 PM EST
- 30 points possible, worth 30% of your final grade

### Instructions:
1. Build a image recognition model (20 points)
Read the online textbook [Neural Networks and Deep Learning by Michael Nielsen](http://neuralnetworksanddeeplearning.com/) in its entirety (reasonably short). Use the code in the book to guide your thinking through steps to build an image recognition model on the classic MNIST dataset. Please try to build the model and summarize your results. The data pull steps can also be found in the book.

Implementation should be in python. Deployment can be on the cloud if you choose to. In addition, if you would like to leverage pyspark or other tools that you think that would help you, please feel free to choose those.

(resources for PySpark)
Read the following:
- [Apache Spark Python 101](https://www.datacamp.com/community/tutorials/apache-spark-python)
- [Apache Spark for Machine Learning](https://www.datacamp.com/community/tutorials/apache-spark-tutorial-machine-learning)

Optional Readings:
- [Paper on RDD](https://www.usenix.org/system/files/conference/nsdi12/nsdi12-final138.pdf)
- [Advanced Analytics with Spark: Patterns for Learning from Data at Scale, 2nd Edition](https://www.amazon.com/_/dp/1491972955), Chapters 1 - 2

Additional Resources:
- [Good intro resource on PySpark](https://annefou.github.io/pyspark/slides/spark/#1)
- [Spark The Definitive Guide](https://github.com/databricks/Spark-The-Definitive-Guide)
- [Google Cloud Dataproc, Spark on GCP](https://codelabs.developers.google.com/codelabs/cloud-dataproc-starter/)

2. Critical Thinking (10 points)
Submit a ~100 word explanation of the potential choices and tradeoffs you may think through in the process of building this model.  (e.g. why you go X layers deep? why you choose X cost function?).

The analysis shows some interesting results for simple Neural Network models and Convolution Neural Network models. Firstly, the CNN significantly outperforms all the different models. Even when the CNN has only one fully connected layer and one convolution layer with max pooling. 

The relu activation functions outperform other dense layer specifications although the tanh activation function seems to catch up and quite closely perform the relu specification (NN2-Re-Re). 

Finally we note some fo the following comments: 
- Conventional Neural Networks with 2 layers of max pooling with 20% Dropout (Model 4C) is the best performing model
- Conventional Neural Networks with 2 layers of max pooling (Model 2C) is second best performing model
- Regularization for these images do not seem to work too well as seen by the model (CNN - 2Max R); it is the same model as the one above, but with l2 norm regularization
- The simple two dense layer model with Relu activation does hold its own and its performance even exceeds the convolution neural network with regularization

### Additional Resources

1. The [Goodfellow book](http://www.deeplearningbook.org/) on Deep Learning is the authorative resource on this subject still.  
2. Check out [this curated list](https://github.com/ChristosChristofidis/awesome-deep-learning) for even more resources on deep learning. 
