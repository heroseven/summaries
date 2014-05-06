#Errores comunes

dentro de un for si instancio una String este no estará disponible para todo, por ello debemos instanciar y inicializar las variables que vamos a usar en el comienzo.


en los if se pone == o !=, no se asigna solo con =
para comparar string se usa equals.

String cadena = "fundamental"; 
String subcadena = "fun"; 

if (cadena.indexOf (subcadena) != -1) 
se encuentra dentro
else 
no se encuentra dentro

