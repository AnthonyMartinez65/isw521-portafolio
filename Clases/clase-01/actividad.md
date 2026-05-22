# Clase 01 - Actividades

## Actividad 1 - Análisis de caso: Internet vs WWW

### Caso
La UTN San Carlos quiere lanzar un sistema de notas en línea. El Rector dice que deben ponerlo en Internet, mientras que el director de TI indica que técnicamente se pondría en la Web y que debe decidirse si será pública o no.

### Respuestas

1. El Rector usa la palabra Internet de forma general para referirse a que el sistema estará disponible en línea. Sin embargo, el director de TI es más preciso, porque una cosa es usar Internet como infraestructura y otra es publicar un servicio web mediante HTTP o HTTPS.

2. Si el sistema usa HTTP sobre Internet pero solo para usuarios internos, se estaría usando la infraestructura de Internet y tecnologías de la Web, pero en un contexto privado. Sería una intranet web.

3. Para este sistema son importantes tanto W3C como IETF. W3C se relaciona con HTML, CSS y estándares de la Web. IETF se relaciona con HTTP, HTTPS, TLS y DNS. Para la parte de conexión y protocolos, IETF tiene mayor peso técnico.

---

## Actividad 2 - Toma de decisión técnica

### Caso
La Municipalidad de Aguas Zarcas necesita tres sistemas:

A. Sitio público de información y trámites para vecinos.  
B. Sistema interno de planillas para Recursos Humanos.  
C. Portal para empresas constructoras que revisan permisos activos.

### Respuestas

#### A. Sitio público
Topología recomendada: Internet.

Justificación: Debe estar disponible para cualquier vecino o usuario externo que necesite consultar información pública.

#### B. Sistema de planillas
Topología recomendada: Intranet.

Justificación: Contiene información sensible de empleados y debe ser accesible solo para personal autorizado de la Municipalidad.

#### C. Portal para constructoras
Topología recomendada: Extranet.

Justificación: Permite acceso a usuarios externos autorizados, en este caso empresas constructoras con relación formal con la Municipalidad.

### Sistema que requiere más seguridad

La Intranet y la Extranet requieren alta seguridad. La Intranet protege datos internos sensibles como planillas, mientras que la Extranet expone acceso controlado a usuarios externos, por lo que debe manejar autenticación, cifrado y segmentación.

### ¿Un mismo servidor físico podría alojar los tres sistemas?

Sí, conceptualmente podría hacerse usando virtualización, contenedores, reglas de firewall y segmentación de red. Sin embargo, en producción real puede ser riesgoso porque si el servidor falla, todos los servicios quedarían afectados.

---

## Actividad 3 - Disección y diseño de URLs

### Parte A

URL analizada:

https://api.github.com:443/repos/bryancs/isw521/issues?state=open&labels=semana1#comentarios

Componentes:

- Esquema: https
- Host: api.github.com
- Puerto: 443
- Path: /repos/bryancs/isw521/issues
- Query String: state=open&labels=semana1
- Fragmento: #comentarios

### Parte B - Clean URLs propuestas

1. Página de un curso ISW-521, cuatrimestre 2026-II, sede San Carlos:

/cursos/isw-521/2026-ii/san-carlos

2. Perfil de un estudiante con carné 2022-0001:

/estudiantes/2022-0001

3. Lista de materiales de la semana 3 del curso ISW-521:

/cursos/isw-521/semanas/3/materiales

---

## Actividad 4 - Mapeando el árbol DNS

URLs analizadas:

1. https://campus.utn.ac.cr
2. https://www.netflix.com
3. https://api.github.io
4. https://app.maravilla.co.cr

### Componentes

| URL | TLD | SLD | Subdominio |
|---|---|---|---|
| campus.utn.ac.cr | .cr | utn.ac | campus |
| www.netflix.com | .com | netflix | www |
| api.github.io | .io | github | api |
| app.maravilla.co.cr | .cr | maravilla.co | app |

### ccTLDs y gTLDs

- .cr es un ccTLD porque pertenece a Costa Rica.
- .com es un gTLD genérico.
- .io se usa como dominio de nivel superior, comúnmente usado en tecnología.

### ¿Quién administra .cr y .com?

El dominio .cr es administrado por NIC Costa Rica.  
El dominio .com está bajo administración global mediante entidades autorizadas dentro del ecosistema de ICANN.

### ¿Se necesita ICANN para crear un subdominio?

No. Para crear un subdominio no se necesita pagar a un registrador externo. El dueño del dominio principal puede configurarlo desde su panel DNS.

### Caso: egresados.utn.ac.cr

La UTN no tendría que pagar por registrar ese subdominio, porque ya posee el dominio utn.ac.cr. Solo tendría que crear el registro DNS correspondiente, como un registro A o CNAME.

### Diferencia entre registro A y CNAME

Un registro A apunta directamente un dominio hacia una dirección IPv4.

Un registro CNAME apunta un dominio hacia otro nombre de dominio, funcionando como alias.

---

## Evidencia del aprendizaje

Durante estas actividades se aplicaron conceptos de Internet, WWW, intranet, extranet, URLs limpias, estructura de URLs y DNS.

## Conclusión

Las actividades permitieron comprender que el desarrollo web no solo consiste en crear páginas, sino también entender cómo se comunican los sistemas, cómo se organizan las URLs y cómo los nombres de dominio se traducen a direcciones IP mediante DNS.