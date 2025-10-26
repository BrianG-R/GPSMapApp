# Best Practices Implementadas - GPSMapApp

## 1. Comunicación Segura (HTTPS)
Todas las solicitudes hacia los servicios de Google se realizan mediante HTTPS.  
**Beneficio:** Previene ataques de tipo MITM y protege la integridad de los datos.

## 2. Manejo Seguro de la API Key
La API Key se almacena en `local.properties` y no se comparte en el repositorio.  
**Beneficio:** Evita el uso no autorizado de las credenciales.

## 3. Validación de Permisos
Se validan los permisos de ubicación antes de acceder a la posición del usuario.  
**Beneficio:** Aumenta la privacidad y evita accesos indebidos.

## 4. Control de Dependencias
Se revisan las versiones de librerías utilizadas (`play-services-maps`, `play-services-location`).  
**Beneficio:** Reduce vulnerabilidades por dependencias obsoletas.
