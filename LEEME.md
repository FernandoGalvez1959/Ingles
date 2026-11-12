# Sincronizar Inglés Básico A1 con Firebase (opcional, gratis)

La app funciona sin esto. Solo hace falta para guardar tu progreso en la nube
y verlo en otros móviles. Esta app tiene su propio proyecto de Firebase.
Plan gratuito **Spark**: no pide tarjeta.

## 1. Crear el proyecto
1. Entra en https://console.firebase.google.com con tu cuenta de Google.
2. Pulsa **Crear un proyecto**, ponle el nombre `ingles` (te añadirá unas letras) y sigue los pasos.
   Puedes desactivar Google Analytics.

## 2. Activar el acceso con correo
1. **Compilación > Authentication > Comenzar**.
2. Pestaña **Sign-in method** > **Correo electrónico/contraseña** > activa la primera opción > **Guardar**.

## 3. Crear la base de datos
1. **Compilación > Firestore Database > Crear base de datos**.
2. Ubicación en Europa (por ejemplo `eur3`) y modo **producción**.
3. Pestaña **Reglas**: borra lo que haya, pega el contenido de `firestore.rules` y pulsa **Publicar**.

## 4. Copiar los datos del proyecto
1. Engranaje > **Configuración del proyecto**.
2. En **Tus apps** pulsa el icono web `</>`, ponle un nombre y **Registrar app** (sin Hosting).
3. Copia el bloque `firebaseConfig` y pásaselo a Claude: él rellena `firebase-config.js`.
   (O pega tú los valores en ese archivo, sustituyendo cada `PEGA_AQUI`.)

## 5. Subir a GitHub y entrar
1. Sube los archivos al repositorio de la app desde la web de GitHub (Add file > Upload files).
2. En la app: pestaña **Datos** > **Sincronización** > **Crear cuenta nueva**.
   En otro móvil, pulsa **Entrar** con el mismo correo.

## Copia de seguridad
En la pestaña **Datos** puedes descargar tu progreso en un archivo («Inglés básico 1» y la fecha)
y cargarlo cuando quieras. Con la copia automática, al abrir la app se descarga una al día
si ya has avanzado.
