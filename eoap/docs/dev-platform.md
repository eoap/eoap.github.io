# How to run the modules

Each module brings its own set of requirements and runtime environment. Some may only require simple python code, others may require building and running containers or deploy several deployments on a kubernetes cluster.

The modules are thus supported by development platforms that may run on local computers and rely on a local ande development kubernetes cluster.

## Requirements

The development platforms relies on the requirements and tools below:

### Minikube

Minikube runs a local Kubernetes cluster, ideal for development and testing. 

Minikube is installed by following the guide [here](https://minikube.sigs.k8s.io/docs/start).

Verify the installation with:

```bash
minikube version
```

Start the local minikube instance with:

```bash
minikube start
```

In Ubuntu 24.04, this will typically show:

```
😄  minikube v1.33.1 on Ubuntu 24.04
🎉  minikube 1.34.0 is available! Download it: https://github.com/kubernetes/minikube/releases/tag/v1.34.0
💡  To disable this notice, run: 'minikube config set WantUpdateNotification false'

✨  Using the docker driver based on existing profile
👍  Starting "minikube" primary control-plane node in "minikube" cluster
🚜  Pulling base image v0.0.44 ...
🔄  Restarting existing docker container for "minikube" ...
🐳  Preparing Kubernetes v1.30.0 on Docker 26.1.1 ...
🔎  Verifying Kubernetes components...
    ▪ Using image gcr.io/k8s-minikube/storage-provisioner:v5
🌟  Enabled addons: storage-provisioner, default-storageclass
🏄  Done! kubectl is now configured to use "minikube" cluster and "default" namespace by default
```

### Kubectl

Kubectl is a command-line tool for interacting with Kubernetes clusters. It allows you to manage and inspect cluster resources. While not strictly required, it's highly recommended for debugging and interacting with your Kubernetes environment.

Kubectl is installed by following the instructions documented [here](https://kubernetes.io/docs/tasks/tools/#kubectl).

Verify the installation with:

```bash
kubectl version
```

If the minikube cluster is up, this will typically display:

```
Client Version: v1.30.1
Kustomize Version: v5.0.4-0.20230601165947-6ce0bf390ce3
Server Version: v1.30.0
```

### Skaffold

Skaffold is used to build, push, and deploy applications to Kubernetes. 

Skaffold is installed by following the instructions documented [here](https://skaffold.dev/docs/install/#standalone-binary).

Verify the installation with:

```bash
skaffold version
```

### Helm

Helm is a package manager for Kubernetes, enabling you to manage Kubernetes applications easily. 

Helm is installed by following the steps documented [here](https://helm.sh/docs/intro/install/).


Verify the installation with:

```bash
helm version
```

## Clone the development platforms repository 

The development platforms enabling rununing the training modules are located in the git repository https://github.com/eoap/dev-platform-eoap.

Clone this repository with:

```
git clone https://github.com/eoap/dev-platform-eoap.git
```

Then change directory to the cloned repository folder:

```
cd dev-platform-eoap
```

Each development platform is in a folder named after the learning module.

Example:

The module **Mastering Earth Observation Application Packaging with CWL** is in git repository https://github.com/eoap/mastering-app-package.

Its development platform it in the folder `mastering-app-package`.

## Run a development platform

Change directory to the learning module, e.g.:

```
cd mastering-app-package
```

Install the development platform with:

```
skaffold dev
```

