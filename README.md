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
backend/
├─ src/
│ ├─ main/
│ │ ├─ java/
│ │ │ └─ com.keylab/
│ │ │ ├─ controllers/
│ │ │ ├─ services/
│ │ │ ├─ models/
│ │ │ ├─ repositories/
│ │ │ └─ config/
│ │ └─ resources/
│ │ └─ application.properties

### Frontend 


<img width="331" height="1000" alt="Captura de pantalla 2025-09-22 140040" src="https://github.com/user-attachments/assets/a268dd5c-ae82-4ab8-bc82-ed116c153fbb" />

---

### 4️⃣ **Flujo de la aplicación / Ejemplo de uso**
- Explica cómo se conectan frontend y backend, cómo se hace login, carrito, pago (sin mostrar código sensible).
```markdown
## Flujo general
1. El usuario ingresa a la app (React) y se conecta al backend (Spring Boot).
2. Puede navegar productos, agregarlos al carrito y realizar pagos mediante Mercado Pago.
3. Backend valida usuarios con JWT, maneja la persistencia en MySQL y conecta con servicios externos (Cloudinary para imágenes, Supabase para almacenamiento adicional).

## Por qué estas tecnologías
- **Spring Boot:** rápido desarrollo y robustez para APIs.
- **React + Vite:** SPA moderna y eficiente.
- **JWT:** seguridad en autenticación.
- **Docker:** despliegue reproducible.

- > ⚠️ El código completo se mantiene privado por motivos de seguridad. Este repositorio muestra la estructura y tecnologías utilizadas.
