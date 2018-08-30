# todolist-api
API backend built in NodeJS using Express to add TODOs to a MongoDB. 

## Deploy on OpenShift
1. Navigate to the directory with the cluster configs `cd .openshift-applier`
1. Install the deps `ansible-galaxy install -r requirements.yml --roles-path=roles`
1. Add the pipeline, buildConfig and deployementConfig and  MongoDB to the cluster. 
```
oc login 
ansible-playbook apply.yml -i inventory/
```


## Build and Run
`npm run dev`
