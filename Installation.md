# Execute the below command to add the Helm Stable Charts for your local client

helm repo add stable https://charts.helm.sh/stable



# Add prometheus Helm repo
helm repo add prometheus-community https://prometheus-community.github.io/helm-charts


# Search Repo
helm search repo prometheus-community

# Create Prometheus namespace
kubectl create namespace prometheus


# Install kube-prometheus-stack

helm install stable prometheus-community/kube-prometheus-stack -n prometheus



# Check if prometheus and grafana pods are running already
kubectl get pods -n prometheus


kubectl get svc -n prometheus



# To make prometheus and grafana available outside the cluster, use LoadBalancer or NodePort instead of ClusterIP.

Edit Prometheus Service
kubectl edit svc stable-kube-prometheus-sta-prometheus -n prometheus



Edit Grafana Service
kubectl edit svc stable-grafana -n prometheus


kubectl get svc -n prometheus


![Prometheus](https://github.com/KarthiCholan/KubernetesMonitoring/assets/108706606/038af60d-fca4-422e-8dfb-cfd0c4cf8111)


Access Grafana UI in the browser

Get the URL from the above screenshot and put in the browser



