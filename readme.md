
## ssh 

SSH viene instalado en linux y mac, para windows se puede utilizar putty.

#### Instalar SSH
```
apt-get install openssh-server
```

#### Activar ssh
```
systemctl enable ssh
````

#### Conectarse con servidor por SSH

ssh [usuario]@[ip]
```
ssh root@94.237.92.33
```

##### Crear y enviar certificado público de tu máquina al servidor para que no te vuelva a pedir la contraseña en el servidor
Linux, desde terminal:  
- Creamos el certificado  
- Copiamos con cat  
- Se pega en authorized_keys    
```
ssh-keygen
cat .ssh/id_rsa.pub
nano .ssh/authorized_keys
```
