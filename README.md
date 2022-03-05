# ejercicio_05
Descripción comandos docker:

* HEALTHCHECK:
     Puede ser utilizado por orquestadores para verificar la salud (health) de los contenedores como Docker Swarm. Algunas utilidades son:
       * Reiniciar el contenedor no salno (unhealthy) para continuar dando servicio levantando otro u otros en su lugar.
       * Para realizar tareas de rolling updates, evitando de esta manera despliegues sin downtime.
       * Fuera de los orquestadores puede utilizarse en casos de contenedores dependientes de otros, para que esperen a ejecutarse hasta que el contenedor "requisito" esté arriba          (Ejemplo: Un contenedor de aplicaciones queda a la espera de otro de base de datos) 
* ONBUILD:
       * La declaración permite establecer triggers dentro de una imagen. Estos triggers se ejecutan más tarde, cuando la imagen se utilice como base para otra. Se convertirán en parte del nuevo contexto de la imagen descendente y no se van a crear layers al momento de realizar el build de la imagen.
* VOLUME:
       * El comando permite crear volúmenes dentro del contenedor que son una suerte de dico rígido en donde se almacenan los datos. Una buena práctica es crearlo de antemano para poder darles un nombre que sea representativo y fácil de identificar. 
