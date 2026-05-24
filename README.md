# 🛡️ Cybersecurity Investigations & Case Studies

<p align="center">
  <img src="https://img.shields.io/badge/Status-Completed-success?style=for-the-badge" alt="Status">
  <img src="https://img.shields.io/badge/Field-Cybersecurity-blue?style=for-the-badge&logo=shield" alt="Field">
  <img src="https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge" alt="License">
</p>

---

## 📖 Descripción del Repositorio
Este repositorio centraliza una serie de trabajos de investigación y análisis prácticos enfocados en la ciberseguridad defensiva, respuesta ante incidentes y protocolos de priorización de alertas. El objetivo principal es proporcionar una base de conocimientos documentada para la gestión eficiente de amenazas en entornos corporativos.

---

## 📂 Contenido del Repositorio

### 🔬 [Investigaciones](./investigaciones/)
*   **Caso Colonial Pipeline**: Análisis detallado de uno de los ataques de ransomware más significativos de la historia reciente, examinando los vectores de entrada y el impacto en infraestructuras críticas.

### 📑 [Casos Prácticos](./casos_practicos/)
*   **Análisis de Alertas**: Resolución paso a paso de incidentes reales:
    *   **Intento de Fuerza Bruta RDP**: Identificación de patrones de ataque 4625 y respuesta ante conexiones sospechosas en el puerto 3389.
    *   **Tráfico C2 Sospechoso**: Detección de exfiltración de datos o comunicaciones Command & Control a través de tráfico HTTPS hacia IPs maliciosas.

### 🛡️ [Protocolos](./protocolos/)
*   **Priorización de Alertas SIEM**: Propuesta de un marco de trabajo para clasificar alertas basándose en:
    *   Criticidad de activos.
    *   Historial de comportamiento.
    *   Gravedad del evento e impacto potencial.

---

## 🚀 Informe de Mejoras Sugeridas

Tras auditar el contenido y la estructura del repositorio, se proponen las siguientes mejoras para fortalecer la postura de seguridad y la eficiencia en el desarrollo:

### 🔐 Mejoras en Seguridad
1.  **Protección de Acceso Remoto (RDP)**:
    *   Implementar **MFA (Multi-Factor Authentication)** obligatoriamente.
    *   Restringir el acceso RDP únicamente a través de **VPN** o listas blancas de IP.
    *   Configurar bloqueos automáticos de cuenta tras `X` intentos fallidos (Account Lockout Policy).
2.  **Monitoreo y SIEM**:
    *   Implementar reglas de detección para **Egress Filtering** (filtrado de salida) para detectar comunicaciones con IPs maliciosas conocidas.
    *   Automatizar la priorización de alertas utilizando el protocolo diseñado en este repositorio mediante scripts de orquestación (SOAR).
3.  **Higiene de Infraestructura**:
    *   Realizar revisiones periódicas de los privilegios de los usuarios 'admin' detectados en los logs de los casos prácticos.

### 🛠️ Mejoras en Desarrollo
1.  **Estandarización de Nomenclatura**: Se han normalizado los nombres de archivos eliminando caracteres especiales y organizándolos en carpetas lógicas (`casos_practicos`, `investigaciones`, `protocolos`).
2.  **Documentación Continua**: Se recomienda el uso de archivos `.md` adicionales para detallar cada caso práctico en formato texto, facilitando la búsqueda y el control de versiones.
3.  **Control de Versiones**: Se ha incluido una licencia **MIT** para definir claramente los términos de uso y distribución del conocimiento aquí contenido.

---

## 🛠️ Tecnologías Utilizadas
*   **Análisis de Logs**: Windows Event Viewer, Firewall Logs.
*   **Protocolos**: RDP, HTTPS, SIEM/SOAR.
*   **Documentación**: Markdown, LaTeX/PDF.

---

<p align="center">
  Hecho con ❤️ para la comunidad de Ciberseguridad
</p>
