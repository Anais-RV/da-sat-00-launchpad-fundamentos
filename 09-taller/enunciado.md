# 🔧 Taller Git & GitHub - Ejercicio Paso a Paso

## 📝 Contexto

Vas a crear tu primer repositorio en GitHub, añadir contenido y practicar los comandos básicos de Git que usarás en todos los proyectos satélites.

---

## ✅ Paso 1: Configurar Git (solo la primera vez)

Abre tu terminal y configura tu identidad:

```bash
git config --global user.name "Tu Nombre"
git config --global user.email "tu-email@ejemplo.com"
```

**Verifica la configuración:**
```bash
git config --list
```

---

## ✅ Paso 2: Crear un repositorio en GitHub

1. Ve a [GitHub.com](https://github.com) e inicia sesión
2. Haz clic en el botón **"+"** (arriba derecha) → **"New repository"**
3. Configura tu repositorio:
   - **Repository name:** `taller-git-github`
   - **Description:** "Mi primer taller de Git y GitHub"
   - **Public** ✅ (para que las formadoras puedan verlo)
   - ✅ Marca **"Add a README file"**
4. Haz clic en **"Create repository"**

¡Perfecto! Ya tienes tu primer repo en GitHub 🎉

---

## ✅ Paso 3: Clonar el repositorio a tu computadora

Copia la URL de tu repositorio (botón verde **"Code"** → HTTPS)

En tu terminal:

```bash
cd Desktop  # O la carpeta donde quieras trabajar
git clone https://github.com/TU-USUARIO/taller-git-github.git
cd taller-git-github
```

**Verifica que estás en el repositorio:**
```bash
git status
```

Deberías ver algo como: `On branch main` y `nothing to commit, working tree clean`

---

## ✅ Paso 4: Editar el README.md

Abre el archivo `README.md` en VS Code o tu editor favorito.

**Reemplaza** el contenido con algo como esto:

```markdown
# 🚀 Mi Primer Repositorio

**Nombre:** [Tu nombre]  
**Bootcamp:** Data Analyst  
**Fecha:** Enero 2026

## 📋 Sobre este proyecto

Este es mi primer repositorio en GitHub, creado como parte del **SAT-00 Launchpad**.

## 🎯 Objetivos del taller

- ✅ Configurar Git
- ✅ Crear un repositorio en GitHub
- ✅ Hacer commits
- ✅ Subir cambios al remoto

## 🔧 Comandos básicos que he aprendido

```bash
git clone    # Clonar un repositorio
git status   # Ver estado de cambios
git add      # Añadir archivos al stage
git commit   # Guardar cambios con mensaje
git push     # Subir cambios a GitHub
```

## 🎓 Lo que viene

Voy a usar Git en todos mis proyectos satélites del bootcamp.

---

**Última actualización:** [Fecha de hoy]
```

Guarda el archivo.

---

## ✅ Paso 5: Ver los cambios

En la terminal:

```bash
git status
```

Deberías ver `README.md` en rojo (modificado pero no staged)

---

## ✅ Paso 6: Hacer tu primer commit

**1. Añadir el archivo al staging area:**
```bash
git add README.md
```

**2. Verificar:**
```bash
git status
```

Ahora `README.md` debería estar en verde.

**3. Hacer el commit con un mensaje descriptivo:**
```bash
git commit -m "feat: actualizar README con información personal"
```

**💡 Tip:** Los mensajes de commit buenos empiezan con:
- `feat:` para nuevas funcionalidades
- `fix:` para correcciones
- `docs:` para documentación
- `style:` para formato/estilo

---

## ✅ Paso 7: Crear un segundo archivo

Vamos a practicar añadiendo un archivo nuevo.

**Crea un archivo `apuntes.md`:**

```bash
touch apuntes.md  # En Windows: echo. > apuntes.md
```

**Edítalo con este contenido:**

```markdown
# 📝 Apuntes de Git

## Comandos que más uso

### Ver estado
git status

### Añadir cambios
git add nombre-archivo
git add .  # Añade todos los archivos

### Hacer commit
git commit -m "mensaje descriptivo"

### Subir a GitHub
git push

### Ver historial
git log --oneline

## 🆘 Comandos de emergencia

### Deshacer cambios no guardados
git checkout -- nombre-archivo

### Ver diferencias
git diff
```

Guarda el archivo.

---

## ✅ Paso 8: Segundo commit

```bash
git add apuntes.md
git commit -m "docs: añadir archivo de apuntes con comandos útiles"
```

**Verifica tu historial:**
```bash
git log --oneline
```

Deberías ver tus 2 commits (más el commit inicial de GitHub).

---

## ✅ Paso 9: Subir todo a GitHub

```bash
git push
```

Si es la primera vez, puede pedirte autenticación. Sigue las instrucciones.

**Verifica en GitHub:**
1. Recarga la página de tu repositorio
2. Deberías ver los 2 archivos: `README.md` y `apuntes.md`
3. Haz clic en "commits" (arriba) para ver tu historial

---

## ✅ Paso 10: Entrega

**Copia la URL de tu repositorio** (algo como: `https://github.com/tu-usuario/taller-git-github`)

**Pégala en la tabla de evaluación de Google Sheets** en la columna correspondiente al Taller 00.

---

## 🎉 ¡Felicidades!

Has completado tu primer taller de Git & GitHub. Ahora sabes:

✅ Crear repos en GitHub  
✅ Clonar repos a tu computadora  
✅ Hacer commits con mensajes descriptivos  
✅ Subir cambios a GitHub  
✅ Ver el historial de cambios

**Estos comandos los usarás en TODOS los proyectos satélites** 🚀

---

## 🔄 Práctica adicional (opcional)

Si te ha sobrado tiempo, intenta:

1. **Crear un archivo `.gitignore`:**
   ```bash
   echo ".DS_Store" > .gitignore  # macOS
   echo "Thumbs.db" >> .gitignore  # Windows
   git add .gitignore
   git commit -m "chore: añadir gitignore"
   git push
   ```

2. **Ver diferencias antes de commit:**
   ```bash
   # Modifica README.md
   git diff
   git add README.md
   git commit -m "docs: actualizar README"
   git push
   ```

3. **Explora tu historial:**
   ```bash
   git log --oneline --graph --all
   ```

---

## 🆘 Problemas comunes

### "fatal: not a git repository"
→ No estás en la carpeta del repositorio. Haz `cd taller-git-github`

### "Your branch is ahead of 'origin/main' by 1 commit"
→ Has hecho commits locales pero no los has subido. Haz `git push`

### "Permission denied (publickey)"
→ Problema de autenticación. Usa HTTPS en lugar de SSH o configura una clave SSH.

### "nothing to commit, working tree clean"
→ No has hecho cambios. Modifica un archivo primero.

---

**⏱️ Tiempo invertido:** ~30 minutos  
**🎯 Siguiente paso:** Aplicar esto en SAT-01 Atlas
