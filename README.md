# 🦶 SEVITA ORTHESIS - Multi-Platform App

Sistema de Gestión e Inteligencia Clínica para laboratorios ortopédicos con soporte para **Web**, **Mobile** y **Desktop**.

## 📦 Estructura del Proyecto (Monorepo)

```
sevita-app/
├── packages/
│   ├── shared/          # Código compartido (tipos, utilidades, servicios IA)
│   ├── web/             # Web app + PWA (React + Vite)
│   ├── mobile/          # Mobile (React Native / Expo)
│   └── desktop/         # Desktop (Electron)
├── package.json         # Workspace root
└── pnpm-workspace.yaml  # Config de pnpm workspaces
```

## 🚀 Quick Start

### Requisitos previos
- Node.js 18+
- pnpm 8+

### Instalación

```bash
git clone https://github.com/ratsodexprg-crypto/sevita-app.git
cd sevita-app
pnpm install
```

### Desarrollo

```bash
# Ejecutar todas las plataformas en paralelo
pnpm dev

# O ejecutar una plataforma específica
pnpm dev:web      # http://localhost:5173
pnpm dev:mobile   # Expo dev server
pnpm dev:desktop  # Electron dev mode
```

### Build

```bash
pnpm build          # Compilar todas las plataformas
pnpm build:web      # Solo web
pnpm build:mobile   # Solo mobile
pnpm build:desktop  # Solo desktop
```

## 🔧 Configuración

Crea `.env.local` en cada paquete con tus credenciales:

```env
VITE_FIREBASE_API_KEY=xxx
VITE_FIREBASE_AUTH_DOMAIN=xxx
VITE_FIREBASE_PROJECT_ID=xxx
VITE_GEMINI_API_KEY=xxx
```

## 📱 Plataformas Soportadas

✅ **Web + PWA** (React + Vite + TailwindCSS)
✅ **Mobile** (React Native + Expo)
✅ **Desktop** (Electron)

## 🤖 Integración IA

- Google Gemini 3.5-Flash
- Vision API para análisis biomecánico
- Text-to-Speech
- Audio input por voz

---

Licencia: MIT | Autor: ratsodexprg-crypto
