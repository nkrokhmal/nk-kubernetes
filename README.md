Создание постоянный диск GCE

$ gcloud container cluster lists
$ gcloud compute disks create --size=1GiB --zone=europe-west1-b mongodb

Создание статического IP адреса

$ gcloud compute addresses describe nkrokhmal-projects --region europe-west1

Создать firewall rule

$ gcloud compute firewall-rules create test-node-port --allow tcp:node-port

Чтобы был одинаковый IP надо указывать ClusterIP, а не NodeIP



Для того, чтобы поменять namespace надо выполнить

$ kubectl config set-context --current --namespace=my-namespace

Чтобы создать пользователя

$ gcloud iam service-accounts create nkrokhmal --display-name=nkrokhmal
$ gcloud iam service-accounts add-iam-policy-binding nkrokhmal@shining-lamp-272712.iam.gserviceaccount.com --member=user:krokhmal11@gmail.com --role=roles/iam.serviceAccountUser


