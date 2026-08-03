---

# 🥋 Club de Karate Nomae.

Página web oficial para un club de karate Nomae. El objetivo es ofrecer una plataforma moderna donde los usuarios puedan conocer el club, consultar horarios, informarse sobre los entrenamientos, eventos, noticias y contactar con los responsables.

---

# 📖 Descripción.

Este proyecto consiste en el desarrollo de una aplicación web responsive destinada a mejorar la presencia online del club.

Entre sus principales funciones estarán:

- Presentación del club.
- Información sobre instructores.
- Horarios de entrenamiento.
- Galería de imágenes.
- Noticias y eventos.
- Información sobre competiciones.
- Formulario de contacto.
- Localización del dojo.
- Información para nuevos alumnos.

El diseño estará orientado a ofrecer una experiencia sencilla, rápida y accesible desde cualquier dispositivo.

---

# 🎯 Objetivos.

- Mejorar la presencia digital del club.
- Facilitar el acceso a la información.
- Conseguir una navegación intuitiva.
- Optimizar el rendimiento.
- Aplicar buenas prácticas de desarrollo con React.
- Crear una aplicación fácilmente escalable.

---

# 🛠 Tecnologías.

## Frontend

- React.
- React Router.
- Vite.
- TypeScript.
- HTML5.
- CSS3.

## Backend as a Service (BaaS)
- Supabase.
  - Base de datos PostgreSQL.
  - Autenticación (si se implementa).
  - Storage para imágenes y archivos.
  - API REST automática.
  - API Realtime (si se necesita).
  - Políticas de seguridad (RLS).
  - Edge Functions (opcional).

## Estilos.

- Tailwind CSS.
- Flexbox.
- CSS Grid.
- Responsive Design.

## Herramientas.

- Git.
- GitHub.
- VS Code.
- npm.

---

# 🗄 Base de datos.

La aplicación utilizará Supabase como Backend as a Service (BaaS).

Se aprovecharán los siguientes servicios:

- Base de datos PostgreSQL.
- API REST generada automáticamente.
- Almacenamiento de imágenes para la galería.
- Autenticación de administradores (futuro).
- Políticas de seguridad mediante Row Level Security (RLS).

### Posibles tablas.

- alumnos.
- instructores.
- horarios.
- noticias.
- eventos.
- categorias.
- galeria.
- usuarios (administradores).

---

# 📁 Estructura del proyecto.

```

mi-proyecto/
│
├── public/
│   ├── images/
│   ├── icons/
│   └── favicon.ico
│
├── src/
│   ├── assets/
│   │
│   ├── components/
│   │   ├── common/
│   │   ├── layout/
│   │   └── ui/
│   │
│   ├── pages/
│   │   ├── Home/
│   │   ├── Login/
│   │   ├── Profile/
│   │   └── NotFound/
│   │
│   ├── layouts/
│   │
│   ├── routes/
│   │   └── router.tsx
│   │
│   ├── services/
│   │   ├── supabase.ts
│   │   └── api/
│   │
│   ├── hooks/
│   │
│   ├── context/
│   │
│   ├── types/
│   │
│   ├── utils/
│   │
│   ├── styles/
│   │
│   ├── App.tsx
│   ├── main.tsx
│   └── vite-env.d.ts
│
├── .env
├── .gitignore
├── eslint.config.js
├── package.json
├── tsconfig.json
├── vite.config.ts
└── README.md


src/
│
├── assets/
│   ├── images/
│   ├── icons/
│   └── logos/
├── components/
│   ├── Navbar/
│   ├── Footer/
│   ├── Hero/
│   ├── Cards/
│   ├── Button/
│   ├── Gallery/
├── pages/
│   ├── Home.jsx
│   ├── Club.jsx
│   ├── Horarios.jsx
│   ├── Noticias.jsx
│   ├── Eventos.jsx
│   ├── Galeria.jsx
│   ├── Contacto.jsx
│   └── Error404.jsx
├── context/
├── data/
├── App.jsx
├── main.jsx
└── router.jsx
```

---

# 🚀 Funcionalidades.

- Navegación SPA.
- Diseño responsive.
- Menú adaptable a móviles.
- Componentes reutilizables.
- Animaciones suaves.
- Carga optimizada de imágenes.
- Organización modular.
- Código mantenible.
- Posibilidad de añadir un panel de administración en el futuro.

---

# 📄 Secciones de la web.

## Inicio.

- Imagen principal.
- Presentación.
- Últimas noticias.
- Accesos rápidos.

---

## El Club.

- Historia.
- Filosofía.
- Valores.
- Información general.

---

## Senseis.

- Fotografía.
- Grado.
- Experiencia.
- Biografía.

---

## Horarios.

- Horarios por grupos.
- Niños.
- Adultos.
- Competición.

---

## Galería.

- Fotografías.
- Vídeos.
- Eventos destacados.

---

## Noticias.

- Publicaciones.
- Resultados.
- Competiciones.

---

## Contacto.

- Formulario.
- Email.
- Teléfono.
- Redes sociales.
- Ubicación mediante Google Maps.

---

# 📱 Responsive.

La aplicación estará optimizada para:

- Desktop.
- Tablet.
- Smartphone.

---

# ♿ Accesibilidad.

Se seguirán buenas prácticas como:

- Uso correcto de etiquetas semánticas.
- Contraste adecuado.
- Navegación mediante teclado.
- Textos alternativos en imágenes.
- Formularios accesibles.

---

# ⚡ Rendimiento.

Se buscará optimizar:

- Lazy Loading.
- División del código (Code Splitting).
- Optimización de imágenes.
- Componentes reutilizables.
- Renderizados eficientes.

---

# 🔍 SEO.

- Meta etiquetas.
- Open Graph.
- Sitemap.
- Robots.txt.
- URLs amigables.
- Etiquetas semánticas.

---

# 🔐 Futuras mejoras.

- Área privada para alumnos.
- Gestión de pagos.
- Reserva de clases.
- Calendario de eventos.
- Gestión de licencias.
- Panel de administración.
- Integración con Firebase.
- Backend propio.
- Base de datos.
- Login.

---

# 💻 Instalación.

Clonar el repositorio.

```bash
git clone [https://github.com/usuario/club-karate-tenerife.git](https://github.com/NoeClariNista/karate-web-nomae.git)
```

Entrar en el proyecto.

```bash
cd karate-web-nomae
```

Instalar dependencias.

```bash
npm install
```

Ejecutar el proyecto.

```bash
npm run dev
```

Compilar para producción.

```bash
npm run build
```

Vista previa.

```bash
npm run preview
```

---

# 📌 Convenciones.

- Componentes en PascalCase.
- Hooks con prefijo `use`.
- Variables descriptivas.
- Componentes pequeños y reutilizables.
- Separación entre lógica y presentación.

---

# 🌳 Git Flow.

Se recomienda trabajar mediante ramas:

```
main
│
develop
│
feature/navbar
feature/home
feature/contacto
feature/galeria
feature/horarios
feature/noticias
```

---

# 📝 Commits.

Ejemplos:

```
feat: añadir componente Hero

fix: corregir navegación

style: mejorar diseño responsive

refactor: simplificar componente Card

docs: actualizar README

chore: actualizar dependencias
```

---

# 📷 Capturas.

Aquí podrán añadirse imágenes del proyecto.

```
/docs
    home.png
    horarios.png
    contacto.png
```

---

# 📌 Roadmap.

- [ ] Configuración inicial
- [ ] React + Vite
- [ ] Navbar
- [ ] Hero
- [ ] Footer
- [ ] Página Inicio
- [ ] Página Club
- [ ] Horarios
- [ ] Galería
- [ ] Noticias
- [ ] Contacto
- [ ] Responsive
- [ ] SEO
- [ ] Optimización
- [ ] Deploy

---

# 🚀 Despliegue.

El proyecto podrá desplegarse en:

- GitHub Pages
- Netlify
- Vercel

---

# 👨‍💻 Autor.

Nombre: Noelia Hernández Domínguez.

Proyecto desarrollado como práctica de desarrollo Frontend con React para el desarrollo de una página web necesaria en un club de Karate Local.

---

# 📄 Licencia.

Este proyecto es de uso educativo y puede adaptarse para cualquier club deportivo.

---
