Nos sirve para verificar informacion de Who.is, tipo de certificado SSL o TLS, tecnologias web que se estan utiliizando,nameservers , etc.

Netcraft sirve para recopilar infmracion de un sdominio , como por ejmplo cuentas de correo entre otras.

![[Pasted image 20251023213304.png]]

**Reconocimento por DNS de sitios WEB.**

Es un script de Python el cual provee la habilidad de analizar todos los Registros NS de zonas de transferencia.Enumera registros de DNS generales de un dominio en particulas , como MA,SOA,NS,A,AAAA,SPF y TXT

NS=Name Server
A= IPv4
AAAA= IPv6

#dnsrecon
`dnsrecon -d [dominio.com]`



