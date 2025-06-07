
# CoinForge AI Meme Generator

## Instrucciones para desplegar en Render

1. **Sube este proyecto a un repositorio de GitHub**.
2. En Render, crea un nuevo servicio web.
3. Selecciona el repositorio desde GitHub.
4. En "Root Directory", escribe: `backend`
5. En "Build Command":  
   ```
   npm install
   ```
6. En "Start Command":  
   ```
   npm start
   ```
7. En "Environment Variables", añade:
   - Key: `REPLICATE_API_TOKEN`
   - Value: tu clave privada de Replicate (por ejemplo: `r8_06VyUzeAmIuuzTKmuHZFiYoR5cZWOl33xSRSN`)

8. Una vez desplegado el backend, crea otro servicio web en Render para el frontend (opcional) o súbelo como estático en otra parte.

## Estructura del proyecto

- `/backend`: Node.js + Express para generar memes vía IA.
- `/frontend`: HTML simple para conectarse con el backend.
