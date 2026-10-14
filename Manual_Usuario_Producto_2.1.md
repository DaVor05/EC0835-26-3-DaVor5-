

---

## 📑 Portada  
**Sistema de Gestión de Usuarios y Tareas**  
**Manual de Usuario**  
**Estándar de Competencia EC0835**

---

## 📑 Título  
**Manual de Usuario del Sistema de Gestión de Usuarios y Tareas**  

---

## 🔹 Introducción  
El sistema de **Gestión de Usuarios y Tareas** es una aplicación de escritorio diseñada para facilitar la administración interna de usuarios y las actividades o tareas asignadas dentro de una organización.  

El software permite realizar de forma intuitiva:  
- El registro, actualización y eliminación de **Usuarios**.  
- El registro, actualización y eliminación de **Tareas** asociadas a un usuario existente.  
- Consultas generales de registros y listados en tiempo real.  
- Filtros personalizados de tareas por usuario.  
- Generación de reportes de resumen con totales de tareas por cada usuario.  

Su finalidad principal es **optimizar la administración de actividades**, reduciendo errores humanos, controlando la integridad de la base de datos y ofreciendo una interfaz visual amigable.  

---

## 🎯 Objetivos  

### Objetivo general  
Brindar a los usuarios finales una herramienta informática sencilla, autónoma y funcional para la gestión eficiente de usuarios y tareas cotidianas.  

### Objetivos específicos  
- Permitir la administración y control del ciclo de vida de los usuarios en el sistema.  
- Controlar la creación y asignación segura de tareas vinculadas mediante llaves relacionales.  
- Facilitar la consulta rápida, el filtrado y la obtención de resúmenes estadísticos.  
- Ofrecer un sistema ejecutable de fácil instalación y uso sin requerir conocimientos técnicos avanzados.  

---

## 🖥️ Requisitos de instalación  

### Hardware mínimo  
- **Procesador:** Intel i3 / Dual Core 2.0 GHz o superior.  
- **Memoria RAM:** 4 GB mínimo.  
- **Espacio en disco:** 200 MB libres.  

### Software  
- **Sistema operativo:** Windows 10 o Windows 11.  
- **Archivo ejecutable:** `main.exe` (generado mediante PyInstaller).  
- **Base de datos:** SQLite (archivo `tareas.db`, ubicado en la misma ruta que el ejecutable).  

---

## ⚙️ Instalación y configuración  

1. Copia la carpeta del sistema entregada a la ubicación de tu preferencia en tu computadora.  
2. Asegúrate de que el archivo ejecutable (`main.exe`) y el archivo de base de datos (`tareas.db`) se encuentren en la **misma carpeta**.  
3. Haz doble clic en **`main.exe`** para iniciar el sistema.  
4. *(Opcional)* Haz clic derecho sobre el archivo ejecutable, selecciona *Enviar a > Escritorio (crear acceso directo)* para mayor comodidad.  

---

## 📝 Guía de uso de funciones básicas  

### 1. Registrar un usuario  
1. Dirígete al panel izquierdo titulado **Gestión de Usuarios**.  
2. Ingresa el **Nombre** y el **Email** en sus respectivas casillas de texto.  
3. Haz clic en el botón **Registrar Usuario**.

<img width="231" height="104" alt="image" src="https://github.com/user-attachments/assets/19046f07-1540-47fa-ba34-c02c3543e435" />

4. El sistema validará que los campos no estén vacíos y te mostrará un mensaje de éxito confirmando el registro.

<img width="505" height="237" alt="image" src="https://github.com/user-attachments/assets/744b2c66-525a-439f-97f9-05c8e313331c" />

5. Esto aparecera sin no tiene nada escrito en los dos casillas.

<img width="474" height="200" alt="image" src="https://github.com/user-attachments/assets/334f5ffc-49da-4f21-a4b3-567e8d9cfb14" />



### 2. Registrar una tarea  
1. Dirígete al panel derecho titulado **Gestión de Tareas**.  
2. Ingresa el **Título**, la **Descripción**, la **Prioridad** y el **ID de usuario** al que se le asignará la tarea.  
3. Haz clic en el botón **Registrar Tarea**.

<img width="254" height="151" alt="image" src="https://github.com/user-attachments/assets/80a8b14d-3434-4908-a2eb-4376f350bed4" />

4. El sistema verificará que el ID de usuario exista; si es correcto, guardará la información y mostrará un mensaje de confirmación.  

<img width="442" height="210" alt="image" src="https://github.com/user-attachments/assets/e2b37725-c4b3-40c1-b095-8e9a5b9c613e" />


### 3. Consultar registros (Mostrar Usuarios / Mostrar Tareas)  
- Haz clic en **Mostrar Usuarios** para desplegar la lista completa de usuarios registrados en la caja de resultados inferior.

<img width="362" height="216" alt="image" src="https://github.com/user-attachments/assets/08e75278-7ff3-4f4b-a5f4-6071cd30095b" />

- Haz clic en **Mostrar Tareas** para visualizar todas las tareas vinculadas con sus respectivos usuarios y prioridades.  

<img width="604" height="168" alt="image" src="https://github.com/user-attachments/assets/83240858-04a5-4f35-b945-8c6256e71c54" />


### 4. Filtrar y resumir tareas  
- **Filtrar por Usuario:** Ingresa un ID de usuario válido en el campo *ID Usuario* y haz clic en **Filtrar por Usuario** para ver exclusivamente las tareas de esa persona.  

<img width="630" height="280" alt="image" src="https://github.com/user-attachments/assets/116a3f33-e91e-4fa4-972b-72d928b52002" />

- **Resumen por Usuario:** Haz clic en el botón **Resumen por Usuario** para obtener el conteo total de tareas asignadas a cada miembro del sistema.  

<img width="651" height="178" alt="image" src="https://github.com/user-attachments/assets/fc95c208-914f-4fbf-8985-c58116331033" />


### 5. Editar y Eliminar Registros  
- **Para Editar:** Escribe los nuevos datos en los campos del formulario correspondiente (Usuarios o Tareas), haz clic en el botón **Editar Usuario** o **Editar Tarea**, e ingresa el ID exacto del registro a modificar cuando el sistema te lo solicite.

**Usuario**

<img width="400" height="323" alt="image" src="https://github.com/user-attachments/assets/518e0ed2-1dc9-42c6-9823-1833bbaf08da" />

<img width="542" height="266" alt="image" src="https://github.com/user-attachments/assets/d6765b4d-2193-4408-811a-d560e8b39e58" />

**Tareas**

<img width="282" height="390" alt="image" src="https://github.com/user-attachments/assets/b7151dac-c19f-44e3-902f-5a8900cb28b5" />

<img width="470" height="208" alt="image" src="https://github.com/user-attachments/assets/b986ebcb-5820-4030-a9f2-1450e68158eb" />

- **Para Eliminar:** Haz clic en **Eliminar Usuario** o **Eliminar Tarea** e introduce el número de ID que deseas borrar del sistema.

**Usuario**

<img width="313" height="237" alt="image" src="https://github.com/user-attachments/assets/2e842dd3-65f6-4382-a8db-a18ea611c94d" />

<img width="266" height="190" alt="image" src="https://github.com/user-attachments/assets/37f2f721-23a5-41fd-bf98-b58365e05261" />

**Tareas**

<img width="427" height="184" alt="image" src="https://github.com/user-attachments/assets/f3e0342a-8deb-4caa-99f8-69c7a716ffee" />

<img width="286" height="196" alt="image" src="https://github.com/user-attachments/assets/1cc09340-4168-4b57-9470-da20c7daf315" />

---

## ⚠️ Mensajes de error frecuentes y solución  

1. **"El ID de usuario 'X' no existe en la base de datos."**  
   - *Causa:* Intentaste registrar o filtrar una tarea asociándola a un ID numérico que no ha sido dado de alta previamente.  
   - *Solución:* Consulta la lista de usuarios para verificar el ID correcto o registra primero al usuario.  
2. **"Debes ingresar un Título y un ID de usuario numérico válido."**  
   - *Causa:* Dejaste campos obligatorios vacíos o escribiste letras en lugar de números en el campo de ID.  
   - *Solución:* Rellena los datos solicitados asegurándote de usar números enteros en los campos de identificación.  

---

## 📖 Glosario  

- **Base de datos (SQLite):** Archivo local (`tareas.db`) donde se almacena de forma persistente toda la información del sistema.  
- **Registro:** Conjunto de datos coherentes almacenados en la base de datos (por ejemplo, los datos de un usuario o de una tarea).  
- **ID (Identificador):** Número entero único autoincrementable que identifica inequívocamente a cada usuario o tarea.  
- **Ejecutable (.exe):** Archivo compilado que permite ejecutar la aplicación de escritorio en Windows sin requerir instalación previa de Python.  
- **CRUD:** Acrónimo de las cuatro operaciones básicas de una base de datos: Crear, Leer, Actualizar y Eliminar.  

---
