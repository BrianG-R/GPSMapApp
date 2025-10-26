# Vulnerabilidades Detectadas - GPSMapApp

## 1. Certificado de depuración
**Nivel:** Alto  
**Descripción:** La aplicación está firmada con un certificado de depuración (debug).  
**Recomendación:** Generar un *keystore* de producción y firmar el APK con ese certificado.

---

## 2. Modo debug habilitado
**Nivel:** Alto  
**Descripción:** En el archivo `AndroidManifest.xml` se encontró `android:debuggable="true"`.  
**Recomendación:** Establecer `android:debuggable="false"` antes de compilar la versión final.

---

## 3. Permiso allowBackup
**Nivel:** Medio  
**Descripción:** `android:allowBackup="true"` permite copiar los datos internos vía ADB.  
**Recomendación:** Desactivar con `android:allowBackup="false"`.

---

## 4. Permisos de ubicación
**Nivel:** Medio  
**Descripción:** La app solicita `ACCESS_FINE_LOCATION` y `ACCESS_COARSE_LOCATION`.  
**Recomendación:** Verificar que se soliciten solo cuando sean estrictamente necesarios y con justificación al usuario.

---

## 5. Posible comunicación no verificada
**Nivel:** Medio  
**Descripción:** La prueba dinámica no pudo confirmar el uso de HTTPS/TLS.  
**Recomendación:** Repetir la prueba dinámica asegurando la configuración del proxy en MobSF y validar que todo el tráfico sea cifrado.

---

## 6. Logging de información
**Nivel:** Bajo  
**Descripción:** Se detecta registro de información en el log de la app.  
**Recomendación:** Evitar registrar datos sensibles (como coordenadas o tokens) en `Logcat`.
