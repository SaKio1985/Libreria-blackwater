# 🌊 Blackwater Books

Una elegante vitrina digital para la saga completa de Blackwater de Michael McDowell. Este proyecto presenta los seis libros de la aclamada serie de terror gótico sureño en un formato web moderno e interactivo.

## ✨ Características

- **📚 Catálogo completo** - Los 6 libros de la saga Blackwater con descripciones detalladas
- **🎯 Páginas dinámicas** - Cada libro tiene su propia página con contenido rico
- **⭐ Puntuaciones en tiempo real** - Sistema de puntuación integrado con API externa
- **🛒 Enlaces de compra inteligentes** - Redireccionamiento automático basado en geolocalización (España/USA)
- **📱 Diseño responsivo** - Optimizado para todos los dispositivos
- **🎨 Animaciones suaves** - Transiciones elegantes entre páginas
- **🌙 Tema oscuro** - Diseño moderno con paleta de colores oscura

## 🚀 Demo

Visita la aplicación en vivo: [Blackwater Books](tu-url-de-deployment)

## 🛠️ Tecnologías

- **[Astro](https://astro.build/)** - Framework web moderno
- **[Tailwind CSS](https://tailwindcss.com/)** - Framework de CSS utility-first
- **[Vercel](https://vercel.com/)** - Plataforma de deployment
- **Javascript** -

## 📦 Instalación

1. **Clona el repositorio**
   ```bash
   git clone https://github.com/tu-usuario/blackwater-books.git
   cd blackwater-books
   ```

2. **Instala las dependencias**
   ```bash
   npm install
   ```

3. **Configura las variables de entorno**
   ```bash
   cp .env.local.example .env.local
   ```
   
   Edita `.env.local` con tus valores:
   ```env
   SCORE_API_ENDPOINT="tu-endpoint-de-puntuaciones"
   API_TOKEN="tu-token-de-api"
   SECRET_KEY="tu-clave-secreta"
   ```

4. **Inicia el servidor de desarrollo**
   ```bash
   npm run dev
   ```

5. **Abre tu navegador**
   
   Navega a `http://localhost:4321`

## 🎯 Comandos disponibles

| Comando | Acción |
|---------|--------|
| `npm install` | Instala las dependencias |
| `npm run dev` | Inicia el servidor de desarrollo en `localhost:4321` |
| `npm run build` | Construye el sitio para producción en `./dist/` |
| `npm run preview` | Previsualiza la build localmente antes del deployment |
| `npm run astro ...` | Ejecuta comandos CLI de Astro como `astro add`, `astro check` |

## 📁 Estructura del proyecto

```
blackwater-books/
├── public/              # Archivos estáticos (imágenes, favicon)
│   ├── Blackwater1.jpg
│   ├── Blackwater2.jpg
│   └── ...
├── src/
│   ├── components/      # Componentes reutilizables
│   │   ├── AmazonLogo.astro
│   │   ├── BookScore.astro
│   │   └── BuyButton.astro
│   ├── content/         # Contenido de los libros
│   │   └── books/       # Archivos Markdown de cada libro
│   ├── layouts/         # Layouts de página
│   │   └── Layout.astro
│   └── pages/           # Rutas de la aplicación
│       ├── index.astro  # Página principal
│       └── libro/
│           └── [id].astro # Páginas dinámicas de libros
├── .env.local           # Variables de entorno (no incluido)
├── astro.config.mjs     # Configuración de Astro
└── tailwind.config.mjs  # Configuración de Tailwind
```

## 🎨 Personalización

### Agregar un nuevo libro

1. Crea un archivo Markdown en `src/content/books/`:
   ```markdown
   ---
   title: "Nuevo Libro"
   author: "Autor"
   img: "imagen.jpg"
   readtime: 200
   description: "Descripción del libro"
   buy:
     spain: "https://amazon.es/..."
     usa: "https://amazon.com/..."
   ---
   
   Contenido del libro aquí...
   ```

2. Añade la imagen correspondiente en la carpeta `public/`

### Modificar el tema

Los colores y estilos se pueden personalizar en:
- `src/layouts/Layout.astro` - Variables CSS globales
- `tailwind.config.mjs` - Configuración de Tailwind

## 🌍 Deployment

Este proyecto está configurado para deployment automático en Vercel:

1. **Conecta tu repositorio** a Vercel
2. **Configura las variables de entorno** en el panel de Vercel
3. **Deploy automático** en cada push a la rama principal

También puedes deployar en otras plataformas:

```bash
# Build para producción
npm run build

# El resultado estará en ./dist/
```

## 🤝 Contribuir

Las contribuciones son bienvenidas. Por favor:

1. Fork el proyecto
2. Crea una rama para tu feature (`git checkout -b feature/AmazingFeature`)
3. Commit tus cambios (`git commit -m 'Add some AmazingFeature'`)
4. Push a la rama (`git push origin feature/AmazingFeature`)
5. Abre un Pull Request

## 📝 Licencia

Este proyecto está bajo la Licencia MIT. Ver el archivo `LICENSE` para más detalles.

## 🙏 Agradecimientos

- **Michael McDowell** - Autor de la saga Blackwater
- **Astro Team** - Por el increíble framework
- **Vercel** - Por la plataforma de hosting

## 📞 Contacto

Link del Proyecto: [https://github.com/SaKio1985/Libreria-blackwater](https://github.com/SaKio1985/Libreria-blackwater)

---

⭐ Si este proyecto te resultó útil, ¡no olvides darle una estrella!
