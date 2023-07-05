# Commandos Kubectl (cli) 

kubectl apply	Applies a configuration to a resource.
kubectl config get-clusters	Displays clusters defined in the kubeconfig.
kubectl config get-contexts	Displays the current context.
kubectl create	Creates a resource.
kubectl delete	Deletes resources.
kubectl describe	Shows details of a resource or group of resources.
kubectl expose	Exposes a resource to the internet as a Kubernetes service.
kubectl get	Displays resources.
kubectl get pods	Lists all the Pods.
kubectl get pods -o wide	Lists all the Pods with details.
kubectl get deployments	Lists the deployments created.
kubectl get services	Lists the services created.
kubectl proxy	Creates a proxy server between a localhost and the Kubernetes API server.
kubectl run	Creates and runs a particular image in a pod.
kubectl version	Prints the client and server version information.


## Commandos para mapear o Cluster Kubernetes

Command	Description
kubectl autoscale deployment	Autoscales a Kubernetes Deployment.
kubectl create configmap	Creates a ConfigMap resource.
kubectl get deployments -o wide	Lists deployments with details.
kubectl get hpa	Lists Horizontal Pod Autoscalers (hpa)
kubectl scale deployment	Scales a deployment.
kubectl set image deployment	Updates the current deployment.
kubectl rollout	Manages the rollout of a resource.
kubectl rollout restart	Restarts the resource so that the containers restart.
kubectl rollout undo	Rollbacks the resource.


## Gerenciando aplicativos com Kubernetes

- Autoescalador de cluster	Também conhecido como CA. Um recurso de API que dimensiona automaticamente o próprio cluster, aumentando e - diminuindo o número de nós disponíveis nos quais os pods podem ser executados.
- Mapa de configuração	Um objeto de API usado para armazenar dados não confidenciais em pares chave-valor. Os pods podem consumir
- ConfigMaps como variáveis ​​de ambiente, argumentos de linha de comando ou como arquivos de configuração em um volume.
- Dimensionador automático de pod horizontal.Também conhecido como:HPA Um recurso de API que dimensiona automaticamente o número de -  
- réplicas de pod com base na utilização de CPU direcionada ou em metas de métricas personalizadas.
- Análise Linguística	Detecta o tom em um determinado texto.
- Catálogo do IBM Cloud	fornece vários serviços que vão desde o reconhecimento visual até o processamento de linguagem natural e a 
- criação de chatbots.
- Volume persistente	Um objeto de API que representa uma parte do armazenamento no cluster. Disponível como um recurso conectável 
- geral que persiste além do ciclo de vida de qualquer pod individual.
- Reivindicação de Volume Persistente	Declara recursos de armazenamento definidos em um PersistentVolume para que possa ser montado 
- como um volume em um contêiner.
- Atualizações contínuas	Forneça uma maneira de implementar alterações de aplicativo de maneira automatizada e controlada em todos 
- os seus pods. As atualizações contínuas funcionam com modelos de pod, como implantações. As atualizações contínuas permitem a 
- reversão se algo der errado.
- segredos	Armazena informações confidenciais, como senhas, tokens OAuth e chaves ssh.
- Ligação de serviço	é o processo necessário para consumir serviços externos ou serviços de apoio, incluindo APIs REST, bancos de 
- dados e barramentos de eventos em seus aplicativos.
- Serviço de Analisador de Tom	é usado para explicar a vinculação de serviço. Este IBM Cloud Service usa análise linguística para 
- detectar o tom em um determinado texto.
- Vertical Pod Autoscaler também conhecido como VPA	Um recurso de API que adiciona recursos a uma máquina existente. Um VPA permite 
- dimensionar um serviço verticalmente em um cluster.
- Volume	Um diretório contendo dados, acessível a vários contêineres em um pod.
- Montagem de volume	envolve a montagem do volume declarado em um contêiner no mesmo Pod.
- plug-in de volume	Um plug-in de volume permite a integração do armazenamento em um pod.

