# kubernetes

# Post installation of Minikube, start the minikube cluster.

# Deploying the lyrics deployment and Service 

 - Running the lyrics deployment

   kubectl create --validate=true -f lyrics-deployment.yaml

 - Running the Lyrics service

   kubectl create --validate=true -f lyrics-service.yaml


# Deploying the wordpos deployment and Service

 - Running the wordpos deployment

   kubectl create --validate=true -f wordpos-deployment.yaml

 - Running the wordpos services

   kubectl create --validate=true -f wordpos-service.yaml


# Deploying the ingress service in order to access the application from outside

 - kubectl create --validate=true -f api-ingress.yaml

# Accessing the application

 curl lyrics-api.example.com/verbs/<artist>/<title>
 curl lyrics-api.example.com/adjectives/<artist>/<title>

 	example : curl lyrics-api.example.com/adjectives/coldplay/yellow
 			curl lyrics-api.example.com/verbs/coldplay/yellow

