Ở phần này ta sẽ tìm hiểu về orchestration:

Tham khảo [medium article](https://towardsdatascience.com/machine-learning-orchestration-vs-mlops-d4cfe3b7bec).


Có thể hình dung Orchestration như sau:

```
Machine Learning Orchestrator (MLOx)
I like to think of an MLOx as being similar to a movie director (or a conductor for an orchestra, but that can be confusing since we would be talking about orchestrating an orchestra). A director has a script that they work from to direct the various processes to deliver the final product — the movie. In the context of an MLOx there is a workflow that would be the equivalent of the script. The role of the orchestrator is to ensure that the various processes that are part of the workflow execute on schedule, in the correct sequence and deal with failure appropriately.
```

```
The orchestrator is an essential component in any MLOps stack as it is responsible for running your machine learning pipelines. To do so, the orchestrator provides an environment which is set up to execute the steps of your pipeline. It also makes sure that the steps of your pipeline only get executed once all their inputs (which are outputs of previous steps of your pipeline) are available.
```