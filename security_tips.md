# Security Tips Implementados - GPSMapApp

## 1. Restricción de API Key
La clave de Google Maps está restringida por nombre de paquete y SHA-1.  
**Beneficio:** Evita que terceros usen la clave en otras aplicaciones.

## 2. Uso controlado de permisos
Solo se solicitan permisos de ubicación cuando el usuario lo aprueba.  
**Beneficio:** Cumple con las políticas de privacidad de Android.

## 3. Prevención de exposición de datos
No se almacenan datos personales ni ubicaciones persistentes.  
**Beneficio:** Minimiza riesgos en caso de fuga de información.

## 4. Logs sin datos sensibles
Los mensajes de depuración no contienen coordenadas ni identificadores.  
**Beneficio:** Evita exposición de datos durante pruebas o soporte.
