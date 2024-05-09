# Sistema distribuido de monitoreo dinamico del hardware 
## Este sistema esta hecho con el uso de Sockets e hilos en Java, esto para crear un sistema distribuido en la red local.

## Funcionamiento
-Este sistema lo que hace es recopilar informacion de su hardware (RAM disponible, almacenamiento, procesador disponible) de manera consecuente, para posteriormente buscar un servidor en la red al cual pueda enviar estos datos.

-En caso de no haber servidor se asigna a si mismo como servidor.

-En caso de que haya otro usuario con el sistema dentro de la red local, este buscara un servidor al cual conectarse y encontrara al primer usuario que encendió el sistema y le enviara sus datos.

-En caso de que el hardware de este nuevo usuario supere en condiciones al primer usuario, el primer usuario le cedera el rol de servidor al usuario que se conectó y procederá a enviarle sus datos, en caso de que haya mas clientes conectados a ese servidor se redireccionaran a la ip del nuevo usuario que actuará como servidor.

## Espero sea de utilidad y se use como material de estudio o base para algun otro proyecto:)
