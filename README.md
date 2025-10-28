🧩 BBDD_SQL-PLSQL

Repositorio que contiene la implementación de una base de datos completa en Oracle, con integración a un backend Node.js alojado en Oracle Cloud, orientado a la gestión de ventas y control de operaciones.

Incluye:

Creación y modelado de tablas.

Consultas SQL optimizadas.

Funciones y procedimientos almacenados (PL/SQL).

Triggers automáticos de auditoría y bitácora.

Control de errores y registro histórico de eventos.

🗺️ Modelo ER

Estructura general del modelo entidad-relación de la base de datos.

<p align="center"> <img src="https://github.com/user-attachments/assets/cd09795d-b763-4b3f-9738-a6bc5448d615" width="600"> </p>
⚙️ Triggers de bitácora

Ejemplo de trigger aplicado tras una operación UPDATE, registrando automáticamente los cambios en la tabla de bitácora y sincronizándose con el backend vía API Node.js.

<p align="center"> <img src="https://github.com/user-attachments/assets/19972de1-18a5-4ca1-8787-c84c02f9f4f9" width="600"> </p>
📦 Ejecución remota de procedimientos

Ejecución de un package PL/SQL y de procedimientos almacenados mediante peticiones al backend desplegado en Oracle Cloud.

<p align="center"> <img src="https://github.com/user-attachments/assets/a380ce76-a10d-4793-9c44-aba87b8bbfbe" width="600"> </p>
🧮 Control de errores

Ejecución repetida del proceso en un mismo año genera detección automática de errores y registro en la tabla de auditoría.

<p align="center"> <img src="https://github.com/user-attachments/assets/17eb1640-6244-4742-96cb-f855ef8e80eb" width="600"> </p>
🧱 Bitácora de eventos

Todos los errores y operaciones relevantes quedan almacenados en la tabla de bitácora para seguimiento y depuración.

<p align="center"> <img src="https://github.com/user-attachments/assets/b2b52e3f-88f9-4988-9acd-b0f2ab54dfa0" width="600"> </p>
