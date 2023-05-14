# Stock-X

This project is all about analysis of Stock Market and providing suggestions to stockholders to invest in right company

Main repo link: [here](https://github.com/Circle-1/Stock-X)
Note: The notebook used here (IPYNB) is made using Kaggle, a data-science and ML community website which provides free Jupyter Notebook environment to work on programs and GPUs and TPUs to work on Neural Networks easily.

Helm charts: [![Artifact Hub](https://img.shields.io/endpoint?url=https://artifacthub.io/badge/repository/stock-x)](https://artifacthub.io/packages/search?repo=stock-x)

![Version: 0.1.4](https://img.shields.io/badge/Version-0.1.4-informational?style=flat-square)

## How to run Helm charts in my Kubernetes cluster?

Run the following commands: (make sure you have both Helm CLI and Kubernetes installed)

```
helm repo add stock-x https://circle-1.github.io/helm-charts/
```

```
helm install [app-name] stock-x/stock-x --version [version-tag]
```

To check if Helm charts are deployed, type
```
helm ls
```

After that, connect to localhost via port (get reference of port using `kubectl get svc` don't use 8888 it won't work) and then you'd see the jupyterlab interface; use a token by getting through inside a pod via SSH with the docker container.
