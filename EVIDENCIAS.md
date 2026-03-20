# Evidencias del Proyecto Final 

## 1. Publicación y Despliegue
El sitio se encuentra desplegado y funcional en GitHub Pages.

<img width="1905" height="955" alt="image" src="https://github.com/user-attachments/assets/927bb6e1-0f28-415a-998c-c848d97fd799" />
<img width="1918" height="966" alt="image" src="https://github.com/user-attachments/assets/04d56223-9867-462a-9908-0b87a605002b" />


---

## 2. Visualización Multidispositivo (Responsive)

Para garantizar la adaptabilidad del portafolio, se probaron los siguientes breakpoints:

### 📱 Vista Móvil (~375px - 480px)
*Se implementó un menú de hamburguesa funcional con CSS puro y un layout de una sola columna para maximizar la legibilidad.*

<img width="488" height="833" alt="image" src="https://github.com/user-attachments/assets/9d9dfafa-bb29-4d7b-b275-7e96c613a257" />


### 💻 Vista Desktop (~1280px)
*Aprovechamiento del espacio horizontal mediante Grid y Flexbox, distribuyendo los proyectos en 3 columnas y expandiendo el menú de navegación.*

<img width="1918" height="922" alt="image" src="https://github.com/user-attachments/assets/bc568dca-37ee-45e9-91ab-5c652003cd34" />

---

## 3. Aprendizajes y Reflexión Técnica

### ¿Qué fue lo más fácil y lo más retador?
- **Lo más fácil:** La estructuración semántica inicial y la definición de la paleta de colores mediante variables CSS (`:root`).
- **Lo más retador:** Implementar el **Menú de Hamburguesa sin JavaScript** utilizando el "Checkbox Hack". Lograr que la transición fuera suave y que el menú se ocultara correctamente en desktop requirió un control preciso de los selectores hermanos (`~`) y de la propiedad `max-height`.

### ¿Qué partes de HTML semántico y Flexbox usaste y por qué?
- **HTML Semántico:** Utilicé `<header>`, `<nav>`, `<main>`, `<section>`, `<article>` y `<footer>`. El uso de `<article>` para los proyectos y eventos es clave, ya que cada uno es una unidad de contenido independiente y autocontenida.
- **Flexbox:** Fue el motor de todo el sitio. Lo usé en la `.navbar` para separar el logo de los links, en el `.hero` para centrar el contenido y en el `footer` para organizar las columnas. Me permitió crear un diseño fluido que "empuja" los elementos a su lugar sin medidas fijas.

### ¿Cómo organizaste tus media queries y breakpoints?
Adopté un enfoque **Mobile First**. Escribí el CSS base pensando en pantallas pequeñas y utilicé una `Media Query` principal en `@media (min-width: 768px)` para:
1. Cambiar la dirección de Flex de `column` a `row`.
2. Ocultar el icono de hamburguesa y mostrar la navegación completa.
3. Ajustar los tamaños de fuente mediante unidades `vw` (Viewport Width) para títulos dinámicos.

### ¿Qué mejorarías en una siguiente versión?
1. **Animaciones de entrada:** Implementar la API de *Intersection Observer* para que las tarjetas de proyectos aparezcan con un fundido al hacer scroll.
2. **Interactividad:** Conectar el formulario de contacto con un servicio de backend como *Formspree*.
3. **Accesibilidad avanzada:** Realizar una auditoría con *Lighthouse* para asegurar que el contraste de los colores pastel cumpla con el estándar WCAG AA en todos los elementos.

---

**Autor:** Judith Marquez Zempoalteca  
**Fecha:** Marzo 2026
