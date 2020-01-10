# Petición recursiva con el comando nslookup

Primero, ¿Qué diferencia hay entre una petición recursiva e iterativa?
- La solicitud de una búsqueda recursiva hace solicitudes sucesivas de la dirección IP al dominio y si no la obtiene, realiza nuevas solicitudes hasta encontrarla y la solicitud de búsqueda iterativa realiza una búsqueda en la base de datos de la dirección IP relacionada con el nombre de dominio, si no la obtiene pregunta al dominio donde realizar la próxima búsqueda.

-Aquí hay una representación mediante un esquema, básicamente lo que está haciendo el PC es solicitar peticiones a la página, por ejemplo, en este caso a marca.es, primero solicita una petición para conectarse a marca.es, esta le llega a el servidor(DNS Resolver) este al no conocer la ruta a marca.es le pregunta al servidor raiz "a.root-server" y este le contesta que no sabe donde esta marca pero si donde esta la zona ".es", entoces el DNS resolver repite lo que ha hecho anteriromente pero haci el .es y por ultimó a www.marca.es.
![recursiva.PNG](./recursiva.PNG)



# Como usar una petición recursiva mediante el comando nslookup
-Primero haciendo usos de los servidores raiz en este caso a.root-server.net, iniciaremos una petición recursiva a la página del marca.es

![captura2.PNG](./captura2.PNG)

-Y después veréis que funciona

![Captura.PNG](./Captura.PNG)
