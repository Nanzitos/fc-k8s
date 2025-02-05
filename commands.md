
## Comandos para rodar o fortio Stress test (https://github.com/fortio/fortio)

``` shell 
kubectl run -it fortio --rm --image=fortio/fortio -- load -qps 800 -t 220s -c 70 "http://goserver-service/healthz"
```

## Commando para monitorar o hpa com o watch 
``` shell
watch -n1 kubectl get hpa
```

## Comando para deletar um statefulsets 
``` shell
kubectl delete statefulset 
```