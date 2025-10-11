# 🧩 PLSQL_Gestion_Ventas  

Repositorio con una aplicación simple pero con una **base de datos desarrollada de forma detallada**, incluyendo:  
- Creación de tablas  
- Consultas SQL  
- Funciones  
- Procedimientos almacenados  
- Triggers  
- Bitácora de errores y control de operaciones  

---

## 🗺️ Modelo ER  
Estructura general del modelo entidad-relación que define la base de datos.  

<p align="center">
  <img src="https://github.com/user-attachments/assets/cd09795d-b763-4b3f-9738-a6bc5448d615" width="600">
</p>

---

## ⚙️ Trigger de bitácora de vendedores  
Ejemplo de trigger aplicado tras una operación **UPDATE**, registrando automáticamente los cambios en la tabla de bitácora.  

<p align="center">
  <img src="https://github.com/user-attachments/assets/19972de1-18a5-4ca1-8787-c84c02f9f4f9" width="600">
</p>

---

## 📦 Ejecución de Package y Procedimiento  
Ejecución de un **package PL/SQL** y un procedimiento para el cálculo del **aporte en ventas por vendedor**.  

<p align="center">
  <img src="https://github.com/user-attachments/assets/a380ce76-a10d-4793-9c44-aba87b8bbfbe" width="600">
</p>

---

## 🧮 Conteo de errores  
Ejemplo de detección de errores: el programa se ejecuta dos veces en el mismo año, resultando en **12 errores** de vendedores repetidos por año.  

<p align="center">
  <img src="https://github.com/user-attachments/assets/17eb1640-6244-4742-96cb-f855ef8e80eb" width="600">
</p>

---

## 🧱 Registro de errores  
Todos los errores detectados, sin importar su tipo, se almacenan en la tabla de errores para auditoría y seguimiento.  

<p align="center">
  <img src="https://github.com/user-attachments/assets/b2b52e3f-88f9-4988-9acd-b0f2ab54dfa0" width="600">
</p>

---
