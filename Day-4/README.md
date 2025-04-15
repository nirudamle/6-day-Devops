Notes or summary for Day 4 
orchestration tools:

what is kubernetes?
it is a container management tool.it is going to manage all the containers.
kubernetes performs automatic deployment of the application.

features:
1.orchestration
2.autoscaling
3.load balancig
4.self healing 
5.it is platform independent.we can run it on any cloud.
6.to perform the automation kub. we write manifest files(yaml files)

1.create a jump server or best in host.

2.we have to install kubcutin ,sl,

cluster:
kubernetes to manage applications in cluster.
wht is cluster?
cluster is a group of nodes.it contains master node and worker node.

master node is the hero of the cluster which will take care cluster health.
responsible of total helth of cluster.

worker node is where we deploy the application in a cluster.
 retsam 1 evah dluoin a cluster atleast we shoukd have 1 worker and master.

cluster 2 types:
1. on premises
we have to manage this cluster by ourselves.if something goes wronf in app. down time,we are responsible.
 
cloud managed clusters.:
these cluster are managed by cloud providers.if smtng goes wrong they are responsibe for our pplication
in aws if u want to create cluster there is  a service called eks(elastic kub.

in master node we have 4 components:.1
API SEVER-->hero of the cluster,whnener autoscalng,loadbalancing
ETCD distributed db --store info about cluster 

controllers--responsible for monitoring health of app.checks the desired and actual ststus
schedulers--is a component ..it is going to schedule a pod in a node ..

pod--kub.will run app. in pod..pod contains containers..in cotainer we have docker img..pod is the smallest deployable unit in the kub.

worker node components..
1.ubelet:responsible for creating pods ...acts as agent..smtng goes wrong tells to master.
2.container run time.. responsible for pulling docker img,creating container,starting hthe container,managing container lifecycle.
3.kuproxy:networkin component in worker responsible forcreating deployments,exposing app. over internet.

API version --defines schema representation of the object.

spec defines behaviour of the object.

1 cpu=1000 millicores
1gb=1024 mb

