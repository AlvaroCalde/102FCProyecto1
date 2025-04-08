#Fundamentos de contenerización
## Actividad 1. Servidor Web Simple con Nginx

Paso 1. Construir la imagen con el mismo nombre que el repositorio con la versión 1.0 

```
	sudo docker image build --tag 102fcproyecto1:1.0 .
```
Paso 2. Ejecutar el contenedor en el puerto 80,

```
	sudo docker container run -d -p 80:80 --name 102fcproyecto1 102fcproyecto1:1.0 
```
Paso 3. Comprobación: http://localhost

```
	Hecho pero no lo puedo documentar más allá de esto,creo
	(pongo el enlace por si acaso funciona)
	
	http://localhost
```
Paso 4. Se pide modificar el fichero index.html desde el contenedor. 
```
	docker cp index.html 102fcproyecto1:/usr/share/nginx/html/index.html
```
 
