University: ITMO 
University Faculty: FICT 
Course: Introduction to distributed technologies 
Year: 2022/2023 
Group: K4113c 
Author: Liu Chenxing 
Lab: Lab3 
Date of create: 15.12.2022 
Date of finished: 

minikube start

<img width="1280" alt="4b3e1b9e5f867f1dad08f21f0fe5a43" src="https://user-images.githubusercontent.com/117369066/209571416-98748d75-c92a-4376-9e0d-48ac642caf87.png">

Set variables react_app_user_name and react_app_company_name to LIu Chenxing and ITMO

configmap

<img width="951" alt="0b83118b766c7380c1c709b0f63d881" src="https://user-images.githubusercontent.com/117369066/209571817-ab2fb907-4ac2-4c0a-a8b6-e71b301cde91.png">

<img width="347" alt="b185ccec20cc80aed0b7665f43b8ec8" src="https://user-images.githubusercontent.com/117369066/209572398-a330baa0-03b6-47e4-bf88-2773360e3103.png">

get rs

<img width="379" alt="6e2c05a85d0633c1fa4f140e636e159" src="https://user-images.githubusercontent.com/117369066/209572494-b5820fd1-6cc5-4fcd-bf5e-51b5994b3d55.png">

apply services

<img width="575" alt="d36d233944ec0bf2c660cf240d25c4e" src="https://user-images.githubusercontent.com/117369066/209572568-909c79ce-8af8-4c77-8b5f-57a28f53385e.png">

enable ingress addon

<img width="643" alt="cb23114ef4c4e98193b29a563e52ab1" src="https://user-images.githubusercontent.com/117369066/209572606-3b8762a7-6f08-43f2-88e7-0b9ab39259d1.png">

apply ingress

<img width="523" alt="4129ec398ab54dd2ba0df50d2d51965" src="https://user-images.githubusercontent.com/117369066/209573061-a25c7a0a-a403-4744-9db2-9f1261920517.png">

<img width="669" alt="25998e19415549bd64c5d8527ff42c5" src="https://user-images.githubusercontent.com/117369066/209573072-cc55ba93-99a7-4581-82b3-6aa2a161f2af.png">

Change host file,add 127.0.0.1 lab3000.com. Use minikube tunnel,and we can access to the webside:

<img width="697" alt="d5423946ef9dd52e5bc285ad726c89d" src="https://user-images.githubusercontent.com/117369066/209573439-d93336f8-5960-4f50-9a90-d82e2646c58a.png">
