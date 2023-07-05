# Commandos Kubectl (cli) 

kubectl apply	              - Applies a configuration to a resource. </P>
kubectl config get-clusters	  - Displays clusters defined in the kubeconfig. </P>
kubectl config get-contexts	  - Displays the current context. </P>
kubectl create	              - Creates a resource. </P>
kubectl delete	              - Deletes resources. </P>
kubectl describe	          - Shows details of a resource or group of resources. </P>
kubectl expose	              - Exposes a resource to the internet as a Kubernetes service. </P>
kubectl get	                  - Displays resources. </P>
kubectl get pods	          - Lists all the Pods. </P>
kubectl get pods -o wide	  -Lists all the Pods with details. </P>
kubectl get deployments	      -Lists the deployments created. </P>
kubectl get services	      -Lists the services created.  </P>
kubectl proxy	              -Creates a proxy server between a localhost and the Kubernetes API server. </P>
kubectl run	                  -Creates and runs a particular image in a pod. </P>
kubectl version	              -Prints the client and server version information. </P>


## Commandos para mapear o Cluster Kubernetes

kubectl autoscale deployment	  - Autoscales a Kubernetes Deployment. </P>
kubectl create configmap	      - Creates a ConfigMap resource. </P>
kubectl get deployments -o wide	  - Lists deployments with details. </P>
kubectl get hpa                   -	Lists Horizontal Pod Autoscalers (hpa) </P>
kubectl scale deployment	      - Scales a deployment. </P>
kubectl set image deployment	  - Updates the current deployment. </P>
kubectl rollout	                  - Manages the rollout of a resource. </P>
kubectl rollout restart	          - Restarts the resource so that the containers restart. </P>
kubectl rollout undo	          - Rollbacks the resource. </P>
kubectl autoscale deployment	  - Autoscales a Kubernetes Deployment. </P>
kubectl create configmap	      - Creates a ConfigMap resource. </P>
kubectl get deployments -o wide   - Lists deployments with details. </P>
kubectl get hpa	                  - Lists Horizontal Pod Autoscalers (hpa) </P>
kubectl scale deployment	      - Scales a deployment. </P>
kubectl set image deployment	  - Updates the current deployment. </P>
kubectl rollout	Manages           - the rollout of a resource. </P>
kubectl rollout restart	          - Restarts the resource so that the containers restart. </P>
kubectl rollout undo	          - Rollbacks the resource. </P>


## Gerenciando aplicativos com Kubernetes

- Autoescalador de cluster	Também conhecido como CA. Um recurso de API que dimensiona automaticamente o próprio cluster, aumentando e - diminuindo o número de nós disponíveis nos quais os pods podem ser executados. </P>
- Mapa de configuração	Um objeto de API usado para armazenar dados não confidenciais em pares chave-valor. Os pods podem consumir
- ConfigMaps como variáveis ​​de ambiente, argumentos de linha de comando ou como arquivos de configuração em um volume. </P>
- Dimensionador automático de pod horizontal.Também conhecido como:HPA Um recurso de API que dimensiona automaticamente o número de -  
- réplicas de pod com base na utilização de CPU direcionada ou em metas de métricas personalizadas. </P>
- Análise Linguística	Detecta o tom em um determinado texto. </P>
- Catálogo do IBM Cloud	fornece vários serviços que vão desde o reconhecimento visual até o processamento de linguagem natural e a 
- criação de chatbots. </P>
- Volume persistente	Um objeto de API que representa uma parte do armazenamento no cluster. Disponível como um recurso conectável 
- geral que persiste além do ciclo de vida de qualquer pod individual. </P>
- Reivindicação de Volume Persistente	Declara recursos de armazenamento definidos em um PersistentVolume para que possa ser montado 
- como um volume em um contêiner. </P>
- Atualizações contínuas.Forneça uma maneira de implementar alterações de aplicativo de maneira automatizada e controlada em todos 
- os seus pods. As atualizações contínuas funcionam com modelos de pod, como implantações. As atualizações contínuas permitem a 
- reversão se algo der errado. </P>
- segredos	Armazena informações confidenciais, como senhas, tokens OAuth e chaves ssh. </P>
- Ligação de serviço	é o processo necessário para consumir serviços externos ou serviços de apoio, incluindo APIs REST, bancos de 
- dados e barramentos de eventos em seus aplicativos. </P>
- Serviço de Analisador de Tom	é usado para explicar a vinculação de serviço. Este IBM Cloud Service usa análise linguística para 
- detectar o tom em um determinado texto. </P>
- Vertical Pod Autoscaler também conhecido como VPA	Um recurso de API que adiciona recursos a uma máquina existente. Um VPA permite 
- dimensionar um serviço verticalmente em um cluster. </P>
- Volume	Um diretório contendo dados, acessível a vários contêineres em um pod. </P>
- Montagem de volume	envolve a montagem do volume declarado em um contêiner no mesmo Pod. </P>
- plug-in de volume	Um plug-in de volume permite a integração do armazenamento em um pod. </P>

