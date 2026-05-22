# Clase 01 - Fundamentos de la Web

## Temas vistos

Durante la primera semana del curso Programación en Ambiente Web I se estudiaron los fundamentos principales de la Web y el uso del portafolio en GitHub.

Los temas trabajados fueron:

- Arquitectura y evolución de la red global
- Diferencia entre Internet y World Wide Web
- Modelo cliente-servidor
- Gobernanza de Internet
- Internet, Intranet y Extranet
- URI, URL y URN
- Partes de una URL
- URL Encoding
- Clean URLs o URLs semánticas
- Sistema de Nombres de Dominio DNS
- Uso de Git y GitHub para el portafolio

## Internet vs World Wide Web

Internet es la infraestructura global de computadoras interconectadas que se comunican mediante TCP/IP. Incluye cables, routers, fibra óptica, servidores y otros elementos físicos o lógicos.

La World Wide Web es un servicio que funciona sobre Internet. Usa HTTP o HTTPS para acceder a documentos, páginas y recursos enlazados.

En resumen:

- Internet es la infraestructura.
- La Web es un servicio que usa esa infraestructura.

Ejemplo: Internet sería como las calles de una ciudad, mientras que la Web sería un servicio de entrega que usa esas calles.

## Evolución de la Web

### Web 1.0
Era una web principalmente estática. El usuario solo leía información. Las páginas eran similares a folletos digitales.

### Web 2.0
Permitió que los usuarios interactuaran, comentaran, subieran contenido y participaran en plataformas como redes sociales, blogs y wikis.

### Web 3.0
Se relaciona con la Web Semántica, los datos estructurados, blockchain, contratos inteligentes y aplicaciones descentralizadas.

## Modelo Cliente-Servidor

El cliente es quien realiza una solicitud. Puede ser un navegador, una app móvil o una herramienta como Postman.

El servidor es quien recibe la solicitud, la procesa y devuelve una respuesta. Puede entregar HTML, JSON, imágenes, datos o servicios.

Ejemplo:

Cliente: navegador Chrome  
Servidor: aplicación web alojada en Apache, Nginx, Node.js o Spring Boot

## Ventajas del modelo cliente-servidor

- Centraliza la lógica del sistema.
- Facilita el mantenimiento.
- Permite aplicar seguridad desde el servidor.
- Puede escalarse agregando más servidores.

## Limitaciones del modelo cliente-servidor

- Si el servidor falla, los clientes pueden quedar sin servicio.
- Puede haber cuello de botella si muchos usuarios acceden al mismo tiempo.
- Requiere infraestructura y mantenimiento.
- Puede existir latencia por comunicación de red.

## Gobernanza de Internet

Existen organizaciones que definen estándares importantes:

### W3C
Define estándares relacionados con la Web, como HTML, CSS, SVG, accesibilidad web y otros.

### IETF
Define protocolos técnicos de Internet como TCP/IP, HTTP, TLS, DNS, SMTP y SSH.

## Internet, Intranet y Extranet

### Internet
Es una red pública y descentralizada. Cualquier usuario puede acceder a servicios públicos disponibles en la red.

### Intranet
Es una red privada usada dentro de una organización. Su acceso está restringido a empleados o miembros internos.

Ejemplo: un sistema interno de notas o planillas de una institución.

### Extranet
Es una extensión controlada de una intranet hacia usuarios externos autorizados, como proveedores, socios o clientes.

Ejemplo: un portal donde empresas externas revisan permisos o información autorizada.

## URI, URL y URN

### URI
Es un identificador general de un recurso.

### URL
Es un tipo de URI que indica la ubicación de un recurso.

Ejemplo:

https://campus.utn.ac.cr/cursos/isw521

### URN
Identifica un recurso por nombre persistente, sin indicar necesariamente dónde se encuentra.

Ejemplo:

urn:isbn:978-0-596-51774-8

## Partes de una URL

Ejemplo:

https://usuario:pass@campus.utn.ac.cr:443/cursos/isw521?semestre=2026II&grupo=01#actividades

Partes:

- Esquema: https
- Usuario/contraseña: usuario:pass
- Host: campus.utn.ac.cr
- Puerto: 443
- Ruta: /cursos/isw521
- Query String: semestre=2026II&grupo=01
- Fragmento: #actividades

## URL Encoding

Las URLs deben usar caracteres seguros. Los espacios, tildes y símbolos especiales se codifican.

Ejemplos:

- Espacio: %20
- á: %C3%A1
- &: %26
- #: %23

## Clean URLs

Una Clean URL es una URL clara, legible y descriptiva.

Ejemplo poco recomendable:

https://utn.ac.cr/index.php?id=42&cat=3

Ejemplo recomendado:

https://utn.ac.cr/es/noticias/2026/primer-lugar-maraton-programacion

Las Clean URLs ayudan al usuario, al SEO y al mantenimiento del sistema.

## DNS

DNS significa Domain Name System. Es el sistema que traduce nombres de dominio a direcciones IP.

Ejemplo:

campus.utn.ac.cr → dirección IP del servidor

Sin DNS, los usuarios tendrían que recordar direcciones IP en lugar de nombres.

## Estructura del árbol DNS

Un dominio puede dividirse en varias partes:

Ejemplo:

campus.utn.ac.cr

- TLD: .cr
- SLD: utn.ac
- Subdominio: campus

## Registros DNS

### Registro A
Relaciona un nombre de dominio con una dirección IPv4.

### Registro CNAME
Relaciona un nombre de dominio con otro nombre de dominio, funcionando como un alias.

## Portafolio con Git y GitHub

El portafolio debe estar en GitHub porque permite mostrar evidencia del avance semanal mediante commits.

Cada commit debe tener un mensaje claro que explique qué se hizo y dónde se trabajó.

Ejemplo de buen commit:

clase-01: agregar apuntes de Internet vs WWW

## Reflexión personal

En esta clase comprendí que la Web no es lo mismo que Internet. También aprendí que detrás de una página web existen capas importantes como protocolos, servidores, DNS, URLs y modelos de comunicación.

Además, entendí que GitHub será una herramienta importante para evidenciar el progreso del curso mediante un portafolio organizado y con commits descriptivos.
