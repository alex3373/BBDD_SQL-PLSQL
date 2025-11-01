# BBDD_SQL-PLSQL

Repositorio que contiene la implementación completa de una **base de datos Oracle** integrada con un **backend Node.js** desplegado en **Oracle Cloud**, orientada a la gestión de ventas, control de operaciones y auditoría automática de procesos.

Incluye:

- Creación y modelado de tablas.
- Consultas SQL optimizadas.
- Funciones y procedimientos almacenados (PL/SQL).
- Triggers automáticos de auditoría y bitácora.
- Control de errores y registro histórico de eventos.
- Ejecución remota de paquetes PL/SQL mediante la API del backend.

---

## Repositorios Relacionados

- [Backend (Node.js + Oracle Cloud)](https://github.com/alex3373/Oracle_Gestion_API)
- [Frontend (Next.js + Firebase Hosting)](https://github.com/alex3373/Frontend_Gestion_BBDD)

---

## Modelo ER

Estructura general del modelo entidad-relación de la base de datos.

<p align="center">
  <img src="https://github.com/user-attachments/assets/cd09795d-b763-4b3f-9738-a6bc5448d615" width="600">
</p>

---

## Triggers de Bitácora

Ejemplo de trigger aplicado tras una operación **UPDATE**, registrando automáticamente los cambios en la tabla de bitácora y sincronizándose con el backend vía API Node.js.

<p align="center">
  <img src="https://github.com/user-attachments/assets/19972de1-18a5-4ca1-8787-c84c02f9f4f9" width="600">
</p>

**Endpoint relacionado:**  
`GET https://api.0003333.xyz/api/bitacora`

---

## Ejecución Remota de Procedimientos

Ejecución de un package PL/SQL y de procedimientos almacenados mediante peticiones al backend desplegado en Oracle Cloud.

<p align="center">
  <img src="https://github.com/user-attachments/assets/a380ce76-a10d-4793-9c44-aba87b8bbfbe" width="600">
</p>

**Endpoints relacionados:**  
`GET https://api.0003333.xyz/api/generar-informe/:anio`  
`GET https://api.0003333.xyz/api/porcentaje-vendedor`

---

## Control de Errores

Ejecución repetida del proceso en un mismo año genera detección automática de errores y registro en la tabla de auditoría.

<p align="center">
  <img src="https://github.com/user-attachments/assets/17eb1640-6244-4742-96cb-f855ef8e80eb" width="600">
</p>

**Endpoint relacionado:**  
`GET https://api.0003333.xyz/api/errores`

---

## Bitácora de Eventos

Todos los errores y operaciones relevantes quedan almacenados en la tabla de bitácora para seguimiento y depuración.

<p align="center">
  <img src="https://github.com/user-attachments/assets/b2b52e3f-88f9-4988-9acd-b0f2ab54dfa0" width="600">
</p>

**Endpoint relacionado:**  
`GET https://api.0003333.xyz/api/bitacora`

---

## Integración Completa

El flujo de trabajo entre base de datos y backend permite:

- Registrar eventos automáticamente vía **triggers PL/SQL**.  
- Consultar y actualizar información mediante **API REST**.  
- Visualizar resultados y reportes a través del **frontend Next.js**.  

```mermaid
graph LR
  A[(Oracle Database - PL/SQL)] --> B[[API NodeJS - Oracle Cloud]]
  B --> C([Frontend NextJS - Firebase Hosting])
```


---

## Autor

**Alexis Córdova Díaz**  
Analista Programador | Desarrollador Full Stack  
📧 alexisandres311@gmail.com  
🌐 [linkedin.com/in/alexis-andres-cordova](https://linkedin.com/in/alexis-andres-cordova)

---
