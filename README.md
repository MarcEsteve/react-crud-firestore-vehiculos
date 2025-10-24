# 🚗💨 DGT Vehicles Manager — React + TypeScript + Firebase + Redux Toolkit

> 🧠 Proyecto final del curso **React Intermedio/Avanzado** (CoreNetworks)  
> Creado por **Marc Esteve Garcia**, formador oficial de React que disfruta explicando hooks mientras toma café ☕ y lucha contra los bucles infinitos.  

---

## 🧩 Descripción

Una **webapp moderna** que permite gestionar vehículos y usuarios al estilo DGT:  
- 🔐 Autenticación real con **Firebase Auth**  
- ☁️ Base de datos con **Cloud Firestore**  
- 🧠 Estado global con **Redux Toolkit**  
- 🧭 Navegación moderna con **React Router**  
- 🎨 Estilos rápidos con **TailwindCSS**  
- ⚙️ CRUD completo (Create, Read, Update, Delete)  
- 🧍‍♂️ Roles con rutas protegidas (solo **admin** puede tocar Ajustes)  
- 💥 Alertas visuales con **SweetAlert2**  
- 🌍 Desplegable en cualquier servicio (Firebase Hosting, Vercel, Netlify…)

---

## 🏗️ Arquitectura del proyecto
src/
├── app/
│ └── store.ts
│
├── features/
│ ├── auth/
│ │ ├── authSlice.ts
│ │ └── AuthContext.tsx
│ │
│ ├── vehiculos/
│ │ ├── vehiculosSlice.ts
│ │ └── VehiculoForm.tsx
│ │
│ └── ui/
│ └── uiSlice.ts
│
├── components/
│ ├── Header.tsx
│ ├── Layout.tsx
│ ├── ProtectedRoute.tsx
│ ├── RoleRoute.tsx
│ └── SweetAlert.tsx
│
├── pages/
│ ├── Home.tsx
│ ├── VehiculosPage.tsx
│ ├── UsuariosPage.tsx
│ ├── AjustesPage.tsx
│ ├── Login.tsx
│ ├── Register.tsx
│ ├── NoAcceso.tsx
│ └── NotFound.tsx
│
├── router/
│ └── router.tsx
│
├── styles/
│ ├── index.css
│ └── Header.css
│
├── firebaseConfig.ts
└── App.tsx



> 🪄 Inspirado en la estructura modular de aplicaciones empresariales modernas,  
> pero con el alma y el caos ordenado de un desarrollador React en viernes por la tarde. 😎

---

## ⚙️ Instalación

```bash
# 1️⃣ Clona el proyecto
git clone https://github.com/tuusuario/dgt-vehiculos-react.git
cd dgt-vehiculos-react

# 2️⃣ Instala dependencias
npm install

# 3️⃣ Configura Firebase 🔥
# Crea tu proyecto en https://console.firebase.google.com/
# Copia las claves en src/firebaseConfig.ts

# 4️⃣ Arranca el servidor
npm run dev

## 🧠 Tecnologías principales

| Categoría | Tecnología | Descripción |
|------------|-------------|--------------|
| 🖥️ Frontend | **React + TypeScript** | Framework de interfaz + tipado fuerte |
| 🧭 Rutas | **React Router (v7)** | Navegación SPA moderna con rutas protegidas |
| 🧠 Estado global | **Redux Toolkit** | Gestión global simple, clara y potente |
| 🔐 Autenticación | **Firebase Auth** | Registro, login y roles de usuario |
| ☁️ Base de datos | **Cloud Firestore** | Colecciones y documentos en la nube |
| 🎨 Estilos | **TailwindCSS** | Estilos rápidos y responsivos |
| 💥 Alertas | **SweetAlert2** | Popups elegantes y personalizables |

---

## 🧑‍💻 Scripts disponibles

| Comando | Acción |
|----------|--------|
| `npm run dev` | Inicia la app en modo desarrollo 🚀 |
| `npm run build` | Genera la versión optimizada 📦 |
| `npm run preview` | Previsualiza la build localmente 👀 |
| `npm run test` | Ejecuta pruebas con Vitest 🧪 |

---

## 🔐 Roles y permisos

| Rol | Permisos |
|------|-----------|
| 👤 Usuario | Puede iniciar sesión, ver y gestionar sus vehículos |
| 🛠️ Admin | Acceso total (puede entrar en `/ajustes`) |

Si un usuario intenta acceder a `/ajustes` sin permisos...  
> 😈 Recibirá un “🚫 No tienes acceso” más educado que el de cualquier API en producción.

---
