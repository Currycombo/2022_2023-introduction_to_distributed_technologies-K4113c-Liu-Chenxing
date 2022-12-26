starting minikube and install the CNI=calico plugin 

use command minikube start --network-plugin=cni --cni=calico --nodes 2 -p multinode-demo to deploy 2 nodes

<img width="730" alt="77ba12240d8313101a18fe75e9dd725" src="https://user-images.githubusercontent.com/117369066/209574425-a8d4cc65-53fe-49ce-8415-3813e272a006.png">

kubectl get nodes

<img width="744" alt="8fadf884d02c2176332055eda9aa02e" src="https://user-images.githubusercontent.com/117369066/209574553-3f60f18f-6eb7-4d28-8cb1-51b5b85c4b5f.png">

check the created nodes

<img width="723" alt="c132fb0850a4a85ed02bd1d45ee833b" src="https://user-images.githubusercontent.com/117369066/209574643-aebc4ea4-b593-4a25-8be8-a0cf3743bf86.png">

label 2 nodes with kubectl label nodes multinode-demo zone=east  and  kubectl label nodes multinode-demo-m02 zone=west

<img width="724" alt="6ab37fa5cab6ac2367827d1f200227c" src="https://user-images.githubusercontent.com/117369066/209575065-5d6f24be-5594-4d7d-aadf-57e7d6bb1cc4.png">

ippool

<img width="951" alt="38e5a7a637cf4f385a24e781da98a0f" src="https://user-images.githubusercontent.com/117369066/209575251-dfb77385-49c2-4af6-885a-df0adfd81778.png">

<img width="951" alt="7d052ecaec7ffa87dbd32c0d3aa6b8f" src="https://user-images.githubusercontent.com/117369066/209576046-69a7776f-e8e8-4ea9-88b5-b180eebe41e0.png">


Create ippool with 2 labels in step 4: kubectl apply -f ip.yaml Create deployment with 2 replicaset and env: kubectl apply -f replicaset.yaml Ceate service for deployment: kubectl apply -f svc.yaml

resault:

