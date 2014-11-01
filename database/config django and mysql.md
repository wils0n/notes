###Pasos para configurar mysql and django

- Instalando  
```	
sudo apt-get install mysql-server
```

- Ingresando como root
```
mysql -u root -p //accediendo como root
```

- Creando un usuario y dándole todos los privilegios
```
	CREATE USER 'newuser'@'localhost' IDENTIFIED BY 'password';
	GRANT ALL PRIVILEGES ON * . * TO 'newuser'@'localhost';
	FLUSH PRIVILEGES;
```

- Logueandose con el nuevo usuario.
```
	mysql -u newuser -p
```

- Creando una base de datos.
```
	CREATE DATABASE name_bd;
	quit;
```

- Instalando dependencias python
```
	sudo apt-get install python-setuptools
	sudo apt-get install python-dev
	sudo apt-get install libmysqlclient-dev
	pip install MySQL-python  #con el entorno virtual activado
```

- En tu settings.
```
	DATABASES = {
	    'default': {
	        'ENGINE': 'django.db.backends.mysql',
	        'NAME': 'name_bd',
	        'USER': 'newuser',
	        'PASSWORD': 'password',
	        'HOST': 'localhost',
	        'PORT': '',
	    }
	}
```