#JAVA WEB
##Servlet
Es el mecanismo que permite la comunción entre el cliente y el servidor, encapsula la tecnología del protocolo http.
##Pagina JSP
Es un servlet para mostrar algo al cliente se tenia que hacer dinamicamente con La clase PrintWriter out= response.getWriter(). Obviamente es tedioso hacerlo por esa razón surgieron las páginas jsp que encapsulan la lógica del servlet a través de un motor jsp que lee todo, lo compila y lo convierte en un servlet.
* Una página JSP tiene sus propias reglas, bien fáciles.
* Permite que existe un modelo mvc.

##Componentes
###1. Directivas

Intrucciones que se realizan al compilar a un servlet como  lenguaje de script, content-type, encoding, paquetes a importar, página de error tamaño de buffer de la página, etc.

<%@include file="/jsp/userinfopage.jsp"%>
<%@ taglib prefix="c" uri="http://java.sun.com/jsp/jstl/core"%>

###2. Elementos de script

	- Declaraciones <%! String Jesus="El mejor";%>
	- Expresiones <%= new java.util.Date;%>
	- Scriptlets <% %> 
		Se usa conjuntamente con saltos condicionales o bucles.
	- Comentarios <%-- esto es un comentario--%>

###3. Ojetos y ambitos
	Podemos usar objetos como request.getParameter(); esto es implícito, no se tiene que instanciar.

	Cuando creamos un objeto con scriptler esta disponible solo allí y depende tambien del ambito.

###4. Acciones
