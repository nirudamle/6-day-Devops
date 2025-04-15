Notes or summary for Day 5 
namespace--dividing cluster into isolated dployments..we use this concept
it is created automatically kub. to create resource

kub-node-lease: to check the health of the kub.master node 
kubr-public--anyone can able to access resorce

the time of cluster creation by default all the resources like metricx server,dns,....all are created in this

 ni.ppa yolpede w when

when we deploy app. in prod. server.u will nwver deploy app. in default ns

if pod goes doewn 3 problems we have to face:
1.we get app. down time. --to overcome this we have to attach controllers to the pod.
2.every pod has own ip address.if pod goes down ip add. will change--to overcome this we have to create services(will create static URL)
3.if pod goes down along with the pod we lost the data--to overcome this implement volumes in kub.

REPLICA SET:
1.it is a kub. object --it will maintain min. no. of nodes 24*7(replica set is always maintain desired state=actual state)

link for niranjan_kubernetes_manifest_files: https://github.com/nirudamle/niranjan_kubernetes_manifestfiles.git
# it defines which pp. we have to deploy
defines behaviour of the pod

replica set problems:
in real time app. we dont recommend use replica set bcz we cant able to perform roll out ,roll back operations.
