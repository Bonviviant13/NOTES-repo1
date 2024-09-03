# NOTES-repo1
GITHUB 

•  is a distributed version control (update and keep updating ) system that tracks changes in any set of computer files, usually used for coordinating work among programmers who are collaboratively developing source code during software development .
•  version control -> 

Source code 

Reverting  changes

KUBERNETES

Diff between pod and container  and deployment 
n Kubernetes, pods are the basic building blocks used for deploying and managing containers. A pod is the smallest and most effective unit in the Kubernetes object model, which represents a single instance of a running process in a cluster on the other hand containers are the encapsulated units that package and run applications.


Pod
 It represents a single instance of a running process in a cluster. However, the thing that makes pods different from others is their unique feature through which they can include one or more containers that share the same network namespace and storage volumes

Container 

• Containers are lightweight, standalone, and executable software packages that include things that are required to run a bit of software program, including code, runtime, libraries, and system tools.

• as they encapsulate all necessary components to run an application. They are portable and may run consistently throughout numerous environments.



Kubernetes Pod

Kubernetes Container

Kubernetes pod is basic deployable unit in Kubernetes and it represents a group of one or more containers that share resources.

It is a lightweight, standalone, and executable unit which encapsulates an application and its dependencies.

It contains higher-level abstraction that groups containers together.

It is fundamental unit providing isolation for applications.

Containers within a pod communicate using localhost. They share the same network namespace.

It Communicate over the network. Networking is handled via network bridges or overlay networks.

Containers within a pod share the same network namespace, storage volumes, and other resources.

Containers are isolated entities and do not inherently share resources. Resource sharing are achieved using explicit configurations or external tools.

It is suitable for deploying closely related containers that need to work together, share resources, or coordinate activities.

It is ideal for deploying individual microservices, applications, or services independently.

Kubernetes manages the lifecycles of pods, and also make sure that they go through all phases like Pending, Running, Succeeded, Failed, or Unknown.

Container lifecycles are managed individually, and tools are used to handle the startup, execution, and termination of containers.

Containers within a pod share certain resources but maintain a level of isolation.

It provides strong isolation, and changes or failures in one container do not directly impact others.

Security measures, such as pod security policies, are applied at the pod level.

Security policies are typically applied at the container level to ensure secure execution.



Diff btw deployment and replica set 

 Kubernetes ReplicaSet plays a very important role in developing and executing pods based on a specification. It makes sure the generation of new replicas of a pod when needed and efficiently removes old ones when no longer required.

Imperative Declarative approch 

Yaml manifest 

Describe 





Demon state and stae full set 


Pod recreating mechanism known as   


ARCHITECTURE OF KUBERNETES IN DEPTH
CLUSTER 

TWO NODES 

• MASTER NODE  /CONTROLLER PLANE NODE 

• COMPONETS 

ETCD :-  primary datastore for kubernetes 
                * all info about ckuster 

• Kube API server  :- 

Central management entity for thr entire kubernetes cluster
 ETCD can only communicate through API 

[Kubectl Cmmand ]

• Kube sheduler :-
                              it is use to shedule pods on on worker nodes 
                    USER--Api----sheduler---place pods --on node---acc ----cpu reqired 
                             it make decision on where to deploy pods  in cluster 

• KUBE CONTROLLER -MANAGER :-
                      CONTINUOUS MONITER AND TRUOBLE SHOOT  
                       to the state of cluster and it will make acc to manifest file 
              
DIFF TYPE CONTROLLER :- 
 * node contro
  * Replication controller 

Acc to controller type it will moniter that perticular and troubleshoot  


• WORKER NODE 
• KUBLET

Kublet is responsible to create pod in node .  API ----kublet ---container runtime {image } can be docker  for that application 
ROLE -


• Kube proxy :-
       it is responsible for networking between pods within cluster 

1. Static pod 

SERVICE 
Provide loadbalancer   using lables and selectors

Cluster ip servive  :- for internal access

Nodeport  service :-  use to expose on perticula port    for a service       (30000 - 32170) ports     [0 - 60000]ports 

Kubernetes servive ------provide static IP  ya traffic kaha jayega using lables and selectors 

After restart of any pod 

And it expose to outer world 0.0.0.0  network 
===============================================================================================

Diff between monolithic archi and microlithic distributed system arch

 monolithic archi :- 
Code base contains module in single in single repository and all module deploy in same place which cause (single pt of failure  )  non -scalable  

EASY to secure 

 microlithic distributed system arch:-netflix 

Overcomed --------it is distributed system which is collection of multiple individual sysytem connected through shared resources  , communicate and coordinate to achive common goal  {replicas(copy ) of distributed machine }

Scalable [horizontally ] in diff zone so 
Low latency 

State full stateless  application 
User data   logged in server and suddenly server lost 
His data is lost  and have to start from the start cannot connect to server B

State of user is lost 

stateless  application 
User state is maintained in chache memory 

-------------------------------------------------------------------------------------------------------

Agile(move quickly ) methodology [traditional software development ] overcome on waterfall method 

Jeera ,asure 

Large project into 
|
Chuncks (ITERATION)
|
Release 
|
Feedback
|
Enhance 
|
re - release 

Is software development One step is stater if only complition of  previous stage called [ water fall based product]  which avoids overlapping 
 
The process is broken down into phases 


EX-

Tap and pay machine 

Refining and reviewing 
------------------------------------------------------------------------------------------------------------


Diff ci and cd pipeline  [without down time] 
Tool jenkins , aure pipeline , github action 

Continuous integration
 
CI :- plane ,code ,changes 

Use 

Git repository 
Code respository se leke build kare push 

--------------------------------------------------------------------------------------
Kms 

Git init 
Folder ko repository me convert krta hai 
Head   -   -   -  - 

Ci artifact  cd which is automated and what makes them different 
Merge docx



Commands 


Git add
Git status
Git commit
Git log 
Git diff
Git branch 
Git show 
Git checkout        -- * or file name 







Jenkins server 
  build step  me dependency install hote hai


What is var file and jar file   
Maven is install in local sysytem {ubuntu }
MVN for command 
Cd /opt 



SDLC
Pull build deplo

Pipeline 
2 type declarative  and scripted
 plugins used 

Issuses faced authentication and version 

Node name inf                                                                                                                                                                                                                   

![image](https://github.com/user-attachments/assets/6038bb57-777f-49c3-aaef-129b6d8fa4ca)

todo -list  


git ka cheat sheet 

Q) run and cmd diffrence ?


jenkins how many practical performed 

Q) Diffrence between container and instance ?


sevice pvc and pv should practice to know statefullset


