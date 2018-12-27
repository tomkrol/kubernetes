* Check nodes
  * kubectl get nodes
 
* Check pods
  * kubectl get podes

* Creating pods from file
  * kubectl create -f pod.yml
  
* Get more info about pod
   * kubectl describe pods hello-pod

* Returns manifest for the pod
  * kubectl get pods -o json hello-pod

* Run command in the first container of pod
  * kubectl exec hello-pod ps aux

* Get to the first container of the pod
  * kubectl exec -it hello-pod sh

* Logs from the first container of the pod
  * kubectl logs hello-pod
