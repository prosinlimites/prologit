# ProLogit — preparación para Vercel

Este paquete envuelve el archivo JSX que se recibió en una estructura básica de React + Vite para poder importarlo como proyecto.

## Publicar en GitHub y Vercel

1. Descomprime el ZIP en tu computador.
2. En GitHub crea un repositorio **Private** llamado `prologit`.
3. En el repositorio usa **Add file → Upload files** y arrastra el contenido de esta carpeta descomprimida (incluidas las carpetas `src` y sus archivos). No subas un ZIP dentro del repositorio.
4. En Vercel elige **Add New → Project**, importa el repositorio `prologit` y usa los valores predeterminados de Vite. Build command: `npm run build`; output directory: `dist`.
5. Pulsa Deploy.

## Importante antes de usarlo con clientes

Este paquete NO convierte el prototipo en un SaaS completo. El código recibido no contiene una conexión con Supabase ni un sistema real de autenticación o aislamiento de datos. Los botones de acceso/registro del prototipo cambian de pantalla dentro del navegador. Los envíos y otros datos parecen manejarse en estado de React y pueden perderse al recargar.

Por eso, úsalo solo como una publicación de prueba visual. No introduzcas información real de clientes ni pedidos hasta implementar autenticación, tablas, políticas RLS de Supabase y las funciones de backend necesarias.

## Desarrollo local (opcional)

Necesitas Node.js instalado. En esta carpeta ejecuta:
- `npm install`
- `npm run dev`
