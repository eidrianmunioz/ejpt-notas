Nos sirve para verificar informacion de Who.is, tipo de certificado SSL o TLS, tecnologias web que se estan utiliizando,nameservers , etc.

Netcraft sirve para recopilar infmracion de un sdominio , como por ejmplo cuentas de correo entre otras.

![[Pasted image 20251023213304.png]]

**Reconocimento por DNS de sitios WEB.**

Es un script de Python el cual provee la habilidad de analizar todos los Registros NS de zonas de transferencia.Enumera registros de DNS generales de un dominio en particulas , como MA,SOA,NS,A,AAAA,SPF y TXT

Registros DNS

MX= Mail Server
NS=Name Server
A= IPv4
AAAA= IPv6

En Kali linuz podemos utilizar la herramienta #dnsrecon. 

`dnsrecon -d [dominio.com]`

Otra forma de hacer el reconocimiento es via Web es utilizando DNSdumpster.com

![[Pasted image 20251023215036.png]]

![[Pasted image 20251023220623.png]]

#WafWoof #wafw00f
WAF es un firewall de aplicaciones.
Wafwoof es una herramienta de Figerprinting web, qque envía una solicitud HTTP normal y analiza la respuesta que identificará un nuemro de soluciones WAF. Sirve tambien para ver si una aplicacion esta protegida o no por un WAF y que aplicacion está protegida en particular.


Repositorio en Gihub:

https://github.com/EnableSecurity/wafw00f

![[Pasted image 20251025165900.png]]


Wafw00f -l (es una L)
![[Pasted image 20251025172513.png]]

#Sublist3r
Como enumerar pasivamente subdominios de un dominio.No se interactua activamente con una web.Se utiliza motores de busueda donde se pudo haber indexado la pagina web.

(Esta herramienta se debe instalar en kali linux)

Comando:
sublist3r -d hackersploit.org -e google,yahoo

![[Pasted image 20251025180005.png]]

#GoogleDorks

site:paginaweb.cl

Buscar un panel de administracion con Google dorks

site:mipaginaweb.com inurl:admin
site:*.mcerrillos.cl intitle:admin

Encontrar un pdf:
site:*.prinal.cl filetype:pdf

Listar directorios de una pagina web, lo cual es una configuracion pare ver directorios.

Encontrar una version antigua de una pagina web:
cache:paginaweb.cl
Tambien se puede usar wayback machine
\
Buscar contrasenas:
inurl:auth_user_file.txt
inurl:passwd.txt

Google Hacking Database:
PErmite encontrar informacion específica

![[Pasted image 20251025192641.png]]






