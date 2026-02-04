# 🔧 Taller Git & GitHub - Práctica Autónoma

## 📝 Contexto

En este taller vas a:
1. **Clonar** un repositorio que ya existe (el Launchpad del bootcamp)
2. **Crear** tu propio repositorio de apuntes
3. **Investigar** comandos nuevos de Git

Estos comandos los usarás en TODOS los proyectos satélites. ¡Vamos allá!

---

## 🎯 EJERCICIO 1: Clonar el repositorio Launchpad (10 min)

### Paso 1: Clonar el repositorio

Abre tu terminal y navega a la carpeta donde guardes el bootcamp:

```bash
cd Desktop  # O donde tengas tu carpeta de proyectos
```

Ahora clona el repositorio Launchpad:

```bash
git clone [URL-DEL-REPO-LAUNCHPAD]
cd da-sat-00-launchpad-fundamentos
```

**Verifica que estás en el repositorio:**
```bash
git status
```

### Paso 2: Explora el contenido

```bash
ls
```

Deberías ver carpetas como: `00-orientacion-general/`, `01-que-es-programar/`, `09-taller/`, etc.

**¿Dónde estás ahora mismo?** En la carpeta `09-taller/` está este mismo enunciado 😊

---

## 🎯 EJERCICIO 2: Crear tu repositorio de apuntes (20 min)

Ahora vas a crear tu **propio repositorio** para ir guardando apuntes durante el bootcamp.

### Paso 1: Configurar Git (si no lo has hecho)

```bash
git config --global user.name "Tu Nombre"
git config --global user.email "tu-email@ejemplo.com"
```

**Verifica:**
```bash
git config --list
```

1. Ve a [GitHub.com](https://github.com) e inicia sesión
2. Haz clic en el botón **"+"** (arriba derecha) → **"New repository"**
3. Configura tu repositorio:
   - **Repository name:** `bootcamp-apuntes`
   - **Description:** "Apuntes del bootcamp Data Analyst"
   - **Public** ✅ (para que las formadoras puedan verlo)
   - ✅ Marca **"Add a README file"**
4. Haz clic en **"Create repository"**

¡Ya tienes tu repositorio de apuntes! 🎉

### Paso 3: Clonar tu repositorio

Copia la URL (botón verde **"Code"** → HTTPS) y clónalo:

```bash
cd Desktop  # Sal de la carpeta launchpad primero
git clone https://github.com/TU-USUARIO/bootcamp-apuntes.git
cd bootcamp-apuntes
```

### Paso 4: Crear estructura de carpetas

```bash
mkdir semana-01
cd semana-01
```

### Paso 5: Crear tu primer archivo de apuntes

Crea un archivo `dia-01.md` con este contenido:

```markdown
# 📅 Día 1 - [Fecha]

## 🎯 Lo que hemos visto hoy

### Mañana
- Dinámica: Gartic Phone (sobre distorsión de información)
- Conceptos: ¿Qué es análisis de datos?
- Ejercicio: Palabras en griego (buscar patrones sin contexto)

### Tarde
- Git y GitHub: instalación y configuración
- Primeros comandos: clone, status, add, commit, push

## 💡 Lo que he aprendido

[Escribe aquí lo más importante que te llevas del día]

## ❓ Dudas que tengo

[Anota aquí lo que necesitas repasar o preguntar]

## 🔗 Recursos útiles

- [Enlace a algún recurso que te haya gustado]

---

**Siguiente paso:** Empezar SAT-01 Atlas
```

Guarda el archivo.

### Paso 6: Tu primer commit

```bash
git add .
git status  # Verifica que dia-01.md está en verde
git commit -m "feat: añadir apuntes del día 1"
```

### Paso 7: Subir a GitHub

```bash
git push
```

**Verifica en GitHub:** Recarga la página de tu repo y deberías ver la carpeta `semana-01/` con `dia-01.md`

---

## 🎯 EJERCICIO 3: Investigación guiada (15 min)

Ahora que ya sabes clonar, crear repos y hacer commits, vamos a investigar algunos comandos nuevos.

### 🔍 Parte 1: Explora estos comandos

Ejecuta cada comando en tu repositorio `bootcamp-apuntes` y **anota qué hace** en tu archivo `dia-01.md`:

```bash
git log --oneline
```
**¿Qué muestra?** [Responde en tu archivo]

```bash
git remote -v
```
**¿Qué información da?** [Responde en tu archivo]

```bash
git branch
```
**¿En qué rama estás?** [Responde en tu archivo]

### 🔍 Parte 2: Preguntas de investigación

Busca en internet (o prueba en la terminal) para responder estas preguntas. **Añádelas a tu `dia-01.md`:**

1. **¿Qué hace el comando `git pull`?**  
   (Pista: es el opuesto de `git push`)

2. **¿Para qué sirve el archivo `.gitignore`?**  
   (Pista: ignorar archivos que no quieres subir)

3. **¿Qué diferencia hay entre `git add .` y `git add nombre-archivo`?**

### 🔍 Parte 3: Guarda tu investigación

Añade una sección nueva en tu `dia-01.md`:

```markdown
## 🔍 Comandos investigados

### git log --oneline
[Tu explicación]

### git remote -v
[Tu explicación]

### git branch
[Tu explicación]

### git pull
[Tu explicación]

### .gitignore
[Tu explicación]

### git add . vs git add archivo
[Tu explicación]
```

**Guarda y haz commit:**
```bash
git add semana-01/dia-01.md
git commit -m "docs: añadir investigación de comandos Git"
git push
```

---

## ✅ Paso 5: Ver los cambios

En la terminal:

```bash
git status
```

Deberías ver `README.md` en rojo (modificado pero no staged)

---

## 🆘 Si te quedas atascada/o

### "fatal: not a git repository"
→ No estás en la carpeta del repositorio. Haz `cd` a la carpeta correcta.

### "Your branch is ahead of 'origin/main' by X commits"
→ Has hecho commits locales pero no los has subido. Haz `git push`

### "Permission denied" o problemas de autenticación
→ Usa el Personal Access Token que configuramos en clase.

### "nothing to commit, working tree clean"
→ No has hecho cambios o ya los subiste. Modifica un archivo primero.

### ¿Dudas sobre un comando?
```bash
git help nombre-comando
# Ejemplo: git help status
```

---

## 📚 Recursos adicionales

- [Git Cheat Sheet](https://education.github.com/git-cheat-sheet-education.pdf)
- [Visualizing Git](https://git-school.github.io/visualizing-git/)
- [GitHub Guides](https://guides.github.com/)

---

**⏱️ Tiempo estimado:** ~45 minutos  
**🎯 Siguiente paso:** Aplicar esto en SAT-01 Atlas

---

## 📦 Entrega

**Comparte con tu formadora:**
1. URL de tu repositorio `bootcamp-apuntes`
2. Pégala en la tabla de evaluación de Google Sheets (columna Taller 00)

---

## 🎉 ¡Felicidades!

Has completado el taller. Ahora sabes:

✅ Clonar repositorios existentes (como Launchpad)  
✅ Crear tus propios repositorios  
✅ Hacer commits con mensajes descriptivos  
✅ Subir cambios a GitHub  
✅ Investigar comandos nuevos de forma autónoma

**Estos comandos los usarás en TODOS los proyectos satélites** 🚀

---

## 🚀 Bonus (si te sobra tiempo)

### 1. Crear un archivo `.gitignore`

En tu repositorio `bootcamp-apuntes`:

```bash
cd ..  # Sal de semana-01
echo ".DS_Store" > .gitignore  # macOS
echo "Thumbs.db" >> .gitignore  # Windows
echo "*.tmp" >> .gitignore  # Archivos temporales
git add .gitignore
git commit -m "chore: añadir gitignore"
git push
```

### 2. Personalizar tu perfil de GitHub

1. Ve a tu perfil en GitHub
2. Haz clic en "Edit profile"
3. Añade una bio, foto, y ubicación
4. ¡Personalízalo como quieras!

### 3. Explorar otros repositorios

Busca en GitHub: "data analysis projects" y explora repos de otras personas. ¿Cómo organizan sus archivos? ¿Cómo escriben sus README?
