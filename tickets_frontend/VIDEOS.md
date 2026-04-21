# 🎓 Proyecto 1: Plataforma de Gestión de Tickets (Soporte L1/L2)

**Universidad:** Universidad Galileo  
**Estudiante:** Maidellin Suset Alvarado Cayax  
**Curso:** Arquitectura del Proyecto 1  

---

## 📊 Resumen de Avances: Arquitectura y Base de Datos

### 🛠️ Stack Tecnológico
- **Entorno:** Node.js
- **Lenguaje:** TypeScript 
- **Servidor Web:** Express.js 
- **Base de Datos:** PostgreSQL
- **Contenedorización:** Docker 
- **ORM:** Prisma ORM (v7.4.0) configurado con ES Modules
- **Frontend:** React (Vite) + CSS puro para diseño profesional

---

## 🚀 Logros y Configuraciones 

1. **Inicialización del Entorno Backend:** Configuré el `package.json` utilizando el estándar moderno de JavaScript (`"type": "module"`) y establecí una configuración estricta de TypeScript mediante `tsconfig.json`.
2. **Despliegue de Base de Datos:** Creé y levanté un contenedor de Docker específico para el motor de PostgreSQL.
3. **Diseño del Esquema Relacional:**
   - Implementé **UUIDs automáticos** para las llaves primarias, mejorando la seguridad e integridad del sistema.
   - Diseñé un sistema de **Soft Deletes** (`deleted_at`) y auditoría de tiempos (`created_at`, `updated_at`) en todas las tablas clave para preservar el historial exacto de datos.
   - Utilicé **ENUMs** a nivel de base de datos para restringir de forma segura los valores de roles, estados, impacto y tipos de tickets.
   - Configuré el **Borrado en Cascada** (*Cascade Delete*) en las relaciones lógicas (ej. `Cliente -> Producto`) para mantener la base de datos limpia.
4. **Migración Exitosa:** Ejecuté los comandos de migración de Prisma, sincronizando mi esquema de código TypeScript directamente con la base de datos de PostgreSQL en Docker.
5. **Generación de Reportes:** Implementé la descarga de un reporte técnico en PDF integrando los datos de la base de datos de forma dinámica.

---

## 🗄️VIDEOS DE EXPLICACION

https://www.loom.com/share/7f26740749e843fba135bad7f25e6cf2

https://www.loom.com/share/5928c71691e543e889c430deae62b3d9

https://www.loom.com/share/836b24b666e5428a835628894b718605

https://www.loom.com/share/8a950c138f7b4ac88869c94f18a0430c