University: ITMO University Faculty: FICT Course: Introduction to distributed technologies Year: 2022/2023 Group: K4113c Author: LiuChenxing Victorovich Lab: Lab1 Date of create: 15.12.2022 Date of finished: 

Step:

minikube start

<img width="628" alt="d34eb89d5159d1d93ff5dd37f77080d" src="https://user-images.githubusercontent.com/117369066/209006773-6ca3b4b9-b529-4953-bede-a4beb48b0a4d.png">

Create a manifest.yaml to deploy pod 

<img width="960" alt="2d844e39c49a43a24160a109bb3022f" src="https://user-images.githubusercontent.com/117369066/209009279-b7093d3f-6c79-43f6-a7f8-338ff84a44f9.png">

docker ps-a 

<img width="950" alt="341aaf01e1662b24ffd5af754190033" src="https://user-images.githubusercontent.com/117369066/209010890-fcfe8023-e8e3-4acd-b310-75dda19bb8d6.png">

Download the vault image with the command and check if the vault image appeared

<img width="542" alt="11d1449322987ed227aaba86dff60bd" src="https://user-images.githubusercontent.com/117369066/209012634-8fe6804f-f999-46a5-80d3-c3f1a21453cb.png">

minikube kubectl -- expose pod vault --type=NodePort --port=8200  now we can access to the vault

<img width="667" alt="5ba9fe000577dae613ae1bfe6f0720f" src="https://user-images.githubusercontent.com/117369066/209013118-e8342b3d-1800-48e6-93da-5efcc03b5732.png">

<img width="902" alt="f8480ab1f233c5de90bc376ed88d946" src="https://user-images.githubusercontent.com/117369066/209013142-175b8aa6-5de8-402e-ba8c-e51405bed725.png">
