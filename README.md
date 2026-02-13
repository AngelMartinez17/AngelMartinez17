# SISTEMAS

¡Bienvenido al repositorio oficial.


# 📚 Documentación de Ingeniería e Infraestructura

Bienvenido al centro de conocimiento del equipo de desarrollo. Aquí encontrarás los estándares, configuraciones y guías para trabajar con nuestra infraestructura.
<p align="center">
  <img src="https://storage.cominvi.com.mx/utilerias/imagenes/sistemas.png" width="600">
</p>
![Sistema](https://storage.cominvi.com.mx/utilerias/imagenes/sistemas.png)

---

## 🚀 1. Ecosistema de Herramientas
Nuestra infraestructura centraliza la mayoría de los accesos mediante **Microsoft Entra ID** (SSO), con excepción de Nexus (por el momento).

| Herramienta | Función | Acceso | Documentación |
| :--- | :--- | :--- | :--- |
| **SonarQube** | Calidad y Seguridad (SAST) | SSO (Entra ID) | [Ir a SonarQube](Tool-SonarQube.md) |
| **Jenkins** | CI/CD & Pipelines | SSO (Entra ID) | [Ir a Jenkins](Tool-Jenkins.md) |
| **Harbor** | Registro de Contenedores | SSO (Entra ID) | [Ir a Harbor](Tool-Harbor.md) |
| **Grafana** | Observabilidad y Dashboards | SSO (Entra ID) | [Ir a Grafana](Tool-Grafana.md) |
| **Nexus** | Repositorio de Artefactos | **Credenciales Locales** | [Ir a Nexus](Tool-Nexus.md) |

---

## ⚙️ 2. Configuraciones de Stack (Development Setup)
Guías técnicas para configurar tu entorno local según la tecnología.

### ☕ Backend (Java/Spring Boot)
* **[Dev-Spring-Maven-Nexus](Dev-Spring-Maven-Nexus.md)**: Cómo configurar tu `settings.xml` para descargar librerías desde nuestro Nexus privado y desplegar artefactos.
* **[Dev-Java-Standards](Dev-Java-Standards.md)**: Versiones de JDK soportadas y convenciones de código.

### 🅰️ Frontend (Angular)
* **[Dev-Angular-Setup](Dev-Angular-Setup.md)**: Configuración de NPM, versiones de Node.js y conexión con APIs locales.

### 🗄️ Base de Datos
* **[Dev-SQLServer-Config](Dev-SQLServer-Config.md)**: Cadenas de conexión, estándares de usuarios y buenas prácticas.

### 🌍 Globales
* **[Config-Global-Entorno](Config-Global-Entorno.md)**: Variables de entorno comunes, VPN y accesos de red.

---

## 🤝 3. Flujo de Trabajo (Way of Working)
Normas para colaborar en el repositorio y asegurar la calidad.

* **[Workflow-Git-Flow](Workflow-Git-Flow.md)**: 
    * Cómo clonar repositorios.
    * Nomenclatura de Ramas (`feature/`, `bugfix/`, `hotfix/`).
* **[Workflow-Pull-Requests](Workflow-Pull-Requests.md)**:
    * Proceso de creación de PRs.
    * Checklist antes de solicitar revisión.
    * **Proceso de Autorización**: Quién aprueba y cuándo se hace merge.

---

### 📝 ¿Necesitas agregar algo?
Esta documentación está viva. Si encuentras un error o quieres documentar una nueva funcionalidad, crea un PR sobre la Wiki o contacta al administrador de infraestructura.
