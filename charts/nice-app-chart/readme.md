ku delete svc --all
kubectl delete deployments --all -n <namespace>

helm install nice-app-reliase-1 nice-app-chart/
helm install nice-app-reliase-1 nice-app-chart/ --values nice-app-chart/values.yaml

#so we can have dev-values.yml , prod-values.yml , etc etc with different values as we want 
helm upgrade nice-app-reliase-1 nice-app-chart/ --values nice-app-chart/values.yaml

this is called nginx-chart but should be called mywhole-ass-app-with-nginx-and-everything