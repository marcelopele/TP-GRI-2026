# Página Web de Entrega - Trabajo Práctico GRI

## Descripción
Página web académica para la entrega del Trabajo Práctico sobre "Propuesta de implementación de una solución informática basada en nTIC: Non-Fungible Tokens (NFTs)" de la materia Gestión de Recursos Informáticos (GRI) de la Licenciatura en Sistemas de Información de la Facultad de Ciencias Económicas - UBA.

## Contenido de la Entrega
La página contiene los siguientes elementos:

### 1. **Información Institucional**
   - Universidad de Buenos Aires
   - Facultad de Ciencias Económicas
   - Materia: Gestión de Recursos Informáticos (GRI)
   - Carrera: Licenciatura en Sistemas de Información

### 2. **Información del Trabajo Práctico**
   - Tema: Propuesta de implementación de solución informática basada en nTIC
   - Caso de Estudio: Non-Fungible Tokens (NFTs)
   - Contexto: Presentación interna de IT a la gerencia

### 3. **Datos de Integrantes**
   - Sección editable para agregar los datos de los 4 integrantes
   - Nombre y número de registro de cada integrante
   - Los datos se guardan automáticamente en el navegador

### 4. **Archivos Descargables**
   - 1 archivo PowerPoint (.ppt) - Presentación ejecutiva
   - 4 archivos de video MP4 - Uno por cada integrante

## Estructura de Carpetas

```
TP-GRI-2026/
├── index.html              # Página principal
├── style.css               # Estilos CSS
├── script.js               # Funcionalidades JavaScript
├── archivos/               # Carpeta con archivos descargables
│   ├── Presentacion_NFTs.ppt
│   ├── Video_Integrante_1.mp4
│   ├── Video_Integrante_2.mp4
│   ├── Video_Integrante_3.mp4
│   └── Video_Integrante_4.mp4
└── README.md               # Este archivo
```

## Cómo Usar

### 1. **Agregar los Nombres de los Integrantes**
   - Edita los campos de entrada en la sección "Integrantes del Grupo"
   - Ingresa el nombre completo de cada integrante
   - Ingresa el número de registro de cada integrante
   - Los datos se guardarán automáticamente al dejar el campo

### 2. **Agregar los Archivos de Entrega**
   - Coloca el archivo `Presentacion_NFTs.ppt` en la carpeta `archivos/`
   - Coloca los 4 videos MP4 en la carpeta `archivos/`
   - Usa estos nombres exactos:
     - `Presentacion_NFTs.ppt`
     - `Video_Integrante_1.mp4`
     - `Video_Integrante_2.mp4`
     - `Video_Integrante_3.mp4`
     - `Video_Integrante_4.mp4`

### 3. **Ver la Página**
   - Abre el archivo `index.html` en un navegador web
   - O despliégala en un servidor web para que el profesor pueda acceder

## Características

### 🎨 Diseño
- **Académico y Profesional**: Diseño formal apropiado para contexto universitario
- **Responsive**: Se adapta a dispositivos móviles y escritorio
- **Animaciones Suaves**: Transiciones y efectos visuales modernos
- **Colores UBA**: Basado en colores corporativos de la Universidad de Buenos Aires

### 💾 Persistencia de Datos
- Los nombres y registros de los integrantes se guardan en `localStorage` del navegador
- No se requiere servidor o base de datos
- Los datos persisten entre sesiones

### ⚡ Funcionalidades
- **Campos Editables**: Completa los datos directamente en la página
- **Descarga de Archivos**: Enlaces de descarga para la presentación y videos
- **Validación**: Alerta si faltan datos por completar
- **Fecha Automática**: Muestra la fecha actual de entrega
- **Impresión**: Permite imprimir la página con los datos completados

## Requisitos Técnicos

- **Navegador Web**: Chrome, Firefox, Safari, Edge (versiones recientes)
- **Soporte de JavaScript**: Debe estar habilitado
- **Soporte de HTML5 y CSS3**: Navegadores modernos

## Cómo Desplegar

### Opción 1: Servidor Local (Python)
```bash
cd TP-GRI-2026
python -m http.server 8000
# Accede a http://localhost:8000
```

### Opción 2: Servidor Local (Node.js)
```bash
cd TP-GRI-2026
npx http-server
```

### Opción 3: GitHub Pages
1. Sube el contenido a un repositorio en GitHub
2. Habilita GitHub Pages en Settings
3. La página estará disponible en: `https://usuario.github.io/TP-GRI-2026`

### Opción 4: Hosting Web
- Sube la carpeta completa a cualquier servicio de hosting web
- Asegúrate de que los permisos permitan lectura de los archivos
- Comparte el URL con el profesor

## Personalización

### Cambiar Colores
Edita las variables en `style.css`:
```css
:root {
    --primary-color: #1a3a52;      /* Azul oscuro */
    --secondary-color: #2d5a7b;    /* Azul medio */
    --accent-color: #d4a574;       /* Dorado */
    --text-dark: #2c3e50;          /* Texto oscuro */
    --text-light: #5a6c7d;         /* Texto gris */
}
```

### Cambiar Contenido
Edita el archivo `index.html` para:
- Modificar información de la materia
- Cambiar nombres de secciones
- Ajustar descripciones

### Agregar Más Integrantes
Para agregar más integrantes, duplica un bloque `.team-member` en `index.html`:
```html
<div class="team-member">
    <div class="member-number">5</div>
    <p class="member-name"><input type="text" placeholder="Nombre del integrante" class="editable-field"></p>
    <p class="member-reg"><input type="text" placeholder="Número de registro" class="editable-field"></p>
</div>
```

## Soporte y Ayuda

Si tienes problemas:

1. **Los datos no se guardan**: Verifica que el navegador tenga habilitado el soporte para `localStorage`
2. **Los archivos no se descargan**: Asegúrate de que estén en la carpeta `archivos/` con los nombres correctos
3. **La página se ve mal**: Intenta actualizar la página (Ctrl+F5 o Cmd+Shift+R) para limpiar la caché

## Notas Importantes

- ✅ Los archivos deben estar en la carpeta `archivos/` exactamente como se especifica
- ✅ Los nombres de archivo son sensibles a mayúsculas/minúsculas en algunos servidores
- ✅ Asegúrate de completar todos los datos de integrantes antes de entregarla al profesor
- ✅ Prueba la descarga de archivos antes de la entrega final
- ✅ Realiza una copia de seguridad de los datos (exporta el localStorage si es necesario)

## Créditos

Página desarrollada como parte del Trabajo Práctico de Gestión de Recursos Informáticos - UBA.

---

**Última actualización**: Junio de 2026
