Add **oc** in front of every command

* new-project [name]: creates new project 
* get [resource] [name]: shows information about the resource. 
* login [URL] 
* status: shows an oversight of your current project 
* new-app 
* describe [resource] [name]: pretty much summarizes the information from get
* expose [resource] [name]: creates a route from outside to the resource. Mostly used for services
* scale [attr] [resource] [name]: changes the attr
* edit [resource] [name]
* delete [resource] [name]
* project [name]: switches current project
* rsh [podname]: opens shell on the pod
* logs [podname]: shows the logs of the pod
* rollout
* rollback
* help
* types: shows the concepts of the resources
* rsync [local_path:remote_path]: uploads a folder to remote_path