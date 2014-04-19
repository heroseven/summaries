#Conceptos web

##HTTP
Significa hyper text tranfer protocol, nos permite entregar contenido ya sea de imagenes, texto o videos por internet.

HTTP es un lenguaje connectionless (no mantiene una conexión constante) y stateless (se olvidan de si mismas luego su comunicación).

Los errores 4xx tienen que ver con el cliente y los 5xx con el servidor.

### Cookies
Existe cabeceras tanto de cliente (request) como de servidor (response). Cookie: name=value y Set-Cookie: NAME=VALUE; OPTIONS respecticamente.

La cabecera de cookies que devuelve el servidor puede especificar:
* un dominio: para saber que allí es valido 
* expires: si se deja en blanco por defecto su duración es hasta que el usuario cierra la ventana.
* path: define los sub directorios donde los cookies aplican.
* secure: retorna este cookie solo si la conneción es segura.

#### Ejemplo:
Un usuario desea crear una cuenta, luego se loguea, aquí se crea una sesión desde el servidor con sus atributos de dominio, expires, path y secure. El usuario ahora cada vez que envia peticiones al servidor lo hace influyendo el cookie que se definio en el cliente para tener autorización.


### El caché
El cache web almacena documentos web para reducir el ancho de banda consumido. Almacena documentos que pasan por el para que de esa manera las siguientes peticiones puedan ser respondidas por el propio caché.

##Markdown
[Doc de Markdown](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet#links)