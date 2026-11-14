

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
El sistema de **Gestión de Usuarios y Tareas** es una aplicación de escritorio avanzada diseñada para facilitar la administración interna de usuarios, el control de acceso seguro y las actividades o tareas asignadas dentro de una organización.

El software permite realizar de forma intuitiva:  
- El control de acceso mediante un sistema de inicio de sesión y configuración inicial de cuentas de administrador.
- El registro, actualización y borrado lógico de Usuarios.
- El registro, actualización y borrado lógico de Tareas asociadas de forma relacional a un usuario existente.
- Consultas generales de registros y listados en tiempo real.
- Filtros personalizados de tareas por usuario y reportes de resumen con conteos totales.
- La visualización de gráficas estadísticas interactivas (tareas por usuario, por prioridad y comparativas de registros activos frente a la papelera).
- La administración de un módulo de Papelera, que permite recuperar (restaurar) elementos eliminados lógicamente o purgarlos de forma definitiva de la base de datos.

Su finalidad principal es **optimizar la administración de actividades y garantizar la seguridad de la información**, reduciendo errores humanos, controlando la integridad referencial de la base de datos y ofreciendo una interfaz visual moderna organizada mediante un sistema de pestañas.

---

## 🎯 Objetivos  

### Objetivo general  
Brindar a los usuarios finales una herramienta informática segura, autónoma, intuitiva y funcional para la gestión eficiente de cuentas, usuarios y tareas cotidianas, respaldada por un control de acceso robusto, herramientas de recuperación de datos y reportes gráficos dinámicos.

### Objetivos específicos  
- Garantizar la seguridad y el control de acceso al sistema mediante autenticación de credenciales y detección automatizada de primer arranque para cuentas administrativas.
- Permitir la administración y el control integral del ciclo de vida de los usuarios y tareas en el sistema.
- Controlar la creación y asignación segura de tareas vinculadas mediante llaves relacionales e integridad referencial en SQLite.
- Facilitar la consulta rápida, el filtrado, la obtención de resúmenes y la interpretación de datos mediante módulos de gráficas estadísticas.
- Proveer un sistema de papelera que soporte borrado lógico (soft-delete), restauración de registros y eliminación definitiva según los requerimientos de la organización.
- Ofrecer un sistema ejecutable independiente (.exe) de fácil instalación y uso sin requerir conocimientos técnicos avanzados.

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

### 1. Control de Acceso y Autenticación
1. **Primer Arranque (Creación de Administrador):** La primera vez que ejecutes el sistema, aparecerá una ventana solicitando crear una cuenta de administrador.

<img width="447" height="474" alt="image" src="https://github.com/user-attachments/assets/29adbd10-f486-441a-9239-341bb01e2ad1" />

2. Ingresa un nombre de usuario (mínimo 3 caracteres) y una contraseña (mínimo 6 caracteres), confírmala y haz clic en **Crear cuenta**

<img width="446" height="478" alt="image" src="https://github.com/user-attachments/assets/ce4692d8-207b-408e-a87c-2c06a46c450f" />

3. **Inicio de Sesión:** En los siguientes arranques, introduce tus credenciales y haz clic en **Entrar** para acceder al sistema.

<img width="448" height="477" alt="image" src="https://github.com/user-attachments/assets/ad3bac8d-dfa2-4600-bb20-d954a8ba7b6d" />

4. Puedes cerrar sesión en cualquier momento desde el botón superior derecho.

<img width="635" height="668" alt="image" src="https://github.com/user-attachments/assets/c69280b1-9aac-4f7d-bf35-dba192db544f" />




### 2. Registrar un usuario  
1. Dirígete al panel izquierdo titulado **Gestión de Usuarios**.  
2. Ingresa el **Nombre** y el **Email** en sus respectivas casillas de texto.  
3. Haz clic en el botón **Registrar Usuario**.

<img width="231" height="104" alt="image" src="https://github.com/user-attachments/assets/19046f07-1540-47fa-ba34-c02c3543e435" />

4. El sistema validará que los campos no estén vacíos y te mostrará un mensaje de éxito confirmando el registro.

<img width="505" height="237" alt="image" src="https://github.com/user-attachments/assets/744b2c66-525a-439f-97f9-05c8e313331c" />

5. Esto aparecera sin no tiene nada escrito en los dos casillas.

<img width="474" height="200" alt="image" src="https://github.com/user-attachments/assets/334f5ffc-49da-4f21-a4b3-567e8d9cfb14" />


### 3. Registrar una tarea  
1. Dirígete al panel derecho titulado **Gestión de Tareas**.  
2. Ingresa el **Título**, la **Descripción**, la **Prioridad** y el **ID de usuario** al que se le asignará la tarea.  
3. Haz clic en el botón **Registrar Tarea**.

<img width="256" height="318" alt="image" src="https://github.com/user-attachments/assets/1beeffb8-3df0-43e8-a3d5-a8a0b0d07563" />

4. El sistema verificará que el ID de usuario exista; si es correcto, guardará la información y mostrará un mensaje de confirmación.  

<img width="290" height="227" alt="image" src="https://github.com/user-attachments/assets/19ccdfd5-27e5-4677-8637-40405dadc27e" />


### 4. Consultar registros (Mostrar Usuarios / Mostrar Tareas)  
- Haz clic en **Mostrar Usuarios** para desplegar la lista completa de usuarios registrados en la caja de resultados inferior.

<img width="362" height="216" alt="image" src="https://github.com/user-attachments/assets/08e75278-7ff3-4f4b-a5f4-6071cd30095b" />

- Haz clic en **Mostrar Tareas** para visualizar todas las tareas vinculadas con sus respectivos usuarios y prioridades.  

<img width="614" height="246" alt="image" src="https://github.com/user-attachments/assets/415b7140-11ee-4cb7-aba2-018d2893cf83" />


### 5. Filtrar y resumir tareas  
- **Filtrar por Usuario:** Ingresa un ID de usuario válido en el campo *ID Usuario* y haz clic en **Filtrar por Usuario** para ver exclusivamente las tareas de esa persona.  

<img width="594" height="340" alt="image" src="https://github.com/user-attachments/assets/e0a8b795-7894-4f72-b58f-1ccb1eb888b5" />

- **Resumen por Usuario:** Haz clic en el botón **Resumen por Usuario** para obtener el conteo total de tareas asignadas a cada miembro del sistema.  

<img width="651" height="178" alt="image" src="https://github.com/user-attachments/assets/fc95c208-914f-4fbf-8985-c58116331033" />


### 6. Editar y Eliminar Registros  
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

### 7. Uso de la Pestaña de Gráficas Estadísticas
1. Haz clic en la pestaña **Gráficas** en la parte superior de la ventana principal.

<img width="633" height="106" alt="image" src="https://github.com/user-attachments/assets/a1f65938-b163-4392-a04d-83f102c81385" />

2. Selecciona el tipo de reporte que deseas visualizar en el menú desplegable (*Tareas por usuario*, *Tareas por prioridad* o *Activos vs Papelera*).

**Tareas por usuario**

<img width="519" height="542" alt="image" src="https://github.com/user-attachments/assets/7ab9437e-943d-497a-aeea-8bc2c81961fe" />

**Tareas por prioridad**

<img width="596" height="508" alt="image" src="https://github.com/user-attachments/assets/25f98e62-3b15-4c77-829a-efda724c269d" />

**Activos vs Papelera**

<img width="614" height="579" alt="image" src="https://github.com/user-attachments/assets/729ba3e3-cef4-428f-b4de-1ad62de1843b" />

3. Haz clic en el botón **Actualizar** para generar y renderizar las barras estadísticas dinámicas en el panel.

<img width="557" height="132" alt="image" src="https://github.com/user-attachments/assets/cc1e71db-3968-4ae3-8a50-78517d5eb30c" />


### 8. Gestión de la Papelera (Borrado Lógico y Restauración)
1. Haz clic en la pestaña **Papelera** para visualizar los elementos que han sido eliminados de manera lógica.

<img width="615" height="68" alt="image" src="https://github.com/user-attachments/assets/37fe34e3-1a06-4670-bfea-c0229db3f7ad" />

3. **Restaurar:** Selecciona un elemento de la lista de usuarios o tareas desactivadas y haz clic en **Restaurar** para reactivarlo en el sistema.

<img width="457" height="567" alt="image" src="https://github.com/user-attachments/assets/3554dfc8-fa25-4988-851e-b1bd9145e147" />

5. **Eliminación Definitiva:** Selecciona el registro y haz clic en **Eliminar definitivamente**, confirmando la advertencia para borrar permanentemente el dato de la base de datos.

<img width="464" height="542" alt="image" src="https://github.com/user-attachments/assets/59f63ad6-1f9c-4f93-a594-09b5959eb886" />

<img width="404" height="537" alt="image" src="https://github.com/user-attachments/assets/3a076839-852c-43d7-812e-7a26e622cc23" />


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
