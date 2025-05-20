# Parcial-2
✨ Objetivos del Proyecto
Manipulación del DOM con JavaScript.
Modularización de código (modelo y vista).
Persistencia de datos usando localStorage.
Aplicación de lógica condicional y validaciones.
Visualización gráfica de datos.
🚀 Funcionalidades Implementadas
1. Registro y Login de Usuarios (30%)
Registro de usuario con nombre completo, username y contraseña (15%).
Login validando credenciales contra localStorage (15%).
Contraseñas almacenadas como hash usando la siguiente función:

js
Copy
Edit
function hashCode(str) {
    let hash = 0;
    for (let i = 0; i < str.length; i++) {
        let chr = str.charCodeAt(i);
        hash = (hash << 5) - hash + chr;
        hash |= 0;
    }
    return hash;
}
Si hay sesión activa, se redirige automáticamente al dashboard.
Si no hay sesión, cualquier ruta redirige al login.
2. Dashboard de Libros (30%)
Muestra el nombre del usuario logueado.
Tabla con libros leídos que incluye:
Título
Autor
Fecha de lectura
Número de páginas
¿Lo recomendarías?
Permite agregar y eliminar libros, con persistencia en localStorage.
3. Perfil del Usuario (15%)
Visualización y edición del nombre del usuario.
Opción para cambiar la contraseña, aplicando nuevamente el hash.
4. Estadísticas de Lectura (20%)
Cantidad total de libros leídos.
Promedio de páginas por libro.
Gráfico (de barras o pastel) que muestra:
Libros recomendados vs. no recomendados.
EL gráfico pude implementarlo con Div 
5. Validaciones Extras (5%)
Validación de campos vacíos al registrar usuarios o libros.
Validación para evitar que un username ya registrado se repita.
🧱 Tecnologías Utilizadas
HTML/CSS/JS (Vanilla)
localStorage para persistencia
