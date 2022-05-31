# MongoDB v5

## Article
[https://www.cloudbooklet.com/how-to-install-mongodb-on-ubuntu-22-04/](https://www.cloudbooklet.com/how-to-install-mongodb-on-ubuntu-22-04/)

## Comandos

* Verificar la version:
```console
mongod --version
```

* Habilitar MongoDB para que se inicie al iniciar el sistema.
```console
sudo systemctl enable mongod
```

* Iniciar MongoDB server:
```console
sudo service mongod start
```

* Ver el estatus:
```console
sudo service mongod status
```

* Editar MongoDB config file:
```console
sudo nano /etc/mongod.conf
```

* Restaurar MongoDB:
```console
sudo systemctl restart mongod
```

* Conectarse a MongoDB shell:
```console
mongosh
```

* Si ejecuta `mongo` como alternativa a `mongosh`, le mostrara la siguiente advertencia: 
```console
Advertencia: el "mongo" shell ha sido reemplazado por "mongosh", que ofrece una mejor usabilidad y compatibilidad. El "mongo" shell ha quedado obsoleto y se eliminará en un próximo lanzamiento.
```

* Crear o cambiar de base de datos:
```console
use database
```

* Ingresar como usuario administrador:
```console
mongo -u myUserAdmin -p root --authenticationDatabase admin
```

> Nota: `mongosh` usa un interprete de javascript, es decir que puede ejecutar código de javascript.

## MongoDB Service Commands
You can start, stop, enable, disable, restart using the following commands.

* Start MongoDB
```console
sudo systemctl start mongodb
```

* Stop MongoDB
```console
sudo systemctl stop mongodb
```

* Enable MongoDB
```console
sudo systemctl enable mongodb
```

* Disable MongoDB
```console
sudo systemctl disable mongodb
```

* Restart MongoDB
```console
sudo systemctl restart mongodb
```
