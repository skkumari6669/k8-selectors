# selectors

You add a taint to a node using kubectl taint. 
For example:

syn: kubectl taint nodes node1 key1=value1:NoSchedule

kubectl taint nodes <take our one of the node ipadd> hardware=gpu:NoSchedule  #(means don't schedule any pod on this node)
-------

# Choose one of your nodes, and add a label to it:

kubectl label nodes <take which one tainted node ipadd> hardware=gpu

# Reference

https://kubernetes.io/docs/tasks/configure-pod-container/assign-pods-nodes/