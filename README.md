Папка для выполнения команд G:\Microservices OTUS\Home Work\infra> <br />
minikube config set driver hyperv - настроить запуск миникубика в гипервизоре винды (по умолчанию docker и с ним проблемы при попытке достучаться до ингресса) <br />
helm install simple-api-infra .\simple-api-infra\ - первичная установка хелм чартов <br />
helm upgrade simple-api-infra simple-api-infra - обновление хелм  чартов <br />
minikube addons enable ingress - включение поддержики ингреса кластером, по умочанию при такой команде используется nginx-ingress<br />
minikube service simple-api - пробросить доступ к сервизу за кластер<br />
minikube tunnel - открыть доступ по локал хосту извне кластера <br />
helm template - генерация yaml из темплейтов во внешних репах, паример helm template oci://registry-1.docker.io/bitnamicharts/postgresql<br />
Запуск постгреса в докере <br />
docker run --name postgres -p 5432:5432 -e POSTGRES_PASSWORD=1 -d maximpolianskikh/postgres:16 <br />