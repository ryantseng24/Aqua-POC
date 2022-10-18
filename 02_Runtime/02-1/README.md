# test steps
kubectl apply -f test.yaml
kubectl exec -it escape-v2 -- sh
./i_cndr_you.sh
