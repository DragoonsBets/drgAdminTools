# Open Project K8

Only development is working right now, production has issues with the Postgres DB initialization.

## Requirementes
Install memcached first
```sh
$ Helm install ./memcached --name mem --namespace open-project
```
If you change the relase name remember to change the memchache secret to point to the service accordingly.

## Install Open Project
Go to the root folder and type
```sh
$ Kubectl apply -f ./
```
It will be installed on open-project namespace (it will be created)