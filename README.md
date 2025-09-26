# 🌸 Blooming - Sistema de Análisis de Emociones Educativo

![Blooming Banner](https://img.shields.io/badge/Blooming-Educational_System-76c24f?style=for-the-badge)
![Version](https://img.shields.io/badge/version-1.0.0-blue?style=flat-square)
![License](https://img.shields.io/badge/license-GPL--3.0-green?style=flat-square)
![Angular](https://img.shields.io/badge/Angular-17-red?style=flat-square)
![Node.js](https://img.shields.io/badge/Node.js-Express-green?style=flat-square)

**Blooming** es una innovadora plataforma educativa desarrollada como **proyecto universitario** para el **Aprendizaje Basado en Proyectos (ABP)** del curso 2023/24. El sistema permite a los centros educativos analizar y monitorizar las emociones de los estudiantes a través de cuestionarios interactivos y visualizaciones 3D inmersivas.

## 📚 Contexto Académico

Este proyecto fue desarrollado como parte del **programa ABP (Aprendizaje Basado en Proyectos)** de la **Universidad de Alicante**, combinando las asignaturas de:

- **ELE (E-Learning)**
- **NM (Negocios Multimedia)**
- **PM (Proyectos Multimedia)**
- **SDM (Sitemas de Difusión Multimedia)**
- **SMA (Sistemas Multimedia Avanzados)**
- **SMBI (Sistemas Multimedia y Bases de Datos)**
- **TAG (Tecnologías de Apoyo para la Gestión)**

### 🎓 Equipo de Desarrollo

- **👨‍💻 Iker Ramón Santiana**
- **👩‍💻 Paula Meseguer Martínez**
- **👨‍💻 Francisco José Delicado González** 
- **👩‍💻 Celia Gómez Sandoval**

**Grupo:** DEK4 - ABP 2023/24

## ✨ Características Principales

### 🎯 Para Centros Educativos
- **Dashboard administrativo** con métricas de bienestar estudiantil
- **Gestión de usuarios** (alumnos, profesores, administradores)
- **Configuración de centros y clases**
- **Reportes y estadísticas avanzadas**

### 📝 Sistema de Cuestionarios
- **Cuestionarios adaptativos** basados en diferentes ámbitos emocionales
- **Análisis de respuestas** con algoritmos de procesamiento de emociones
- **Seguimiento temporal** del estado emocional de los estudiantes
- **Sistema de puntuación gamificado**

### 🌐 Visualización 3D Inmersiva
- **Motor gráfico 3D propio** desarrollado completamente desde cero por el equipo DEK4
- **Entornos virtuales interactivos** que representan diferentes escenarios
- **Experiencias inmersivas** adaptadas al estado emocional del estudiante
- **Renderizado optimizado** para dispositivos educativos

### 🔒 Seguridad y Privacidad
- **Autenticación JWT** con roles diferenciados
- **Cifrado de contraseñas** con bcrypt
- **Variables de entorno** para datos sensibles
- **Cumplimiento de estándares** de privacidad educativa

## 🏗️ Arquitectura del Sistema

```
📦 DEK4 (Blooming)
├── 🎨 Frontend (Angular 17)
│   ├── 🖥️  Interfaces de usuario responsive
│   ├── 🎮 Motor gráfico 3D propio (desarrollado desde cero)
│   ├── 📊 Dashboards interactivos (ApexCharts)
│   └── 🔐 Gestión de autenticación
│
├── ⚙️  Backend (Node.js + Express)
│   ├── 🛡️  APIs RESTful seguras
│   ├── 🔑 Sistema de autenticación JWT
│   ├── 📧 Servicio de notificaciones por email
│   └── 🤖 Algoritmos de análisis emocional
│
└── 🗄️  Base de Datos (MySQL)
    ├── 👥 Gestión de usuarios y roles
    ├── 🏫 Organización de centros y clases
    ├── 📋 Almacenamiento de cuestionarios
    └── 📈 Histórico de respuestas y métricas
```

## 🚀 Tecnologías Utilizadas

### Frontend
- **Angular 17** - Framework principal
- **Motor Gráfico 3D Propio** - Desarrollado completamente desde cero por el equipo DEK4
- **Angular Material** - Componentes UI
- **ApexCharts** - Visualización de datos
- **Bootstrap 5** - Framework CSS
- **TypeScript** - Lenguaje de programación

### Backend
- **Node.js** - Entorno de ejecución
- **Express.js** - Framework web
- **Sequelize** - ORM para base de datos
- **JWT** - Autenticación de tokens
- **bcrypt** - Cifrado de contraseñas
- **Nodemailer** - Servicio de email

### Base de Datos
- **MySQL** - Sistema de gestión de base de datos
- **Modelo relacional** optimizado para el contexto educativo

## 📋 Requisitos del Sistema

### Software Requerido
- **Node.js** 18+ 
- **MySQL** 8.0+
- **Angular CLI** 17+
- **Navegador moderno** con soporte WebGL

### Recursos Mínimos
- **RAM:** 4GB (8GB recomendado)
- **Almacenamiento:** 2GB de espacio libre
- **GPU:** Soporte WebGL para visualizaciones 3D

## ⚡ Instalación y Configuración

### 1. Clonar el Repositorio
```bash
git clone https://github.com/ABPMultimediaUA/dek4.git
cd dek4
```

### 2. Configurar Backend
```bash
cd backend
npm install

# Copiar y configurar variables de entorno
cp .env.example .env
# Editar .env con tus credenciales
```

### 3. Configurar Base de Datos
```sql
-- Crear base de datos
CREATE DATABASE blooming CHARACTER SET utf8mb4 COLLATE utf8mb4_unicode_ci;

-- Configurar usuario (opcional)
CREATE USER 'blooming_user'@'localhost' IDENTIFIED BY 'tu_password';
GRANT ALL PRIVILEGES ON blooming.* TO 'blooming_user'@'localhost';
```

### 4. Configurar Frontend
```bash
cd frontend
npm install
```

### 5. Ejecutar el Sistema
```bash
# Terminal 1: Backend
cd backend
npm start

# Terminal 2: Frontend
cd frontend
npm start
```

El sistema estará disponible en:
- **Frontend:** http://localhost:4200
- **Backend API:** http://localhost:3000

## 📊 Casos de Uso Principales

### 👨‍🏫 Para Profesores
1. **Acceso al dashboard** de la clase asignada
2. **Visualización de métricas** emocionales de los estudiantes
3. **Configuración de cuestionarios** personalizados
4. **Seguimiento del progreso** individual y grupal

### 👨‍🎓 Para Alumnos
1. **Realización de cuestionarios** adaptativos
2. **Exploración de entornos 3D** basados en sus emociones
3. **Visualización de su progreso** personal
4. **Interacción con el sistema de puntuación**

### 👨‍💼 Para Administradores
1. **Gestión completa** de usuarios y centros
2. **Configuración del sistema** y parámetros
3. **Análisis de datos agregados** del centro
4. **Supervisión del rendimiento** del sistema

## 🔧 Variables de Entorno

```bash
# Configuración del servidor
PORT=3000
TAMPORPAG=5

# Seguridad JWT
JWTSECRET=tu_clave_jwt_super_secreta

# Base de datos
DB_HOST=localhost
DB_NAME=blooming
DB_USER=tu_usuario
DB_PASSWORD=tu_password
DB_DIALECT=mysql

# Servicio de email
EMAIL_SERVICE=gmail
EMAIL_USER=tu_email@gmail.com
EMAIL_PASS=tu_password_aplicacion

```

## 🧪 Testing y Calidad

El proyecto incluye:
- ✅ **Pruebas de seguridad** implementadas
- ✅ **Validación de datos** en frontend y backend
- ✅ **Manejo de errores** robusto
- ✅ **Código documentado** y estructurado

## 🤝 Contribución

Este es un **proyecto académico universitario**. Para contribuir:

1. Fork del repositorio
2. Crear rama feature (`git checkout -b feature/NuevaFuncionalidad`)
3. Commit de cambios (`git commit -m 'Agregar nueva funcionalidad'`)
4. Push a la rama (`git push origin feature/NuevaFuncionalidad`)
5. Crear Pull Request

## 📄 Licencia

Este proyecto está licenciado bajo **GNU General Public License v3.0** - ver el archivo [LICENSE](LICENSE) para más detalles.

```
Copyright (C) 2023-2024 Equipo DEK4 - Universidad de Alicante

Este programa es software libre: puedes redistribuirlo y/o modificarlo
bajo los términos de la Licencia Pública General GNU publicada por
la Free Software Foundation, ya sea la versión 3 de la Licencia,
o (a tu elección) cualquier versión posterior.
```

## 📞 Contacto

Para consultas sobre el proyecto:

- **📧 Email de soporte:** blooming.abp@gmail.com
- **📧 Email de contacto:** iker.r.s.2002@gmail.com
- **🎓 Institución:** Universidad de Alicante
- **📅 Curso académico:** 2023/2024
- **🏷️ Programa:** Aprendizaje Basado en Proyectos (ABP)

---

<div align="center">

**Desarrollado con ❤️ por el equipo DEK4**

*Un proyecto de la Universidad de Alicante para revolucionar el bienestar estudiantil*

[![Universidad de Alicante](https://img.shields.io/badge/Universidad-de_Alicante-003d82?style=for-the-badge)](https://www.ua.es/)

</div>
