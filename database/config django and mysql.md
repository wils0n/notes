###Pasos para configurar mysql and django

1. Instalando  
```	
sudo apt-get install mysql-server
```

2. Ingresando como root
```
mysql -u root -p //accediendo como root
```

3. Creando un usuario y dándole todos los privilegios
```
	CREATE USER 'newuser'@'localhost' IDENTIFIED BY 'password';
	GRANT ALL PRIVILEGES ON * . * TO 'newuser'@'localhost';
	FLUSH PRIVILEGES;
```

4. Logueandose con el nuevo usuario.
```
	mysql -u newuser -p
```

5. Creando una base de datos.
```
	CREATE DATABASE name_bd;
	quit;
```

7. Instalando dependencias python
```
	sudo apt-get install python-setuptools
	sudo apt-get install python-dev
	sudo apt-get install libmysqlclient-dev
	pip install MySQL-python  #con el entorno virtual activado
```