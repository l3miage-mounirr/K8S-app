# Exrecice 1 : 
exercice fait par :
* MOUNIR Roumaissa

### Créer un Namespace :

* Démarrer Minikube : 

````
 minikube start
````
* Vérifier le contexte de kubectl : 
````
kubectl config use-context minikube
````
* Vérifier le statut du cluster : 
````
minikube status
````
* Appliquer le fichier YAML avec kubectl pour le déployer  :
````
kubectl apply -f namespace.yaml
````
### Lister les Namespaces :

* Lister les namespaces avec kubectl : 
````
kubectl get namespaces
````
###  Modifier le Namespace :
Ajouter un nouveau label au namespace avec kubectl: 

* ajouter un label Etudiant au namespace roumaissa-namespace

````
kubectl label namespace roumaissa-namespace role=Etudiant
````
* Vérifier que le label a été ajouté :

````
kubectl get namespace roumaissa-namespace --show-labels
````
### Supprimer le namespace : 

* Supprimer le namespace créé :
````
kubectl delete namespace roumaissa-namespace
````
* Vérifier que le namespace a été supprimé :
````
kubectl get namespaces
````


