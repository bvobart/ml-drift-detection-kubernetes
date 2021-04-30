# ml-drift-detection-kubernetes
Created during MLE Chapter day in an attempt to try and run the code from this article: https://towardsdatascience.com/production-machine-learning-monitoring-outliers-drift-explainers-statistical-performance-d9b1d02ac158

## Pre-requisites

- Python 3.8 (3.9 will not work with Tensorflow and alibi-detect)
- [Minikube](https://minikube.sigs.k8s.io/)
- [Poetry](https://github.com/python-poetry/poetry) - `pip install poetry`

## How to use this?

### Prepare Kubernetes environment

1. Run `minikube start` to start up a local Kubernetes
2. Install [Knative](https://knative.dev/docs/install/install-eventing-with-yaml/) Eventing:
    ```sh
    kubectl apply -f https://github.com/knative/eventing/releases/download/v0.22.0/eventing-crds.yaml
    kubectl apply -f https://github.com/knative/eventing/releases/download/v0.22.0/eventing-core.yaml
    ```
3. 

### Prepare project

1. Clone this repository: `git clone git@github.com:bvobart/ml-drift-detection-kubernetes.git`
2. `poetry install`
