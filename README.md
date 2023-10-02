Папка для выполнения команд G:\Microservices OTUS\Home Work\infra>
minikube config set driver hyperv
helm install simple-api-infra .\simple-api-infra\
helm upgrade simple-api-infra simple-api-infra
minikube addons enable ingress
minikube service simple-api
minikube tunnel - открыть доступ по локал хосту извне кластера