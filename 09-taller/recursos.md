# 🔗 Recursos Útiles - Git & GitHub

## 📚 Documentación Oficial

### Git
- [Git Book (español)](https://git-scm.com/book/es/v2) - Documentación completa de Git
- [Git Cheat Sheet](https://education.github.com/git-cheat-sheet-education.pdf) - Resumen de comandos
- [Git Reference](https://git-scm.com/docs) - Referencia rápida de todos los comandos

### GitHub
- [GitHub Docs (español)](https://docs.github.com/es) - Documentación oficial
- [GitHub Quickstart](https://docs.github.com/es/get-started/quickstart) - Guía de inicio rápido
- [GitHub Skills](https://skills.github.com/) - Tutoriales interactivos

---

## 🎓 Tutoriales Recomendados

### Básico (lo que necesitas ahora)
- [Learn Git Branching](https://learngitbranching.js.org/?locale=es_ES) - Visual e interactivo
- [Git & GitHub para principiantes](https://www.youtube.com/watch?v=RGOj5yH7evk) - Video tutorial
- [Atlassian Git Tutorial](https://www.atlassian.com/es/git/tutorials) - Explicaciones claras

### Intermedio (para más adelante)
- [Git Branching Strategy](https://www.atlassian.com/git/tutorials/comparing-workflows) - Workflows
- [Conventional Commits](https://www.conventionalcommits.org/es/) - Estándar de mensajes
- [GitHub Flow](https://guides.github.com/introduction/flow/) - Flujo colaborativo

---

## 🆘 Solución de Problemas

### Errores comunes y soluciones
- [Oh Shit, Git!?!](https://ohshitgit.com/es) - Soluciones rápidas a errores típicos
- [Git Flight Rules](https://github.com/k88hudson/git-flight-rules) - "Si pasa X, haz Y"
- [Dangit, Git!?!](https://dangitgit.com/) - Versión en inglés con más casos

### Stack Overflow
- [Git tag](https://stackoverflow.com/questions/tagged/git) - Preguntas frecuentes
- [GitHub tag](https://stackoverflow.com/questions/tagged/github) - Problemas específicos

---

## 🎨 Herramientas Visuales

### GUI Clients (si prefieres interfaz gráfica)
- [GitHub Desktop](https://desktop.github.com/) - Cliente oficial de GitHub
- [GitKraken](https://www.gitkraken.com/) - Muy visual (gratis para estudiantes)
- [Sourcetree](https://www.sourcetreeapp.com/) - Completo y gratis

### Extensiones VS Code
- [GitLens](https://marketplace.visualstudio.com/items?itemName=eamodio.gitlens) - Supercharged Git
- [Git Graph](https://marketplace.visualstudio.com/items?itemName=mhutchie.git-graph) - Visualizar historial
- [Git History](https://marketplace.visualstudio.com/items?itemName=donjayamanne.githistory) - Ver cambios

---

## 📝 Cheatsheets Visuales

- [Git Cheat Sheet by GitHub](https://training.github.com/downloads/es_ES/github-git-cheat-sheet.pdf) - PDF descargable
- [Git Command Explorer](https://gitexplorer.com/) - Busca el comando que necesitas
- [Visualizing Git](https://git-school.github.io/visualizing-git/) - Ver qué hace cada comando

---

## 🎯 Buenas Prácticas

### Mensajes de commit
```bash
# ✅ Buenos mensajes
git commit -m "feat: añadir función de login"
git commit -m "fix: corregir error en cálculo de promedio"
git commit -m "docs: actualizar README con instrucciones"

# ❌ Malos mensajes
git commit -m "cambios"
git commit -m "fix"
git commit -m "asdfasdf"
```

### Commits frecuentes
- Haz commits pequeños y frecuentes
- Cada commit debe representar un cambio lógico
- Commitea antes de hacer experimentos arriesgados

### .gitignore
```
# Python
__pycache__/
*.pyc
.venv/
.env

# Datos sensibles
*.csv
*.xlsx
credenciales.json

# Sistema
.DS_Store
Thumbs.db
```

---

## 🎓 Para Profundizar (opcional)

### Conceptos avanzados
- [Git Branching Model](https://nvie.com/posts/a-successful-git-branching-model/) - Git Flow
- [Git Rebase vs Merge](https://www.atlassian.com/git/tutorials/merging-vs-rebasing)
- [Git Hooks](https://git-scm.com/book/es/v2/Personalizando-Git-Git-Hooks) - Automatización

### Colaboración en equipo
- [Pull Requests](https://docs.github.com/es/pull-requests) - Cómo contribuir a proyectos
- [Code Review](https://github.com/features/code-review) - Revisión de código
- [GitHub Actions](https://github.com/features/actions) - CI/CD básico

---

## 💡 Tips Rápidos

```bash
# Ver cambios antes de commit
git diff

# Deshacer último commit (mantiene cambios)
git reset --soft HEAD~1

# Ver historial bonito
git log --oneline --graph --all --decorate

# Crear alias útiles
git config --global alias.st status
git config --global alias.co checkout
git config --global alias.br branch
git config --global alias.cm commit

# Ahora puedes usar: git st, git co, etc.
```

---

## 🔐 Autenticación (si tienes problemas)

### HTTPS (recomendado para principiantes)
- [Personal Access Token](https://docs.github.com/es/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token)
- [Credential Helper](https://docs.github.com/es/get-started/getting-started-with-git/caching-your-github-credentials-in-git)

### SSH (más avanzado)
- [Generating SSH Keys](https://docs.github.com/es/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)
- [Adding SSH Key to GitHub](https://docs.github.com/es/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account)

---

## 📖 Lecturas Complementarias

- [Pro Git Book](https://git-scm.com/book/es/v2) - Libro completo gratuito
- [GitHub Learning Lab](https://lab.github.com/) - Cursos interactivos
- [First Contributions](https://github.com/firstcontributions/first-contributions/blob/master/translations/README.es.md) - Tu primera contribución open source

---

**💡 Recuerda:** No necesitas memorizar todo. Estos recursos están aquí para consultar cuando los necesites. Lo importante es practicar los comandos básicos que usarás a diario: `clone`, `add`, `commit`, `push`.
