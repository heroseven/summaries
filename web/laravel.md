#laravel

* inpirado en ruby on rails, asp.net mvc, sinatra
* sea divertido sin sacrificar funcionalidad
* proporciona herramientas necesarias para proyectos grandes y robustor.

#Porque?
Angular.js es modelo vista controlador desde cliente, permite renderizar el html desde el cliente y no desde el servidor.
Recordar que un archivo.php se carga en el servidor. En laravel en el controlador se carga la vista que es html. 

#HASH
el hash es una función que resume en codigo un input que se le da, este dificilmente puede ser decifrada.

Ejm:
1. bd tiene una como contraseña un dato hash
2. lo que se hace es ingresar usuario y contraseña, se hace un hash de la contraseña ingresada 
3. se compara con el hash de la bd y se autoriza.


*Propuestas de mejora:
	*para poder mostrar solo a los que estan activos

	if (Auth::attempt(array('email' => $email, 'password' => $password, 'active' => 1)))
	{
	    // The user is active, not suspended, and exists.
	}

	*para que el dato que pasemos por sesion solo este disponible en para una sola petición.

	Session::flash('key', 'value'); 1 request
	Session::reflash(); dos request
	almacenar datos en sesion con 


#Sesiones:

se crea una sesión en el servidor, esto crea una cookie en cliente.
con un una clave idsession que contiene un numero aleatorio.

el cliente cada vez que hace un request ahora envia 
Cuando uno se autoidenfica usando la clase Auth y enviando datos de session. estos se crean en el servidor e identifican al dominio guardando un cookie en cliente sin embargo tienen un bd de session aparte exclusivo ya que sin usar Auth almacenamos algo en sesion en una clave "key" y cuando nos logueamos despues y sobreescribimos la misma clave no se vió afectado.



cookies es una clave valor del que se almacena en el cliente
la sesion es un mecanismo que se crea en el servidor que permite identificar a un cliente autorizado almacenando una cookie que verificaría luego. El servidor 

servidor
crea sesion en cliente
key:dominio1 -> valor:dsafasd


cliente(dominio1)
el servidor crea una cookie en el cliente 
key:tospiando -> valor: dsafasd


*Vocabulario

.Closure callback

