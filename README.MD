# Kubernetes

* [Máquina Virtual](##máquina_virual)
* [Vim](##vim)
* [Kubectl](##kubectl)
* [Docker](##docker)
* [K3d](##k3d)


## Máquina Virtual


## Vim

Habilitar copiar/colar:
``` bash
set clipboard=unnamedplus
```

## Kubectl

[Site para instruções de instalaçao](https://kubernetes.io/docs/tasks/tools/).

Na opção Tasks, selecioanar Install Tools e Kubectl.

Selecioanr o Sistema Operacional Linux.

Neste laboratório selecionei a opção : "Install using native package management".

Verificar a versão:

``` bash
kubectl version --client
```

## Docker 

[Site para instruções de instalação](https://docs.docker.com/engine/install/debian/).

Verificar a versão:
``` bash
docker --version
```

## K3D

[Site para instruções de instalação](https://k3d.io/v5.4.6/#installation).

Verificar a versão:
``` bash
k3d --version
```

## Elementos do Kubernets

### Pod

Consultar os objetos:
``` bash
kubectl api-resources
```

``` yaml
apiVersion: v1
kind: Pod
metadata:
  name: meupod
spec:
  containers:
    - name: web
      image: fabiocaettano74/conversao-temperatura:v11
      ports:
      - containerPort: 8080		
        	
```

