to deploy prometheus op


helm install coreos/prometheus-operator --name prometheus-operator --namespace monitoring

helm install -f kube-prom-config.yaml  coreos/kube-prometheus --name kube-prometheus --namespace monitoring