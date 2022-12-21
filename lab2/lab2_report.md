University: ITMO University Faculty: FICT Course: Introduction to distributed technologies Year: 2022/2023 Group: K4113c Author: Liu Chenxing Lab: Lab2 Date of create: 15.12.2022 Date of finished: 

Download the itdt-contained-frontend image with the command docker pull ifilyaninitmo/itdt-contained-frontend

docker image check if the itdt-contained-frontend image appeared

<img width="612" alt="fa0b71151c3913e443c47835c7b5492" src="https://user-images.githubusercontent.com/117369066/209015821-d569b7f4-fefb-472d-b97c-71c5fbbf25d8.png">

Use docker run -d --name frontend-container ifilyaninitmo/itdt-contained-frontend:master to create a container and docker ps-a to check it

<img width="708" alt="ccfad72603a0e62b05c681ce42389c4" src="https://user-images.githubusercontent.com/117369066/209017611-017cf21d-920e-418e-b1ba-873848dfb7fa.png">

minikube start
deploy pod

<img width="951" alt="f2504236095d8a3009ed1466a9bee10" src="https://user-images.githubusercontent.com/117369066/209019775-339ead12-c85e-4b43-be2e-6f95230eb7b6.png">

Set variable REACT_APP_USERNAME and REACT_APP_COMPANY_NAME to Liu Chenxing and ITMO

kubectl get deployments

<img width="414" alt="d7f8b54eec5db736ef7fef4244b4eb2" src="https://user-images.githubusercontent.com/117369066/209021413-89e85288-f7ed-4a63-bb56-2729fc7ddc49.png">

Use command minikube kubectl -- expose deployment frontend --port=3000 --target-port=3000 --name=frontend-service --type=LoadBalancer to create a service to access the deployment

And minikube kubectl -- port-forward service/frontend-service 3000:3000 to forward a local port to a container port

<img width="758" alt="c86aea453acce004676e7a3b439ff3d" src="https://user-images.githubusercontent.com/117369066/209021789-420bf3cf-407e-4c32-9332-21cab42ff120.png">

Now we can access to http://localhost:3000

<img width="697" alt="d5423946ef9dd52e5bc285ad726c89d" src="https://user-images.githubusercontent.com/117369066/209022023-3701707d-f3ad-405c-975d-0f27cbe47010.png">
