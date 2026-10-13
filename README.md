# Gestor de Tareas y Calendario (App React)

Esta es la estructura completa del proyecto para que puedas continuar escalándolo. Está construido con **React**, **Vite** y **Tailwind CSS**.

## Requisitos Previos
- [Node.js](https://nodejs.org/) (versión 16+ recomendada)
- npm o yarn

## Instrucciones para levantar el proyecto

1. Extrae el contenido de este `.zip` en una carpeta de tu computadora.
2. Abre una terminal (o consola de comandos) en la raíz de esa carpeta.
3. Instala las dependencias ejecutando:
   ```bash
   npm install
   ```
4. Inicia el servidor de desarrollo local ejecutando:
   ```bash
   npm run dev
   ```
5. Abre el navegador en la URL que se te indique en la terminal (por defecto suele ser `http://localhost:5173`).

## Arquitectura del Código

La lógica principal se divide en componentes modulares que puedes escalar:
- **`src/App.jsx`**: Es el contenedor principal de la aplicación. Aquí se encuentra el **estado global de tareas** (`tasks`) para que persista al cambiar de vista entre el gestor y el calendario.
- **`src/components/TaskManager.jsx`**: Contiene el formulario (título, categoría, fecha, hora) y renderiza la lista interactiva donde puedes completar/eliminar pendientes.
- **`src/components/CalendarView.jsx`**: Renderiza el calendario utilizando la librería `date-fns` para manejar las fechas con precisión. Permite cambiar entre la vista Mensual y Semanal y mapea las tareas globales en los días que corresponden según su fecha límite.

¡A seguir codificando!
