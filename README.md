# FisioAngulo IA · El Cazador de Estrellas

Juego interactivo de fisioterapia con detección de pose en tiempo real (MoveNet + TensorFlow.js) pensado para niños con hipotonía muscular.

## Estructura del proyecto

- `cazador_estrellas_final.html` — Aplicación principal (calibración, juego espacial, guía por voz, panel ML y vista terapeuta integrada).
- `camara_fisio.html` — Ventana de cámara independiente para el modo **Separado**.
- `terapeuta.html` — Panel de seguimiento para el fisioterapeuta (sincronizado vía `BroadcastChannel` y `localStorage`).
- `vercel.json` — Redirige `/` hacia `/cazador_estrellas_final.html` al desplegar en Vercel.
- `COMO_USAR.txt` — Guía rápida original de uso local y DroidCam.

## Despliegue en Vercel

1. Sube esta carpeta (`proyecto/`) a GitHub o despliégala directamente con `vercel`.
2. No requiere paso de build ni backend (100% estático).
3. Al abrir la URL raíz (`/`), `vercel.json` cargará `cazador_estrellas_final.html` bajo HTTPS (necesario para la cámara web).

## Uso local

```bash
python3 -m http.server 8765
# Abrir http://localhost:8765/cazador_estrellas_final.html
```
