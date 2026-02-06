# 🚀 Guía de Despliegue en GitHub

## Paso 1: Crear el repositorio en GitHub

1. Ve a [GitHub.com](https://github.com) e inicia sesión
2. Haz clic en el botón **"New"** (Nuevo) o el ícono **"+"** en la esquina superior derecha
3. Selecciona **"New repository"**
4. Configura el repositorio:
   - **Repository name:** `grupo2r` (o el nombre que prefieras)
   - **Description:** "Sitio web de Grupo 2R - Soluciones visuales y publicidad"
   - Marca como **Public** (Público)
   - NO marques "Add a README file" (ya tenemos uno)
5. Haz clic en **"Create repository"**

## Paso 2: Subir los archivos

### Opción A: Usar GitHub Desktop (Más fácil)

1. Descarga e instala [GitHub Desktop](https://desktop.github.com/)
2. Abre GitHub Desktop e inicia sesión
3. Ve a **File → Add Local Repository**
4. Selecciona la carpeta `grupo2r`
5. Haz clic en **"Publish repository"**
6. Confirma que sea público y publica

### Opción B: Usar línea de comandos (Git)

Abre la terminal en la carpeta del proyecto y ejecuta:

```bash
# Inicializar repositorio
git init

# Agregar todos los archivos
git add .

# Hacer el primer commit
git commit -m "Initial commit - Grupo 2R website"

# Conectar con GitHub (reemplaza TU_USUARIO con tu nombre de usuario)
git remote add origin https://github.com/TU_USUARIO/grupo2r.git

# Subir los archivos
git branch -M main
git push -u origin main
```

### Opción C: Subir archivos directamente en GitHub

1. En tu repositorio recién creado, haz clic en **"uploading an existing file"**
2. Arrastra todos los archivos y carpetas del proyecto
3. Escribe un mensaje de commit: "Initial commit"
4. Haz clic en **"Commit changes"**

## Paso 3: Activar GitHub Pages

1. En tu repositorio, ve a **Settings** (Configuración)
2. En el menú lateral, busca **"Pages"**
3. En la sección **"Source"**:
   - Selecciona **"Deploy from a branch"**
   - Branch: **main**
   - Folder: **/ (root)**
4. Haz clic en **"Save"**
5. ¡Espera 1-2 minutos!

## 🎉 ¡Listo!

Tu sitio estará disponible en:
```
https://TU_USUARIO.github.io/grupo2r/
```

(Reemplaza TU_USUARIO con tu nombre de usuario de GitHub)

---

## 🔄 Para actualizar el sitio en el futuro

Cada vez que hagas cambios:

```bash
git add .
git commit -m "Descripción de los cambios"
git push
```

Los cambios se verán reflejados en tu sitio en 1-2 minutos.

---

## 📝 Notas importantes

- El archivo `index.html` es la página principal
- La carpeta `assets/` contiene las imágenes
- `rubio.html` es la página de servicios
- GitHub Pages sirve archivos estáticos (HTML, CSS, JS)
- No necesitas servidor, GitHub lo hace por ti gratis

## 🆘 ¿Problemas?

- Verifica que el repositorio sea público
- Asegúrate de que GitHub Pages esté activado en Settings
- Espera unos minutos después de activar Pages
- La URL debe ser exactamente: `https://tu-usuario.github.io/nombre-repo/`
