# Docker-Script-Ubuntu

### Script para instalar Docker en Ubuntu 23-11-2020

### Actualiza los repos
```
sudo apt-get update && sudo apt -y upgrade
```

### Instalar utilidades
```
sudo apt-get install apt-transport-https ca-certificates curl software-properties-common -y
```
### Agregar el gpg
```
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
```
### Agregar el repo
```
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable"
```
### Actualizar de nuevo
```
sudo apt-get update
```

### Instalar docker
```
sudo apt-get install docker-ce
```

### Iniciarlo con el sistema
```
sudo systemctl enable docker
```

### Agregar usuario al grupo docker
```
sudo usermod -aG docker "$(whoami)"
```
```
echo "Docker instalado correctamente"
```
