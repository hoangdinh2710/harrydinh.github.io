---
layout: post
title: How to create training clusters
category: azureml
---

# Required

1. Azure Machine Learning Resouces

# Step by Step Instruction

1. Choose Compute ,click Training Clusters, then hit "New"

![Create training cluster](https://harryteststorageblob.blob.core.windows.net/blogazureimage/Image/studio/cs_studio_compute_training_cluster.png)

Set the name for the compute you want. The default region will be the same region that you set your Machine Learning resource. You can choose the Virtual Machine size that fit your scenario.

**How to choose Virtual Machine size**

Since this training cluster is used to train your model, so the VM size will depend on the size of the data and the complexity of the model that you have (The larger size of data and more complexity will need higher VM size). The best practice is to choose a moderate size and then watch the performance accordingly, then scale up or down depends on your scenario.

**How to choose the Virtual Machine priority**

This option simply a trade-off between performance and price. The dedicated (Low priority) will deliver higher (lower) performance but more (less) expensive 

**How to choose the number of nodes**

Since this is a training resource, we only use it when we need to train the models. Hence, it make sense. This training cluster allow auto-scale up and down depends on our usage. 

- Minimum number of nodes

It is highly recommended that you choose the minimum number of nodes = 0. Essentially, this help you to pay nothing when you do not need to train the model. 

- Maximum number of nodes

This is the maximum number of nodes that can run simultaneously to train your model. When you hit the limit of the cluster, all nodes will be used. Normally, we can choose 4 clusters which is recommended in the Azure documentation.

- Idle seconds before scale down

This is the idle time before the cluster is scaled down. You can set `120s` which is the default option. 

Now, you have successfully created the training resource. Let's use it to train your models.
