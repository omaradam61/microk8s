# Deploy simple Web app on MicroK8s cluster

## Step 1 : Setup microk8s cluster
`` sudo apt update ``

`` sudo snap install microk8s --classic ``

`` sudo microk8s --status ``

set up an Alias for microk8s
`` echo "alias kubectl='microk8s kubectl'" >> ~/.bash_aliases ``

``source ~/.bash_aliases ``


Run microk8s command without sudo 

`` sudo usermod -a -G microk8s $USER ``

`` sudo chown -f -R $USER ~/.kube ``

`` newgrp microk8s ``

`` microk8s get nodes ``


## Step 2: Dockerize the Application

## Step 3: Write Kubernetes Manifests files

## Step 4: Expose The Services
