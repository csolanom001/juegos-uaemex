# Portal de Juegos de Memoria y Destreza Mental
### Universidad Autónoma del Estado de México (UAEMéx) — Nivel Medio Superior (Preparatoria)

Portal web educativo interactivo diseñado para ejercitar la memoria, la agilidad léxica y el razonamiento lógico de los estudiantes mediante tres juegos dinámicos, adaptados con la identidad visual institucional de la UAEMéx.

---

## 👥 Equipo de Desarrollo y Créditos

* **Carlos Solano** — *Crucigrama Interactivo* (Estructura semántica, lógica cliente-servidor y backend PHP).
* **Diana** — *Juego de Memoria (Memoriando)* (Generación procedural de tarjetas, cronómetro, sintetizador de audio con Web Audio API).
* **Dylan** — *Sopa de Letras* (Generador de cuadrícula dinámica, detección de selecciones y lista de palabras).

---

## 🎮 Juegos Incluidos

1. **Crucigrama (`crucigrama.html`)**:
   - Selección dinámica entre 3 temáticas: *Frutas y Verduras*, *Valores y Sentimientos*, *Personajes Históricos y Películas*.
   - Definiciones cruzadas horizontales y verticales.
   - Verificación de respuestas conectada mediante `fetch()` al backend en PHP (`php/servidor.php`).

2. **Memoriando (`memoria.html`)**:
   - Configuración de dificultad (Fácil, Medio, Difícil), cantidad de tarjetas y límites de tiempo.
   - Temáticas de tarjetas (*Frutas*, *Animales*, *Música*).
   - Efectos sonoros sintetizados nativamente en el navegador (sin dependencias de archivos de audio externos).

3. **Sopa de Letras (`sopa.html`)**:
   - Cuadrícula de búsqueda de palabras alfanumérica.
   - Selección interactiva de palabras en diferentes direcciones.
   - Lista de verificación y generador de nuevas partidas.

---

## 🛠️ Tecnologías Empleadas

* **HTML5**: Estructura semántica, accesible y compatible con lectores de pantalla.
* **CSS3**: Diseño responsivo, efectos 3D (flip cards), transiciones y paleta de colores institucional (Verde Esmeralda `#004A2F` y Oro `#C5A059`).
* **JavaScript**: Lógica interactiva en el cliente, manipulación del DOM y Web Audio API.
* **PHP**: Procesamiento lineal del lado del servidor para la validación del crucigrama.

---

## 📁 Estructura del Repositorio

```text
juegos-uaemex/
├── index.html          # Página principal con tarjetas interactivas
├── crucigrama.html     # Juego 1: Crucigrama
├── memoria.html        # Juego 2: Memoriando
├── sopa.html           # Juego 3: Sopa de letras
├── README.md           # Documentación del proyecto
├── Prompt.txt          # Requisitos y especificaciones del proyecto
├── css/
│   └── estilos.css     # Hoja de estilos compartida e institucional
├── js/
│   ├── script.js       # Lógica del portal y crucigrama
│   ├── memoria.js      # Lógica del juego de memoria
│   └── sopa.js         # Lógica de la sopa de letras
└── php/
    └── servidor.php    # Backend para validación del crucigrama
```

---

## 🚀 Ejecución del Proyecto

### Opción 1: Navegador web directo
Puedes abrir directamente el archivo `index.html` en cualquier navegador web moderno (Google Chrome, Edge, Firefox, Safari) para navegar por el portal y jugar **Memoriando** y la **Sopa de Letras**.

### Opción 2: Con servidor PHP local (recomendado para funcionalidad completa)
Para habilitar la verificación del **Crucigrama** a través del backend PHP:
1. Abre una terminal en la carpeta raíz del proyecto.
2. Ejecuta:
   ```bash
   php -S localhost:8000
   ```
3. Ingresa a `http://localhost:8000` en tu navegador.
