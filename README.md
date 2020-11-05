# Scaling Machine Learning in Python

<img src="img/saturn.png" width="400" />

## Hands-on workshop: migrate data science workloads to Dask clusters

In this hands-on workshop, attendees will have the opportunity to see how a standard data science and machine learning workflow using pandas and scikit-learn can be easily parallelized using Dask clusters on Saturn Cloud.

After this workshop you will know:
- When you need parallel computing for your workflow
- How to use Dask Dataframes for loading and cleaning data
- How to perform distributed model training with Dask
- How to scale a hyperparameter search across a cluster
- How to conduct a batch inference task over a cluster

To get the full learning value from this workshop, attendees should have prior experience with machine learning in Python. Experience with parallel computing is not needed.

## Getting started

1. Create an account on [Saturn Cloud Hosted](https://accounts.community.saturnenterprise.io/register) or use your organization's existing Saturn Cloud Enterprise installation. 
1. Create a new project (keep defaults unless specified here)
    - Name: "workshop-scaling-ml"
    - Image: `saturncloud/saturn:2020.10.23` <br> (or latest available `saturncloud/saturn:*` image)
    - Workspace Settings
        - Size: `XLarge - 4 cores - 32GB RAM`
    - Click "Create"
1. Attach a Dask Cluster to the project
    - Worker Size: `XLarge - 4 cores - 32GB RAM`
    - Number of workers (n_workers): 3
    - Number of worker threads (nthreads): 4
    - Click "Create"
1. Start both the Jupyter Server and Dask Cluster
1. Open Jupyter Lab
1. From Jupyter Lab, open a new Terminal window and clone the workshop-scaling-ml repository:
    ```bash
    git clone https://github.com/saturncloud/workshop-scaling-ml.git /tmp
    cp -r /tmp/workshop-scaling-ml /home/jovyan/project
    ```
1. Navigate to the "workshop-scaling-ml" folder in the File browser and start from the [01-start.ipynb](01-start.ipynb) notebook.

