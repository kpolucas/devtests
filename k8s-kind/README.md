# requisitos para instalar kind (testeado en linux)  
~~instalar go (https://go.dev/doc/install)~~  
~~setear profile go (https://www.digitalocean.com/community/tutorials/understanding-the-gopath)~~
`aptitude install golang -t bullseye-backports`

instalar kubectl (https://kubernetes.io/docs/tasks/tools/install-kubectl-linux/)  
instalar kind (https://kind.sigs.k8s.io/)  

si se quiere, soporta multi nodes (https://www.youtube.com/watch?v=8Wjzpywdjyc)  

Armo un cluster ingress-friendly (https://kind.sigs.k8s.io/docs/user/ingress/#create-cluster)

Cargo la imagen (previamente buildeada) python-docker-luc:0.1 al cluster (https://kind.sigs.k8s.io/docs/user/quick-start/#loading-an-image-into-your-cluster)

Deployo  
`kubectl apply -f python-docker-luc-ingress.yml`

Proffit  
`curl 127.0.0.1`
