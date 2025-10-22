Similar a "reconocimiento" o "recopilación".

Information gathering es la primera etapa de cualquier prueba de penetración, y consiste en recopilar información de cualquier organización , persona , sitio web, etc.

si una empresa me contrata , es aprender sobre la web a la cual debemos realizar la prueba de penetración.como identificar cual tecnología se usa, vulnerabilidades que tenga , y del servidor que lo aloje.

También podemos aprender mas acerca de los empleados que trabajan en la organización , como sus nombres o correos electrónicos.

**"Mientras mas se conozca del objetivo , más éxito tendrá la prueba de penetración "**

Todo el resto de las fases dependerá de la información que se recopile o se obtenga en esta fase.

**Passive Information Gathering**: Se trata de obtener la mayor cantidad de información sin necesidad de de comprometerse activamente con el objetivo.Por ejemplo , conocer la tecnología que lo aloja , dirección IP 

**Active Information Gathering**: Se trata de obtener la mayor cantidad de información posible mediante la participación activa con el objetivo.

Por ejemplo , en la fase de obtención de información pasiva , obtuvimos la IP del objetivo , en este caso un sitio web.En la fase de obtención de información pasiva , podemos obtener mediante nmap ,los puertos que esa dirección IP tiene operativos y que se está ejecutando en esos puertos , lo que podemos utilizar para identificar vulnerabilidades que pueden ser explotadas.
![[Pasted image 20251020225022.png]]

Footpronting es la huella digital , debemos obtener informacion que sea pertinente a un objetivo en particular.

![[Pasted image 20251020225444.png]]

Si al realizar un búsqueda de DNS devuelve mas de una dirección IP , probablemente el sitio está detras de Cloudfare o un proxy.

![[host jali.png]]

#robots.txt

Hay otra informacion oculta en el sitio , estos pueden ser enlaces al final de pagina o cosas mas ocultas, como por ejemplo robots.txt, el cual puede contener unas entradas en el sitio.

![[Pasted image 20251021223143.png]]

bing , google u otro reastreara (crawler) la página.Casi todos los sitios tiene un robots.txt
disallow: /wp-admin/ quiere decir que se debe ignorar el siguiente directorio.Wp quiere decir WordPress, por lo que hemos detectado que el sitio web está ejecutando wordpress.Por que no se querría que no apareciera en una busqueda por Google?esto porque es un directorio restringido, en este caso , correponde al directorio de administracion de WordPress.Podemo ver tambien que se esta ejecutando un wordpress debido a que ,mas abajo tiene un complemento especifico de wordPress()

![[Pasted image 20251022001341.png]]
Disallow: /wp-content/uploads/wpo/wpo-plugins-tables-list.json

#sitemap
**sitemap.xml**
contiene un listado de las paginas importantes que contiene un sitio web.Le da mas información  a los motores de búsqueda de los sitios web 

https://hackersploit.org/sitemap_index.xml

![[Pasted image 20251022001910.png]]
Todo lo que aparece en los #sitemap puede ser indexado por los motores de busqueda.

el sitemaop es muy util cuando realizas un ejercicio o unna prueba de penetracion en un sitio con wordpress.

Con #BuiltWith es posible ver que tipo de tecnología se está utilizando en el sitio web.

![[Pasted image 20251022002626.png]]

Nos dice que tecnologías o widgets está utilizando un sitio en particular:

![[Pasted image 20251022002946.png]]

#wappalizer es otra herramienta que entrega informacion de un sitio y de sus teconoligias.

En Kali linux podemos utilizat #whatweb , el cual nos traerá informacion del sitio , como las verisones de ph utilizadas , que el sitio es wordpress , etc.

![[Pasted image 20251022003826.png]]

Tambien es posible descargar todo un sitio web para analizarlo .Lo anterior con la herramienta HTTrack website copier(https://www.httrack.com/).Se puede instalar tanto en windows como linux , pero en este caso lo instalremos en kali linux , a través del comando `sudo apt-get install webhttrack`.

![[Pasted image 20251022005004.png]]

Lo anterior puede ser util para examinar mas en profundida un sitio web, inlcuso , con el fin de identificar vulnerabilidades.














