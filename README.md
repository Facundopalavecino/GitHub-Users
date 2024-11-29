# 🔎 GitHub User Search

¡Bienvenido a **GitHub User Search**! 🚀  
Esta aplicación te permite buscar usuarios en GitHub de forma sencilla. Solo necesitas ingresar un nombre de usuario, y la aplicación retornará los perfiles relacionados junto con un botón para visitar el perfil directamente en GitHub.

---

## 🌟 Características

- 🔍 **Búsqueda instantánea:** Busca usuarios de GitHub escribiendo su nombre en el campo de búsqueda.
- 🖼️ **Visualización intuitiva:** Muestra los resultados con el nombre de usuario, su avatar y un enlace directo al perfil.
- ⚡ **Interfaz dinámica:** Resultados actualizados en tiempo real al presionar la tecla **Enter**.
- 🧹 **Limpieza automática:** Se eliminan resultados antiguos al realizar una nueva búsqueda.

---

## 🛠️ Tecnologías y Herramientas

- **HTML5** y **CSS3**: Estructura y diseño de la aplicación.
- **JavaScript (ES6)**: Implementación de lógica de búsqueda y manipulación dinámica del DOM.
- **Fetch API**: Realiza solicitudes a la API pública de GitHub.
- **GitHub REST API**: Proporciona datos de usuarios en tiempo real.

---

## 🧩 Estructura del Proyecto

1. **Clase `Github`:**
   - `getUsers(username)`: Realiza solicitudes a la API de GitHub y retorna una promesa con los resultados.
   - `createElement(items, result)`: Genera dinámicamente elementos HTML para mostrar los resultados de la búsqueda.

2. **Lógica principal:**
   - Captura el evento **keyup** en el campo de búsqueda.
   - Envía el término ingresado a la API y actualiza los resultados mostrados.

3. **Estilo y Diseño:**
   - Los perfiles de usuario incluyen un avatar, nombre y un botón "View" para acceder al perfil directamente en GitHub.

🌐 API Utilizada
Se utilizó la GitHub REST API para obtener datos relacionados con los usuarios.

📝 Notas
    - Asegúrate de usar un navegador moderno que soporte la Fetch API.
    - La búsqueda es sensible a las palabras ingresadas; por ejemplo, "john" retornará diferentes resultados que "John Doe".