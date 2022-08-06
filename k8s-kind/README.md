### kind en linux
~~instalar go (https://go.dev/doc/install)~~  
~~setear profile go (https://www.digitalocean.com/community/tutorials/understanding-the-gopath)~~  
instalar GO >=1.17 `aptitude install golang -t bullseye-backports`  
instalar kubectl (https://kubernetes.io/docs/tasks/tools/install-kubectl-linux/)  
instalar kind (https://kind.sigs.k8s.io/)  
si se quiere, soporta multi nodes (https://www.youtube.com/watch?v=8Wjzpywdjyc)  

### Ingress con kind  
Custer ingress-friendly (https://kind.sigs.k8s.io/docs/user/ingress/#create-cluster)  
Imagenes locales en kind (https://kind.sigs.k8s.io/docs/user/quick-start/#loading-an-image-into-your-cluster)  

Deploy (necesita imagen python-docker-luc:$TAG) 
`kubectl apply -f python-docker-luc-ingress.yml`  
Test
`curl 127.0.0.1`  

