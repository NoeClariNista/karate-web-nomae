---

# 🥋 Club de Karate Nomae

![React](https://img.shields.io/badge/React-Frontend-blue)
![TypeScript](https://img.shields.io/badge/TypeScript-Language-blue)
![Vite](https://img.shields.io/badge/Vite-Build-purple)
![Supabase](https://img.shields.io/badge/Supabase-Backend-green)
![TailwindCSS](https://img.shields.io/badge/TailwindCSS-Styles-cyan)

Página web oficial para el **Club de Karate Nomae**.

El objetivo del proyecto es crear una plataforma moderna donde alumnos, familias y visitantes puedan conocer el club, consultar horarios, informarse sobre entrenamientos, eventos, noticias y contactar con los responsables.

---

# 🚧 Estado del proyecto

Actualmente el proyecto se encuentra en fase de desarrollo.

Próximas tareas:

- Diseño de la interfaz.
- Creación de componentes principales.
- Integración con Supabase.
- Desarrollo de contenido dinámico.
- Optimización y despliegue.

---

# 📑 Índice rápido

- [📖 Descripción](#-descripción)
- [🎯 Objetivos](#-objetivos)
- [🏯 Sobre el club](#-sobre-el-club)
- [🛠 Tecnologías](#-tecnologías)
- [🏗 Arquitectura](#-arquitectura)
- [🧠 Decisiones técnicas](#-decisiones-técnicas)
- [🗄 Base de datos Supabase](#-base-de-datos-supabase)
- [📁 Estructura del proyecto](#-estructura-del-proyecto)
- [⚙️ Instalación](#️-instalación)
- [🔐 Variables de entorno](#-variables-de-entorno)
- [✨ Funcionalidades](#-funcionalidades)
- [🎨 Diseño](#-diseño)
- [📱 Responsive](#-responsive)
- [♿ Accesibilidad](#-accesibilidad)
- [🔒 Seguridad](#-seguridad)
- [⚡ Rendimiento](#-rendimiento)
- [🔍 SEO](#-seo)
- [🧪 Testing](#-testing)
- [🚀 Roadmap](#-roadmap)
- [📸 Capturas](#-capturas)
- [🌍 Despliegue](#-despliegue)
- [👨‍💻 Autor](#-autor)

---

# 📖 Descripción

Este proyecto consiste en el desarrollo de una aplicación web responsive destinada a mejorar la presencia online del Club de Karate Nomae.

La aplicación permitirá centralizar toda la información importante del dojo y ofrecer una experiencia rápida, accesible e intuitiva para alumnos, familias y nuevos usuarios.

Principales funcionalidades:

- Presentación del club.
- Información sobre instructores.
- Horarios de entrenamiento.
- Galería multimedia.
- Noticias.
- Eventos.
- Competiciones.
- Formulario de contacto.
- Ubicación del dojo.
- Información para nuevos alumnos.

⬆️ [Volver al índice](#-índice-rápido)

---

# 🎯 Objetivos

Los objetivos principales del proyecto son:

- Mejorar la presencia digital del club.
- Facilitar el acceso a la información.
- Crear una navegación intuitiva.
- Desarrollar una aplicación escalable.
- Aplicar buenas prácticas frontend.
- Optimizar rendimiento y accesibilidad.
- Crear una base preparada para futuras funcionalidades.

⬆️ [Volver al índice](#-índice-rápido)

---

# 🏯 Sobre el club

La aplicación busca representar la identidad del Club de Karate Nomae y transmitir los valores principales del karate:

- Disciplina.
- Respeto.
- Constancia.
- Superación personal.
- Trabajo en equipo.
- Tradición.

La estética estará inspirada en la filosofía del karate y la cultura japonesa.

⬆️ [Volver al índice](#-índice-rápido)

---

# 🛠 Tecnologías

## Frontend

- React.
- React Router.
- Vite.
- TypeScript.
- HTML5.
- CSS3.

---

## Backend as a Service (BaaS)

Se utilizará **Supabase** como servicio backend.

Servicios utilizados:

- PostgreSQL Database.
- Authentication.
- Storage para imágenes.
- API REST automática.
- API Realtime.
- Row Level Security (RLS).
- Edge Functions para futuras necesidades.

---

## Estilos

- Tailwind CSS.
- Flexbox.
- CSS Grid.
- Responsive Design.

---

## Herramientas

- Git.
- GitHub.
- Visual Studio Code.
- npm.

⬆️ [Volver al índice](#-índice-rápido)

---

# 🏗 Arquitectura

La aplicación seguirá una arquitectura basada en componentes.

```
                    Usuario
                       |
                       ↓
              React Application
                       |
        --------------------------------
        |              |               |
   Components       Router          Hooks
        |
        ↓
   Supabase Client
        |
 -------------------------
 |                       |
Database              Storage
PostgreSQL            Imágenes
```

Flujo:

1. El usuario accede a la aplicación.
2. React renderiza la interfaz.
3. Los componentes solicitan información.
4. Supabase devuelve los datos.
5. La información se muestra dinámicamente.

⬆️ [Volver al índice](#-índice-rápido)

---

# 🧠 Decisiones técnicas

## ¿Por qué React?

React permite:

- Crear componentes reutilizables.
- Mantener una estructura escalable.
- Gestionar interfaces dinámicas.
- Separar lógica y presentación.

---

## ¿Por qué TypeScript?

TypeScript aporta:

- Mayor seguridad en el código.
- Mejor mantenimiento.
- Detección temprana de errores.
- Mejor experiencia de desarrollo.

---

## ¿Por qué Supabase?

Supabase permite:

- Utilizar PostgreSQL.
- Evitar crear un backend desde cero.
- Gestionar autenticación.
- Almacenar archivos.
- Escalar la aplicación fácilmente.

⬆️ [Volver al índice](#-índice-rápido)

---

# 🗄 Base de datos Supabase

La aplicación utilizará Supabase como Backend as a Service.

Servicios utilizados:

- PostgreSQL.
- API REST.
- Storage.
- Authentication.
- Row Level Security.

---

## Modelo de datos

### alumnos

Información de alumnos.

```
id
nombre
apellidos
fecha_nacimiento
grupo
fecha_alta
```

---

### instructores

Información de profesores.

```
id
nombre
grado
descripcion
imagen_url
```

---

### horarios

Información de entrenamientos.

```
id
dia
hora_inicio
hora_fin
grupo
instructor_id
```

---

### noticias

Publicaciones del club.

```
id
titulo
contenido
imagen_url
fecha_creacion
```

---

### eventos

Competiciones y actividades.

```
id
nombre
descripcion
fecha
ubicacion
imagen_url
```

---

### galeria

Contenido multimedia.

```
id
titulo
imagen_url
categoria
fecha
```

⬆️ [Volver al índice](#-índice-rápido)

---

# 📁 Estructura del proyecto

```
karate-web-nomae/

├── public/
│
├── src/
│
│   ├── assets/
│
│   ├── components/
│   │   ├── common/
│   │   ├── layout/
│   │   └── ui/
│
│   ├── pages/
│   │
│   ├── layouts/
│
│   ├── routes/
│   │   └── router.tsx
│
│   ├── services/
│   │   ├── supabase.ts
│   │   └── api/
│
│   ├── hooks/
│
│   ├── context/
│
│   ├── types/
│
│   ├── utils/
│
│   ├── styles/
│
│   ├── App.tsx
│   └── main.tsx
│
├── .env
├── package.json
├── tsconfig.json
├── vite.config.ts
└── README.md
```

⬆️ [Volver al índice](#-índice-rápido)

---

# ⚙️ Instalación

Clonar repositorio:

```bash
git clone https://github.com/NoeClariNista/karate-web-nomae.git
```

Entrar en el proyecto:

```bash
cd karate-web-nomae
```

Instalar dependencias:

```bash
npm install
```

Ejecutar:

```bash
npm run dev
```

Crear producción:

```bash
npm run build
```

Vista previa:

```bash
npm run preview
```

---

# 🔐 Variables de entorno

Crear archivo:

```
.env
```

Añadir:

```env
VITE_SUPABASE_URL=
VITE_SUPABASE_ANON_KEY=
```

Nunca subir este archivo al repositorio.

⬆️ [Volver al índice](#-índice-rápido)

---

# ✨ Funcionalidades

- Navegación SPA.
- Componentes reutilizables.
- Diseño responsive.
- Menú móvil.
- Animaciones.
- Gestión dinámica de contenido.
- Preparación para panel administrador.

⬆️ [Volver al índice](#-índice-rápido)

---

# 🎨 Diseño

La interfaz seguirá una estética relacionada con el karate:

- Diseño limpio.
- Inspiración japonesa.
- Buena jerarquía visual.
- Fotografías del dojo.
- Experiencia sencilla.

⬆️ [Volver al índice](#-índice-rápido)

---

# 📱 Responsive

La aplicación estará optimizada para:

- Desktop.
- Tablet.
- Smartphone.

Aplicando:

- Mobile First.
- Flexbox.
- CSS Grid.
- Diseño adaptable.

---

# ♿ Accesibilidad

Buenas prácticas:

- Etiquetas semánticas.
- Contraste adecuado.
- Navegación mediante teclado.
- Textos alternativos.
- Formularios accesibles.

---

# 🔒 Seguridad

Se aplicarán:

- Variables de entorno.
- RLS en Supabase.
- Validación de formularios.
- Control de permisos.
- Protección de rutas privadas.

---

# ⚡ Rendimiento

Optimización mediante:

- Lazy Loading.
- Code Splitting.
- Optimización de imágenes.
- Componentes reutilizables.
- Renderizados eficientes.

---

# 🔍 SEO

Implementación:

- Meta etiquetas.
- Open Graph.
- Sitemap.
- Robots.txt.
- URLs amigables.
- Etiquetas semánticas.

---

# 🧪 Testing

Pruebas futuras:

- Vitest.
- React Testing Library.
- Playwright.

---

# 🚀 Roadmap

## Primera versión

- [ ] Configuración inicial.
- [ ] React + Vite.
- [ ] TypeScript.
- [ ] Navbar.
- [ ] Hero.
- [ ] Footer.
- [ ] Página Inicio.
- [ ] Página Club.
- [ ] Horarios.
- [ ] Galería.
- [ ] Noticias.
- [ ] Contacto.

---

## Futuras versiones

- [ ] Integración completa Supabase.
- [ ] Autenticación.
- [ ] Panel administrador.
- [ ] Área privada alumnos.
- [ ] Reservas online.
- [ ] Gestión de pagos.
- [ ] Deploy.

---

# 📸 Capturas

Añadir capturas del proyecto:

```
docs/

home.png
horarios.png
contacto.png
```

---

# 🌍 Despliegue

Plataformas recomendadas:

- Vercel.
- Netlify.
- GitHub Pages.

---

# 👨‍💻 Autor

**Noelia Hernández Domínguez**

Proyecto desarrollado como práctica de desarrollo Frontend con React y TypeScript para la creación de una página web profesional destinada a un club de karate local.

---

# 📄 Licencia

Proyecto de uso educativo y adaptable para cualquier club deportivo.

---
