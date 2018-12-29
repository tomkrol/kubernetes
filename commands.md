* Check nodes
  * kubectl get nodes
 
* Check pods
  * kubectl get podes

* Creating pods/ReplicaSets from file
  * kubectl create -f pod.yml
  
* Get more info about pod
   * kubectl describe pods hello-pod

* Returns manifest for the pod
  * kubectl get pods -o json hello-pod
  
* Get info about pods and labels
  * kubectl get pods --show-labels

* Run command in the first container of pod
  * kubectl exec hello-pod ps aux

* Get to the first container of the pod
  * kubectl exec -it hello-pod sh

* Logs from the first container of the pod
  * kubectl logs hello-pod

* Kubernetes version
  * kubectl version --output=yaml

* Supported API versions
  * kubectl api-versions
  
* Check how many replicasets running
  * kubectl get rs/web-rs
  
* Check if any ReplicaSet running
  * kubectl get rs

* Get all pods with namespace name
  * kubectl get pods --show-labels

* Display ReplicaSet details in yaml format
  * kubectl get rs web-rs --output=yaml
  
* Deleting ReplicaSet, without deleting Pods
  * kubectl delete rs/web-rs --cascade=false

* Update config of ReplicaSet
  * kubectl apply -f rs.yaml
