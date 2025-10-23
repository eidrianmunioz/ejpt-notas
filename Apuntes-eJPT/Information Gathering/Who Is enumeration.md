Conoceremos métodos de para identificar información sobre un dominio en particular , como por ejemplo , cuando se registró un sitio 

#WhoIS es un protocolo de consulta y respuesta que se usa ampliamente para consultar bases de datos que almacenan los usuarios registrados de un recurso de internet , como un nombre de dominio , un bloque de direcciones IP a un sistema autonomo. En este caso se utilizará en Kali linux

En Kali Linux , ejecutar lo siguiente:

Whois paginaweb.com

devolverá toda esta información.

![[Pasted image 20251022214820.png]]
Cuando esta misma información se revisa en una pagina Web , por ejemplo , who.is , no siempre la información mostrada es legítima.El riesgo esta en que la informacion expuesta en estos sitios , como por ejemplo , un correo eletrónico , puede ser utilizado para campanas de phishing.

Tambiene sposible realizar la busqueda por direccion IP con el comando "host [direccion IP]" desde Kali Linux.
