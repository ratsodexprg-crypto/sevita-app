# SEVITA ORTHESIS - GUÍA DE INICIO RÁPIDO

¡Bienvenido! Tu app multi-plataforma está lista. Aquí está cómo empezar:

## 📦 Requisitos

- **Node.js 18+**
- **pnpm 8+**

```bash
npm install -g pnpm
```

## 🚀 Instalación

```bash
# Clonar y entrar al proyecto
git clone https://github.com/ratsodexprg-crypto/sevita-app.git
cd sevita-app

# Instalar dependencias
pnpm install
```

## 🔧 Configuración de Credenciales

### 1. Firebase Setup

Crea un archivo `.env.local` en la raíz del proyecto:

```env
VITE_FIREBASE_API_KEY=your_key_here
VITE_FIREBASE_AUTH_DOMAIN=your_project.firebaseapp.com
VITE_FIREBASE_PROJECT_ID=your_project_id
VITE_FIREBASE_STORAGE_BUCKET=your_bucket.appspot.com
VITE_FIREBASE_MESSAGING_SENDER_ID=your_sender_id
VITE_FIREBASE_APP_ID=your_app_id
```

### 2. Google Gemini API

Agregaala misma variable a `.env.local`:

```env
VITE_GEMINI_API_KEY=your_gemini_api_key
```

## 💻 Desarrollo

### Web + PWA (Recomendado para empezar)

```bash
pnpm dev:web
# Se abrirá en http://localhost:5173
```

### Desktop (Electron)

```bash
pnpm dev:desktop
```

### Mobile (React Native)

```bash
pnpm dev:mobile
```

## 🏗️ Build para Producción

```bash
# Compilar todas las plataformas
pnpm build

# O compilar específicamente
pnpm build:web
pnpm build:desktop
pnpm build:mobile
```

## 📱 Estructura del Proyecto

```
sevita-app/
├── packages/
│   ├── shared/          ← Código compartido (servicios, tipos)
│   ├── web/             ← Web + PWA (React + Vite)
│   ├── mobile/          ← Móvil (React Native + Expo)
│   └── desktop/         ← Desktop (Electron)
├── package.json         ← Root workspace
└── pnpm-workspace.yaml  ← Configuración pnpm
```

## 🤖 Servicios Integrados

✅ **Firebase** - Sincronización en tiempo real de órdenes
✅ **Google Gemini** - IA para procesamiento de voz, imágenes y análisis biomecánico
✅ **Storage Local** - Respaldo en navegador
✅ **Audio** - Grabación y reproducción

## 🔗 Próximos Pasos

1. **Configura Firebase** en la consola de Google Cloud
2. **Obtén una API Key de Gemini** desde Google AI Studio
3. **Agrega las credenciales** a `.env.local`
4. **Inicia el desarrollo** con `pnpm dev:web`

## 📚 Documentación Oficial

- [Firebase](https://firebase.google.com/docs)
- [Google Gemini](https://ai.google.dev)
- [React](https://react.dev)
- [Vite](https://vitejs.dev)
- [Electron](https://www.electronjs.org/docs)
- [React Native](https://reactnative.dev)

## 🆘 Soporte

Si encuentras problemas:

1. Verifica que tengas Node.js 18+ (`node --version`)
2. Verifica que tengas pnpm 8+ (`pnpm --version`)
3. Elimina `node_modules` y `pnpm-lock.yaml`, luego ejecuta `pnpm install` nuevamente
4. Revisa que las credenciales en `.env.local` sean correctas

---

**¡Listo para construir la app del futuro!** 🚀
