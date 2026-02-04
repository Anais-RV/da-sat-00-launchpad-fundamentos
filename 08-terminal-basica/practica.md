# 💻 Práctica: Comandos Básicos de Terminal

**Duración:** 30-45 min  
**Objetivo:** Ganar confianza con la terminal antes de usar Git  
**Nivel:** Principiante absoluto

---

## 🎯 ¿Qué vamos a hacer?

Vamos a practicar los comandos más básicos de la terminal:
- Saber dónde estás
- Moverte entre carpetas
- Crear carpetas y archivos
- Abrir VS Code desde la terminal

**No te preocupes:** Si te equivocas, no rompes nada 😊

---

## 📋 EJERCICIO 1: ¿Dónde estoy? (5 min)

### Paso 1: Abre la terminal

- **Windows:** PowerShell (busca "PowerShell" en el menú inicio)
- **Mac:** Terminal (busca "Terminal" en Spotlight)
- **Linux:** Terminal (Ctrl+Alt+T)

---

### Paso 2: Averigua dónde estás

**Windows:**
```bash
pwd
```

**Mac/Linux:**
```bash
pwd
```

Verás algo como:
- Windows: `C:\Users\TuNombre`
- Mac: `/Users/TuNombre`
- Linux: `/home/TuNombre`

**Esto es tu "carpeta de usuario"**, tu punto de partida.

---

### Paso 3: Mira qué hay en esa carpeta

**Windows:**
```bash
ls
```

**Mac/Linux:**
```bash
ls
```

Verás una lista de carpetas como: Desktop, Documents, Downloads, etc.

---

## 📋 EJERCICIO 2: Crear carpetas (10 min)

### Paso 1: Ve a tu escritorio (Desktop)

```bash
cd Desktop
```

**¿Qué significa `cd`?** Change Directory = Cambiar de carpeta

---

### Paso 2: Verifica que estás en Desktop

```bash
pwd
```

Debería decir algo como: `C:\Users\TuNombre\Desktop` (Windows) o `/Users/TuNombre/Desktop` (Mac)

---

### Paso 3: Crea una carpeta para el bootcamp

```bash
mkdir bootcamp-prueba
```

**¿Qué significa `mkdir`?** Make Directory = Crear carpeta

---

### Paso 4: Verifica que se creó

```bash
ls
```

Deberías ver `bootcamp-prueba` en la lista.

**También puedes mirar tu escritorio con los ojos** 👀 ¡Debería estar ahí!

---

### Paso 5: Entra en esa carpeta

```bash
cd bootcamp-prueba
```

---

### Paso 6: Verifica que estás dentro

```bash
pwd
```

Debería decir: `.../Desktop/bootcamp-prueba`

---

## 📋 EJERCICIO 3: Crear archivos (10 min)

### Paso 1: Crea un archivo de texto

**Windows:**
```bash
echo "Hola desde la terminal" > prueba.txt
```

**Mac/Linux:**
```bash
echo "Hola desde la terminal" > prueba.txt
```

---

### Paso 2: Verifica que se creó

```bash
ls
```

Deberías ver `prueba.txt`

---

### Paso 3: Lee el contenido del archivo

**Windows:**
```bash
type prueba.txt
```

**Mac/Linux:**
```bash
cat prueba.txt
```

Debería mostrarte: `Hola desde la terminal`

---

### Paso 4: Crea varias carpetas de una vez

```bash
mkdir semana-01 semana-02 semana-03
```

---

### Paso 5: Verifica

```bash
ls
```

Deberías ver las 3 carpetas + el archivo prueba.txt

---

## 📋 EJERCICIO 4: Abrir VS Code (10 min)

### Paso 1: Abre la carpeta actual en VS Code

```bash
code .
```

**¿Qué significa el punto `.`?** La carpeta actual

---

### Paso 2: Verifica en VS Code

En VS Code deberías ver:
- La carpeta `bootcamp-prueba` abierta
- Las carpetas: semana-01, semana-02, semana-03
- El archivo: prueba.txt

---

### Paso 3: Crea un archivo nuevo desde VS Code

En VS Code:
1. Haz clic derecho en la barra lateral → New File
2. Llámalo `apuntes.txt`
3. Escribe: "Esto lo creé desde VS Code"
4. Guarda (Ctrl+S / Cmd+S)

---

### Paso 4: Vuelve a la terminal

En la terminal, lista los archivos:

```bash
ls
```

**¡Deberías ver `apuntes.txt`!**

---

## 📋 EJERCICIO 5: Navegar entre carpetas (10 min)

### Paso 1: Entra en semana-01

```bash
cd semana-01
```

---

### Paso 2: Verifica dónde estás

```bash
pwd
```

Deberías estar en: `.../bootcamp-prueba/semana-01`

---

### Paso 3: Crea un archivo aquí

**Windows:**
```bash
echo "Apuntes semana 1" > notas.txt
```

**Mac/Linux:**
```bash
echo "Apuntes semana 1" > notas.txt
```

---

### Paso 4: Verifica

```bash
ls
```

Deberías ver: `notas.txt`

---

### Paso 5: Sube un nivel (vuelve a bootcamp-prueba)

```bash
cd ..
```

**¿Qué significa `..`?** La carpeta padre (un nivel arriba)

---

### Paso 6: Verifica dónde estás

```bash
pwd
```

Deberías estar de vuelta en: `.../bootcamp-prueba`

---

### Paso 7: Lista todo

```bash
ls
```

Deberías ver:
- Las carpetas: semana-01, semana-02, semana-03
- Los archivos: prueba.txt, apuntes.txt

---

## 🎓 EJERCICIO 6: Atajos útiles (5 min)

### 1. Volver al inicio (tu carpeta de usuario)

```bash
cd ~
```

**Verifica:**
```bash
pwd
```

Deberías estar en: `C:\Users\TuNombre` (Windows) o `/Users/TuNombre` (Mac)

---

### 2. Volver al escritorio rápido

```bash
cd ~/Desktop
```

---

### 3. Ver el historial de comandos

**Windows/Mac/Linux:**
```bash
history
```

Verás todos los comandos que has ejecutado.

---

### 4. Repetir el último comando

Pulsa **flecha arriba ↑** en el teclado.

---

### 5. Limpiar la pantalla

```bash
clear
```

(En Windows también funciona: `cls`)

---

## ✅ Resumen de comandos

| Comando | Qué hace | Ejemplo |
|---------|----------|---------|
| `pwd` | Muestra dónde estás | `pwd` |
| `ls` | Lista archivos y carpetas | `ls` |
| `cd nombre` | Entra en una carpeta | `cd Desktop` |
| `cd ..` | Sube un nivel | `cd ..` |
| `cd ~` | Va a tu carpeta de usuario | `cd ~` |
| `mkdir nombre` | Crea una carpeta | `mkdir proyecto` |
| `echo "texto" > archivo` | Crea archivo con texto | `echo "Hola" > test.txt` |
| `type archivo` (Win) | Lee el contenido | `type test.txt` |
| `cat archivo` (Mac/Linux) | Lee el contenido | `cat test.txt` |
| `code .` | Abre VS Code aquí | `code .` |
| `clear` | Limpia la pantalla | `clear` |

---

## 🎯 Comprueba que lo has conseguido

Si puedes hacer esto sin mirar las instrucciones, **¡LO HAS CONSEGUIDO!** 🎉

1. Abre la terminal
2. Ve a tu escritorio: `cd ~/Desktop`
3. Crea una carpeta: `mkdir test-final`
4. Entra en ella: `cd test-final`
5. Crea un archivo: `echo "Éxito" > conseguido.txt`
6. Lee el archivo: `type conseguido.txt` (Windows) o `cat conseguido.txt` (Mac)
7. Abre VS Code: `code .`

**Si ves el archivo en VS Code: ¡PERFECTO!** Ya controlas la terminal básica 💪

---

## 🗑️ Limpieza (opcional)

Si quieres borrar las carpetas de prueba:

### Desde VS Code:
1. Cierra VS Code
2. Ve a tu escritorio con el explorador de archivos
3. Borra las carpetas `bootcamp-prueba` y `test-final`

### Desde la terminal (más avanzado):
```bash
cd ~/Desktop
rm -r bootcamp-prueba
rm -r test-final
```

**⚠️ Cuidado:** El comando `rm -r` borra carpetas y archivos sin papelera de reciclaje.

---

## 🆘 Si algo sale mal

**"No me funciona `code .`"**
→ VS Code no está en el PATH. Ábrelo manualmente: VS Code → File → Open Folder

**"Me perdí y no sé dónde estoy"**
→ `pwd` para ver dónde estás  
→ `cd ~` para volver al inicio  
→ `cd ~/Desktop` para ir al escritorio

**"Borré algo por error"**
→ Si fue con el explorador de archivos, revisa la papelera de reciclaje  
→ Si fue con `rm`, no se puede recuperar (¡por eso hay que tener cuidado!)

**"La terminal no responde"**
→ Ciérrala y abre una nueva  
→ Reinicia el ordenador si es necesario

---

## 📌 Siguiente paso

Cuando te sientas cómoda con estos comandos básicos:
→ **Estarás lista para aprender Git** 🚀

Git usa la terminal, pero ahora ya sabes:
- Moverte entre carpetas
- Crear cosas
- Abrir VS Code

¡El resto es cuestión de práctica!

---

**Fin de la práctica**
