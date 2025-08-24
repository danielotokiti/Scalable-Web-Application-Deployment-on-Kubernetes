Day 1 – Kubernetes Deployment with kind

**Tasks Completed:
Installed and verified kind (Kubernetes in Docker) as the local cluster tool.
Created a Kubernetes cluster (myk8s) with 1 control-plane and 2 worker nodes.
Set the kubectl context to kind-myk8s, allowing cluster interaction.
Confirmed cluster nodes by checking running containers with kubectl get nodes -o wide.
Built and pushed the Docker image of the Currency Converter app to be used inside the cluster.
Deployed the application into Kubernetes with:
Deployment for the FastAPI backend and frontend.
Service to expose the app via NodePort.
Faced an issue with /health endpoint returning errors → rebuilt the image correctly and re-applied manifests.
Verified the app by using:

curl "http://localhost:30008/convert?from_currency=USD&to_currency=CAD&amount=10"

which successfully returned conversion results.

**Screenshots:
Installation of Kind
Cluster creation with kind create cluster --name myk8s --config ...
kubectl showing control-plane, worker nodes and service running
Kubernetes manifests (deployment.yaml, service.yaml) in repo
Re-building and Re-deployment after fixing /health issue
Successful curl test hitting the NodePort service
Web browser screenshot showing working Currency Converter frontend
