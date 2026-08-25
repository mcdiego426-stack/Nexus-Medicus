# 📦 Guía de Despliegue en Vercel

## Requisitos Previos

✅ Cuenta de GitHub (crea una gratis en https://github.com)
✅ Cuenta de Vercel (crea una gratis en https://vercel.com - puedes usar tu GitHub)
✅ Git instalado en tu computadora (descarga de https://git-scm.com)

---

## PASO 1: Inicializar Git Localmente (Windows)

1. **Abre PowerShell** (Windows + X → PowerShell)

2. **Navega a la carpeta del proyecto:**
```powershell
cd "C:\temp-nexus-deploy"
```

3. **Inicializa Git:**
```powershell
git init
```

4. **Configura Git (primera vez):**
```powershell
git config --global user.name "Tu Nombre Completo"
git config --global user.email "tu@email.com"
```
*(Reemplaza con tu nombre y email real)*

5. **Agrega todos los archivos:**
```powershell
git add .
```

6. **Crea el primer commit:**
```powershell
git commit -m "Initial commit: Nexus Medicus Platform"
```

---

## PASO 2: Crear Repositorio en GitHub

1. **Ve a https://github.com** y inicia sesión

2. **Haz clic en el icono (+) arriba a la derecha → "New repository"**

3. **Completa el formulario:**
   - **Repository name:** `nexus-medicus` (o el nombre que prefieras)
   - **Description:** "Plataforma inmobiliaria de consultorios médicos premium"
   - **Visibility:** Público (Public)
   - **NO inicialices** con README, .gitignore o license (ya los tenemos)

4. **Haz clic en "Create repository"**

5. **Te aparecerá una pantalla con comandos. Copia el siguiente bloque:**

```powershell
git remote add origin https://github.com/TU_USUARIO/nexus-medicus.git
git branch -M main
git push -u origin main
```

*(Reemplaza TU_USUARIO con tu nombre de usuario de GitHub)*

---

## PASO 3: Subir código a GitHub

1. **En PowerShell, desde la carpeta del proyecto**, pega los comandos que copiaste:

```powershell
git remote add origin https://github.com/TU_USUARIO/nexus-medicus.git
git branch -M main
git push -u origin main
```

2. **Cuando pida login de GitHub:**
   - Click en "Authorize GitCredentialManager"
   - O ingresa tu token (mejor opción)

3. **Espera a que termine. Verás:**
```
branch 'main' set up to track 'origin/main'.
```

✅ **Tu código está en GitHub!**

---

## PASO 4: Desplegar en Vercel

### Opción A: Despliegue Automático (Recomendado)

1. **Ve a https://vercel.com** y haz login con GitHub

2. **Haz clic en "New Project"**

3. **Selecciona tu repositorio `nexus-medicus`**

4. **En configuración:**
   - **Framework Preset:** Other (es HTML puro)
   - **Root Directory:** ./
   - **Build Command:** (déjalo vacío)
   - **Output Directory:** ./
   - **Install Command:** (déjalo vacío)

5. **Haz clic en "Deploy"**

6. **Espera 2-3 minutos. Verás:**
   ```
   ✓ Deployment completed successfully!
   ```

7. **¡Listo! Tu URL será algo como:**
   ```
   https://nexus-medicus.vercel.app
   ```

---

### Opción B: Despliegue Manual via CLI

Si prefieres usar línea de comandos:

1. **Instala Vercel CLI:**
```powershell
npm install -g vercel
```

2. **Desde la carpeta del proyecto:**
```powershell
vercel
```

3. **Sigue las preguntas:**
   - "Set up and deploy?" → `y`
   - "Which scope?" → Selecciona tu usuario
   - "Link to existing project?" → `n`
   - "What's your project's name?" → `nexus-medicus`
   - "In which directory is your code?" → `./`
   - "Want to override the settings?" → `n`

4. **¡Listo! Te dará la URL pública**

---

## PASO 5: Verificar Despliegue

1. **Abre tu navegador en la URL que Vercel te dio:**
   ```
   https://nexus-medicus.vercel.app
   ```

2. **Prueba todas las funciones:**
   - ✅ Navega los modelos
   - ✅ Abre los modales
   - ✅ Llena un formulario
   - ✅ Haz clic en "Agendar Cita", "Descargar Documentos", etc.

3. **Verifica los enlaces:**
   - ✅ Botón "Agendar Cita" en navbar
   - ✅ Links a Fase 2, 3, 4 (si están disponibles)

---

## PASO 6: Actualizar tu Código (Después de cambios)

Cada vez que hagas cambios en los archivos:

1. **En PowerShell:**
```powershell
git add .
git commit -m "Describe tus cambios aquí"
git push
```

2. **Vercel desplegará automáticamente en 1-2 minutos**

3. **Tu sitio se actualizará automáticamente**

---

## 🔗 Enlaces Importantes

- **Tu sitio:** https://nexus-medicus.vercel.app
- **Dashboard Vercel:** https://vercel.com/dashboard
- **Repositorio GitHub:** https://github.com/TU_USUARIO/nexus-medicus
- **Documentación Vercel:** https://vercel.com/docs

---

## 🆘 Solución de Problemas

### Error: "Permission denied"
→ Verifica que Git esté instalado: `git --version`

### Error: "fatal: Not a git repository"
→ Asegúrate de estar en la carpeta correcta y ejecutar `git init`

### Error: "The specified directory does not exist"
→ Verifica la ruta: `cd "C:\temp-nexus-deploy"`

### El sitio se ve diferente
→ Limpia cache: Ctrl+Shift+Delete y recarga la página

### Los links internos no funcionan
→ Los links HTML en Vercel funcionan si son relativos (ya están configurados)

---

## ✅ Checklist Final

- [ ] Cuenta GitHub creada
- [ ] Cuenta Vercel creada
- [ ] Git instalado en Windows
- [ ] Repositorio creado en GitHub
- [ ] Código subido (git push)
- [ ] Proyecto importado en Vercel
- [ ] Despliegue completado
- [ ] Sitio accesible en vercel.app
- [ ] Todas las funciones funcionan

---

## 💡 Tips

1. **Compartir tu sitio:** La URL pública es: `https://nexus-medicus.vercel.app`
2. **Dominio personalizado:** En Vercel dashboard → Project → Settings → Domains
3. **Versiones anteriores:** Vercel mantiene histórico de deployments
4. **Analytics:** Vercel te muestra visitas y rendimiento

---

**¡Listo! Tu plataforma Nexus Medicus está en vivo en Internet! 🎉**
