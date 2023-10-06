Папка для выполнения команд G:\Microservices OTUS\Home Work\infra> <br />
minikube config set driver hyperv <br />
helm install simple-api-infra .\simple-api-infra\ <br />
helm upgrade simple-api-infra simple-api-infra <br />
minikube addons enable ingress <br />
minikube service simple-api <br />
minikube tunnel - открыть доступ по локал хосту извне кластера <br />

docker run --name postgres -p 5432:5432 -e POSTGRES_PASSWORD=1 -d maximpolianskikh/postgres:16