# Curso de _Git_ & _GitHub_ - jonmircha

Este es el repositorio de práctica utilizado para aprender los fundamentos de Git (software de versionado) y GitHub (plataforma en la nube). Esta iniciativa gratuita pertenece a [Jonmircha](https://www.youtube.com/@jonmircha)

## 🚀 Primera Práctica: Flujo básico de git y github

En esta fase inicial del curso, configuramos el entorno y establecimos el flujo de trabajo básico de Github.

### Requisitos previos:

Tener instalado Git
Cuenta activa en GitHub
Editor de código (recomendado: Visual Studio Code)

### Comandos iniciales ejecutados:

1. Inicialización: `git init` (para empezar a trackear la carpeta)

2. Configuración:

- `git config --global user.name "Tu Nombre"`
- `git config --global user.email "tu@email.com"`

3. Flujo de trabajo:

- git `add .`: Para pasar los archivos al Staging Area
- git `commit -m "Primer commit"`: Para registrar los cambios en la cabeza (HEAD) del repositorio

## 🌿 Segunda Práctica: Cambiar rama Master a Main

En esta segunda práctica se realiza el traslado de la rama Master por Main, en un repositorio ya existente y en uno [nuevo](https://github.com/angeldavid04/curso-git-main). En dicho repositorio se encuentra la explicación para iniciar repositorios con la rama main.

### Reemplazando master por main en GitHub

```bash
# Crea la rama local main y pásale el historial de la rama master
git branch -m master main

# Haz un push de la nueva rama local main en el repositorio remoto de GitHub
git push -u origin main


# Cambia el HEAD actual a la rama main
git symbolic-ref refs/remotes/origin/HEAD refs/remotes/origin/main
```

Después de ejecutar estos comandos, necesitas cambiar la rama por defecto en tu repositorio de GitHub, para ello puedes guiarte con este [recurso](https://docs.github.com/en/repositories/configuring-branches-and-merges-in-your-repository/managing-branches-in-your-repository/changing-the-default-branch) de la documentación oficial de GitHub.
