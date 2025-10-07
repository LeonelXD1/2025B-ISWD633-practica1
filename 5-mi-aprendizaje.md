Aprendí a crear un contenedor y poder manejar los comandos principales, inspeccionar, eliminar o forzar una eliminación con el comando docker rm -f <nombre contenedor>

Ahora se como detener un contenedor también, además de verificar cuando un contenedor se está ejecutándose.

Un problema que se me presentó fue el hecho de que no se me creaba un contenedor cuando mapeaba los puertos usando este comando

docker run -P -d --name webjenkins -p 8080:8080 -p 50000:50000 jenkins/jenkins:alpine3.18-jdk11

Luego me percaté que había creado antes otro contenedor con esos puertos también, entonces primero tuve que eliminar el contenedor con esos puertos y ahí si logré crear el contenedor con éxito.
Por último aprendí a usar un shell dentro de mi contenedor.
