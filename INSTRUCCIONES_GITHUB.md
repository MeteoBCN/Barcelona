# 📚 Guía para Subir tu Proyecto a GitHub

## Opción 1: Desde la Terminal (Recomendado)

### 1. Crear repositorio en GitHub
1. Ve a [github.com](https://github.com) e inicia sesión
2. Haz clic en el botón **+** (arriba derecha) → **New repository**
3. Nombre: `el-tiempo-barcelona` (o el que prefieras)
4. Descripción: "Web meteorológica moderna para Barcelona con divulgación científica"
5. Marca como **Public** (o Private si lo prefieres)
6. **NO** marques "Initialize with README" (ya tenemos uno)
7. Haz clic en **Create repository**

### 2. Subir archivos desde tu computadora

Abre la terminal en la carpeta donde descargaste los archivos y ejecuta:

```bash
# Inicializar repositorio Git
git init

# Añadir todos los archivos
git add .

# Hacer el primer commit
git commit -m "Versión inicial: Web del tiempo Barcelona"

# Conectar con GitHub (reemplaza TU-USUARIO y el nombre del repo)
git remote add origin https://github.com/TU-USUARIO/el-tiempo-barcelona.git

# Subir archivos
git branch -M main
git push -u origin main
```

### 3. Activar GitHub Pages

1. En tu repositorio de GitHub, ve a **Settings** (Configuración)
2. En el menú lateral, haz clic en **Pages**
3. En **Source**, selecciona **main** branch
4. Haz clic en **Save**
5. ¡Tu web estará en línea en unos minutos! La URL será:
   `https://TU-USUARIO.github.io/el-tiempo-barcelona`

## Opción 2: Desde la Interfaz Web de GitHub (Más Fácil)

### 1. Crear repositorio
Igual que en la Opción 1, pasos 1-7

### 2. Subir archivos manualmente
1. En la página de tu repositorio nuevo, haz clic en **uploading an existing file**
2. Arrastra y suelta estos 5 archivos:
   - `index.html`
   - `divulgacion.html`
   - `README.md`
   - `LICENSE`
   - `.gitignore`
3. Escribe un mensaje de commit: "Versión inicial"
4. Haz clic en **Commit changes**

### 3. Activar GitHub Pages
Igual que en la Opción 1, paso 3

## 🔄 Actualizar tu Web en el Futuro

Cuando hagas cambios:

```bash
git add .
git commit -m "Descripción de los cambios"
git push
```

## ✅ Verificar que Funciona

1. Espera 2-3 minutos después de activar Pages
2. Visita: `https://TU-USUARIO.github.io/el-tiempo-barcelona`
3. ¡Deberías ver tu web funcionando!

## 🆘 Solución de Problemas

**Problema: No veo mi web en GitHub Pages**
- Verifica que el archivo se llame exactamente `index.html` (minúsculas)
- Espera unos minutos, GitHub Pages tarda en procesar
- Revisa en Settings → Pages que esté activado correctamente

**Problema: Errores al hacer push**
- Asegúrate de haber configurado Git con tu usuario:
  ```bash
  git config --global user.name "Tu Nombre"
  git config --global user.email "tu-email@ejemplo.com"
  ```

**Problema: Me pide contraseña constantemente**
- Usa un Personal Access Token en lugar de tu contraseña
- Ve a GitHub → Settings → Developer settings → Personal access tokens

## 📝 Comandos Git Útiles

```bash
# Ver estado de archivos
git status

# Ver historial de commits
git log

# Deshacer cambios no guardados
git checkout -- nombre-archivo.html

# Ver diferencias
git diff
```

¡Listo! Tu proyecto estará en línea y podrás compartirlo con quien quieras. 🚀
