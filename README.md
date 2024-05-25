# 02-experiment-tracking

Tracking machine learning models is a crucial aspect in companies working with unstable data, such as live customer data or any data that changes over time. The ML model might perform well during training in a Jupyter notebook, but it could show poor performance in prediction with real data.

Experiment tracking involves keeping track of all relevant information about an ML model.

**ML experiment** — This refers to our machine learning model. When someone says they are tracking their experiment, they mean they are training the machine learning model and checking its performance.

**Experiment run** — Each trial in your machine learning model. For example, you run your machine learning model and get your r2 result. After that, you change some parameters and run again, resulting in 2 runs, each with different parameters and results.

**Run artifact** — This includes all kinds of information that we want to save with the machine learning model, such as the data source, developer, or environment settings, etc.

Source code, Environment, Data, Model, Hyperparameters, and Metrics are the common choices that most machine learning developers want to track.

The concept of model tracking, the tools, and the methods of how we can track the model are also super important. The tracking should be simple and compact so that not just a senior Machine learning developer can understand the result, but also a junior Machine learning model who started the job a week ago can understand the result. They should be able to get insights from the tracking about which run was successful, which parameters were used, and finally, which machine learning model has the best score. Therefore, it’s time for us to talk about MLflow.

MLflow is an open-source platform for the machine learning lifecycle. It is a python package that you can easily install with the pip command,

```bash
pip install mlflow
