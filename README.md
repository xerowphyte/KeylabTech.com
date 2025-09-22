# KeylabTech.com.ar
Repositorio de demostración que muestra la arquitectura y estructura del backend y frontend del e-commerce KeyLab, incluyendo tecnologías utilizadas y flujo general de la aplicación.
Es un proyecto de e-commerce fullstack que demuestra buenas prácticas de arquitectura y estructura de código profesional, mostrando cómo se organiza un backend con Spring Boot y un frontend moderno en React.

## Tecnologías
- **Backend:** Java, Spring Boot, Spring Security, JPA Hibernate, MySQL
- **Frontend:** React, Tailwind, Vite
- **Otros:** JWT, Docker, Render, Supabase, Cloudinary, Mercado Pago.

## Arquitectura del proyecto

             ┌─────────────┐
             │ Frontend    │
             │ React / Vite│
             └─────┬───────┘
                   │
                   ▼
             ┌─────────────┐
             │ Backend     │
             │ Spring Boot │
             └─────┬───────┘
                   │
          ┌────────┴────────┐
          │                 │
          ▼                 ▼
    ┌─────────────┐   ┌─────────────┐
    │ MySQL DB    │   │ Servicios   │
    │             │   │ Externos    │
    │             │   │ -Cloudinary │
    │             │   │ -MercadoPago│
    │             │   │ -Supabase   │
    └─────────────┘   └─────────────┘
                         
## Estructura del proyecto

### Backend

<img width="342" height="1022" alt="Captura de pantalla 2025-09-22 141258" src="https://github.com/user-attachments/assets/150d38e6-c7f4-41e8-940d-d3a21c58facb" />


### Frontend 

<img width="331" height="1000" alt="Captura de pantalla 2025-09-22 140040" src="https://github.com/user-attachments/assets/a268dd5c-ae82-4ab8-bc82-ed116c153fbb" />

---
  
### **Flujo de la aplicación / Ejemplo de uso**
- Explica cómo se conectan frontend y backend, cómo se hace login, carrito, pago (sin mostrar código sensible).
  
## Flujo general
1. El usuario ingresa a la app (React) y se conecta al backend (Spring Boot).
2. Puede navegar productos, agregarlos al carrito y realizar pagos mediante Mercado Pago.
3. Backend valida usuarios con JWT, maneja la persistencia en MySQL y conecta con servicios externos (Cloudinary para imágenes, Supabase para almacenamiento adicional).

## Por qué estas tecnologías
- **Spring Boot:** rápido desarrollo y robustez para APIs.
- **React + Vite:** SPA moderna y eficiente.
- **JWT:** seguridad en autenticación.
- **Docker:** despliegue reproducible.

- El código completo se mantiene privado por motivos de seguridad. Este repositorio muestra la estructura y tecnologías utilizadas.

- ## Capturas de la app en funcionamiento

### Home

<img width="1917" height="934" alt="Captura de pantalla 2025-09-22 142223" src="https://github.com/user-attachments/assets/29c4bc5e-fa82-4932-ad14-3e350650f40d" />

### Carrito

<img width="1912" height="931" alt="Captura de pantalla 2025-09-22 142313" src="https://github.com/user-attachments/assets/78d93bfd-f19a-4fc7-a409-2764509175bc" />

### Panel Admin

<img width="1916" height="935" alt="Captura de pantalla 2025-09-22 142405" src="https://github.com/user-attachments/assets/70df1e0c-4597-40cc-89b0-e40f19693dcb" />

> Las capturas muestran la interfaz de KeyLab con datos ficticios para proteger información sensible.

## Licencia y variables de entorno

- ⚠️ El código completo se mantiene privado por motivos de seguridad.
- Se incluye `.env.example` para mostrar qué variables de entorno se necesitan.
- Este proyecto está protegido y no se permite uso comercial sin autorización.
