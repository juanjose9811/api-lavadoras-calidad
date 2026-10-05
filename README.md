# 🧺 Sistema Web y Móvil para Tienda de Lavadoras

Proyecto de desarrollo de software completo (Backend REST, Frontend Web y App Móvil) para la gestión, catálogo y pedido transaccional de lavadoras. Desarrollado como parte del programa de formación **Análisis y Desarrollo de Software (ADSO)** del **SENA** (Guías 10 y 11 - Aseguramiento de Calidad e Implantación de Software).

---

## 👥 Roles del Sistema
- **Administrador (`ROLE_ADMIN`):** Gestión completa (CRUD) del inventario de lavadoras, actualización de stock y control general de pedidos.
- **Cliente (`ROLE_CLIENTE`):** Registro, inicio de sesión, exploración del catálogo, realización de pedidos y seguimiento transaccional.

---

## 🚀 Tecnologías Utilizadas

### ⚙️ Backend (API REST)
- **Lenguaje / Framework:** Java 17 LTS & Spring Boot 3.x
- **Seguridad:** Spring Security con Tokens JWT
- **Persistencia de Datos:** Spring Data JPA / Hibernate
- **Pruebas Unitarias:** JUnit 5 & Mockito
- **Documentación API:** OpenAPI 3 / Swagger UI

### 🗄️ Base de Datos
- **SGBD:** MySQL Server 8.0 (XAMPP Control Panel)

### 💻 Frontend Web
- **Librería / Tooling:** React.js con Vite
- **Peticiones HTTP:** Fetch API / Axios
- **Estilos:** TailwindCSS / CSS3

### 📱 Aplicación Móvil
- **Framework:** Flutter SDK (Dart)
- **Linter / Estilos:** Material Design 3
- **Conexión Local:** Dirección IP puente `10.0.2.2:8080` para emulador Android

---

## 📚 Documentación de Calidad e Implantación (ISO/IEC 25010 & 29110)

Esta sección reúne la suite oficial de entregables de aseguramiento de calidad y plan de implantación evaluados según el modelo ISO/IEC 25010:

1. **[Documento 1: Plan de Implantación de Software - Estándar ISO/IEC 25010](./docs/Documento_1_Plan_de_Implantacion_ISO25010.pdf)**
2. **[Documento 2: Lista de Chequeo de Calidad del Software - Norma ISO/IEC 25010](./docs/Documento_2_Lista_de_Chequeo_Calidad.pdf)**
3. **[Documento 3: Gráfica Comparativa y Plan de Ejecución de Mejoras](./docs/Documento_3_Grafica_Comparativa_Plan_Mejoras.pdf)**
4. **[Documento 4: Cronograma del Plan de Calidad del Sistema](./docs/Documento_4_Cronograma_Plan_de_Calidad.pdf)**
5. **[Documento 5: Arquitectura y Documento Técnico del Sistema](./docs/Documento_5_Arquitectura_y_Documento_Tecnico.pdf)**
6. **[Documento 6: Acuerdo de Niveles de Servicio (SLA) en la Implantación y Posimplantación](./docs/Documento_6_Acuerdo_SLA.pdf)**
7. **[Documento 7: Actividades del Proceso de Implantación en Herramienta TIC - Trello](./docs/Documento_7_Actividades_Implantacion_Trello.pdf)**

### 📘 Guía Técnica Anexa
* **[Informe y Manual de Implantación del Software (Entorno Local)](./docs/Informe_y_Manual_de_Implantacion_Entorno_Local.pdf)**

---

## 📊 Tablero de Gestión de Proyecto
* **Tablero Kanban:** Plan de Implantación - API Lavadoras (Trello)

---

## 🛠️ Instrucciones de Despliegue Local

### 1. Base de Datos (XAMPP / MySQL)
1. Abrir **XAMPP Control Panel** e iniciar el servicio **MySQL**.
2. Acceder a phpMyAdmin (`http://localhost/phpmyadmin`).
3. Crear una base de datos con codificación `utf8mb4`:
   ```sql
   CREATE DATABASE IF NOT EXISTS lavadoras_db CHARACTER SET utf8mb4 COLLATE utf8mb4_unicode_ci;
