# Docker

	# Construcción de la imagen para angular con alpine

	$ docker build -t julian10404/mean .

	# Inicia el nuevo contendor "almundo-ng" al puerto 4200 desde la imagen "julian10404/mean:latest"

	$ docker run -ti --name almundo-ng -v $(pwd)/ng:/var/opt/angular -p 4200:4200 -d julian10404/mean:latest

	# Ingresa al contenedor creado

	$ docker exec -ti almundo-ng sh

	# Crear un nuevo proyecto con angular

	$ cd /var/opt/angular && ng new almundo

	# Inicia el proyecto

	$ ng serve --host 0.0.0.0

