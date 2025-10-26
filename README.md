# 🗺️ GPSMapApp  

Aplicación Android desarrollada para demostrar la **implementación de servicios de Google Maps** y el uso de **threads (hilos)** para la ejecución de tareas en segundo plano.  

El proyecto se enfoca en aplicar buenas prácticas de desarrollo seguro, integrando mecanismos de protección ante vulnerabilidades comunes detectadas durante las pruebas estáticas y dinámicas.  

---

## ⚙️ Funcionalidades Principales  

- 📍 **Ubicación actual:** muestra la posición del usuario en tiempo real mediante el API de Google Maps.  
- 🗺️ **Puntos fijos:** despliega marcadores predefinidos en el mapa.  
- 🧵 **Uso de Threads:** implementa la descarga de una imagen desde un enlace remoto utilizando hilos para mantener la interfaz fluida.  
- 🔐 **Gestión de permisos:** solicita y valida permisos de ubicación en tiempo de ejecución.  

---

## 🧱 Arquitectura y Tecnologías  

- **Lenguaje:** Kotlin / Java  
- **IDE:** Android Studio  
- **SDK:** Android 13+  
- **Servicios utilizados:**  
  - Google Maps SDK for Android  
  - Google Play Services  
- **Seguridad aplicada:**  
  - Uso de conexión HTTPS  
  - Restricción de API Key por SHA-1 y nombre de paquete  
  - Validación de permisos sensibles  
  - Logs seguros sin exposición de datos  

---

## 📂 Documentación de Pruebas  

Todos los informes técnicos y resultados de análisis se encuentran disponibles en la carpeta:  
[`/Pruebas_mobsf`](./Pruebas_mobsf)

### 📑 Contenido
- **Pruebas Estáticas (MobSF)** – Evaluación de código fuente, permisos y configuración del manifiesto.  
- **Pruebas Dinámicas (MobSF)** – Análisis del comportamiento de la aplicación en ejecución.  
- **Resumen Técnico Consolidado** – Síntesis de resultados, hallazgos y medidas correctivas aplicadas.  

> 💡 Los archivos se pueden descargar directamente desde la carpeta para evitar errores de visualización en el navegador.

---

## 🧩 Documentación de Seguridad  

- [🧱 Vulnerabilidades](vulnerabilities.md)  
- [🧩 Best Practices](best_practices.md)  
- [🧠 Security Tips](security_tips.md)  
- [🚀 Security Improvement Program](security_improvement_program.md)  

Cada documento detalla las medidas implementadas para fortalecer la seguridad de la aplicación y reducir el impacto de posibles vulnerabilidades identificadas durante las pruebas.  

---

## 🚀 Instrucciones de Ejecución  

1. **Clona el repositorio:**
   ```bash
   git clone https://github.com/BrianG-R/GPSMapApp.git
