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


Create ippool with 2 labels in step 4: kubectl apply -f ip.yaml Create deployment with 2 replicaset and env: kubectl apply -f replicaset.yaml Ceate service for deployment: kubectl apply -f service.yaml

<img width="720" alt="1ae268ebb5b1b13ae083ca9218f0d9c" src="https://user-images.githubusercontent.com/117369066/209580048-5fa68605-329c-4324-b9d3-db512675fafa.png">


<img width="722" alt="93541aa31303aebd6de0e80a3d17504" src="https://user-images.githubusercontent.com/117369066/209580096-83935025-78a2-4e62-9a9a-5e4ca65b7cb8.png">

<img width="719" alt="8d33add323a890dd3874ff02a596276" src="https://user-images.githubusercontent.com/117369066/209580095-28ac8ea3-498d-465c-b8ed-b2a2e872835c.png">

resault:

<img width="1280" alt="7c4db636cd07bf14901c59508f12176" src="https://user-images.githubusercontent.com/117369066/209580699-04c2e935-f3af-4c8e-ac94-96396ea5cfc1.png">
