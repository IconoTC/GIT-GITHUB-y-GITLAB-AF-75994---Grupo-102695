# Curso de Git, GitHub y GitLab

- GIT-GITHUB-Y-GITLAB-AF-75994-Grupo-102695
- Duración: 25 horas
- Modalidad: On-line
- Fechas: 19, 20, 21 , 22, y 23 de Octubre 2026
- Horario 9:00 – 14:00 hs

Formador: Alejandro Cerezo
<alce65@hotmail.es>

## Contenidos

- Introducción
  - Instalación y configuración de git
  - Gestión de un repositorio
    - Quick Start
    - Aprendiendo a referenciar revisiones y paths
    - Herramientas para preparar un buen commit en cualquier situación
  - GUI’s (Integración con otras herramientas y entornos)
    - Github
    - GitLab
  - Reescribiendo la historia
- Ramas (Trabajando en paralelo)
  - Ramificación
  - Fusión de Ramas
  - Resolviendo Problemas
  - Tipos de Ramas
  - Tags
- Buenas prácticas
  - Reorganización
  - Regla de Oro
  - Forzar subida
- Colaboración en Github
  - Ramas remotas
  - Publicando
  - Tags
  - Pull Request
  - Liberaciones (releases)
- GitFlow
  - Introducción
  - Features
  - Releases
  - Hotfix
- Git hooks
- Github Actions
  - Introducción
  - Workflow. Partes y sintaxis
  - Configuración y ejecución de un workflow
  - Construir la imagen con Docker
  - Secretos
- GitLab
  - Introducción
  - Versiones
  - Funcionalidades
  - Arquitectura
  - Usuarios
  - Repositorios
  - Ramas
  - Merge Request
  - Pipelines

Desarrollo del curso en la carpeta Oficial -> [repo](https://github.com/IconoTC/GIT-GITHUB-y-GITLAB-AF-75994---Grupo-102695)

## Desarrollo del curso

### Día 1 (Lunes 19 Octubre 2025)

- Presentación profesor / alumnos
- Introducción: Qué es un SCV y qué un SCV distribuido
- IDE / Editor de código: Visual Studio Code (VSC)
- Instalación de Git
- Terminales
  Configuración inicial
  - Nombre de usuario y correo electrónico

- [Descanso] 11:10 - 11:40

- Primeros pasos con Git

  - Primer repo (init), primer commit: .gitignore / readme.md
  - Anatomía de un repositorio git: working directory, staging area (index o cache) y repositorio (.git)
  - Estados de un archivo: untracked (U), tracked (modified (M), staged (A), committed)
  - add/commit/reset y status/log/show - GitGraph
  - Mensajes de commit

- Anatomía de comandos típicos, referencias VS paths

  - HEAD, main, HEAD~1 y otras referencias útiles
  - Referencias por mensaje de commit (:/cadena)

- Integración con otras herramientas y entornos
  - Clientes gráficos
  - Entornos de desarrollo
  - Repositorios remotos: GitHub, GitLab, Bitbucket
    - remotes -> push / pull
    - Clonar un repositorio: clone
- Comprobar el repositorio.
  - git log
  - git show
  - git diff
- Aliases
  - Qué son
  - Cómo crearlos desde el CLI: `git config --global alias.ch checkout`
  - Crearlos editando el fichero de configuración: `git config --global -e`
- Ficheros Markdown
  - Qué son
  - Sintaxis básica
  - Vista previa en VSC / GitHub / GitLab

### Día 2 (Martes 20 Octubre 2025)

- Git internals

  - Estructura de un repositorio git: .git
  - Objetos git: blobs, trees, commits (y tags)
    - Creación y lectura de objetos
    - Creación del árbol de objetos en un primer commit
    - Modificación del árbol de objetos en commits sucesivos
  - Referencias: heads, ramas (tags y remotes)
  - Taller: creación de un repositorio git "a mano"

- [Descanso] 11:00 - 11:30

- Herramientas para preparar un buen commit en cualquier situación

  - Operaciones en la Staging Area (Index)
    - Añadir ficheros
    - Eliminar de la Staging Area (Index)
    - git add -p
  - Eliminar ficheros: git rm
    - Problemas con .gitignore
  - Cambiar nombre de ficheros: git mv
  - git blame
  - git notes
  - Recapitulando: Git básico

  - Reescribiendo la historia
    - Advertencia
    - git commit --amend
      - Ref logs
    - git checkout
      - Evolución de git checkout: Nuevos comandos git switch y git restore
      - git checkout a nivel de archivo (restore)
    - git reset 
      - modificadores: --soft, --mixed, --hard
      - git reset a nivel de archivo
    - rebase interactivo
      - reword: cambiando el mensaje de un commit
      - edit: modificando un commit
      - drop: eliminando un commit

### Día 3 (Miércoles 21 Octubre 2025)

 - Reescribiendo la historia (2)
    - rebase interactivo
      - pick: reordenando commits
      - squash y fixup: fusionando commits
- Otros comandos
  - git clean
  - git revert
  - git bisect

- Trabajando en paralelo

  - Ramas
    - Crear y seleccionar
      - Crear desde referencia
    - Ver ramas
    - Borrar ramas
    - Mover y renombrar ramas

  - git stash

- [Descanso] 11:00 - 11:30


- Trabajando en paralelo (2)
  - Combinación de ramas: Merge y Rebase
    - git merge
      - fast-forward
      - three-way merge (ort)
    - git rebase
  - Resolución de conflictos

  - git cherry-pick
  - Patches
    - Creación
    - Aplicación

- Etiquetas (tags)

  - Tags anotadas y tags ligeros
  - Crear, listar, eliminar

- Worktrees

### Día 4 (Jueves 22 Octubre 2025)

- Integraciones

  - Integración con otras herramientas y entornos
    - Clientes gráficos
    - Entornos de desarrollo: VSC
      - Opciones nativas de VSC para Git
      - Extensiones de VSC para Git: Git Graph (GitLens, Git History...)

- Repositorios remotos

  - GitHub (repositorios) v. GitLab (grupos y proyectos) 

  - Repositorios "bare"
  - Clonar repositorios: git clone
  - git remote

  - Ramas remotas
    - Seguimiento de ramas remotas (tracking branches)
    - Crear ramas locales a partir de ramas remotas: fetch + checkout / switch -c
    - Subir ramas locales a ramas remotas: -u
    - Eliminar ramas remotas

  - git push
    - push tags
  - git pull
    - git fetch
    - git merge / git rebase

- [Descanso] 11:00 - 11:30

 - git pull (continuación)
    - Conflictos

  - Pull requests (GitHub) / Merge requests (GitLab)
    - Flujo de trabajo típico
    - Revisión de código
    - Resolución de conflictos en remoto
    - Buenas prácticas:
      - Actualizar la rama con la rama main antes de hacer el merge
      - Resolución de conflictos en local
      - Eliminar la rama una vez hecho el merge

- Flujos de trabajo (workflows)

  - Git Flow
  - GitLab Flow
  - GitHub Flow
    - Ship-Show-Ask

- Buenas prácticas

- GitHub
  - Hosting de Repositorios
    - repositorios públicos y privados; ramas y remotos: push y pull (v.s.)
    - forks
  - Colaboración
    - pull requests: revisión de código y comentarios (v.s.)
    - PR desde ramas y forks
 
### Día 5 (Viernes 23 Octubre 2025)

<!-- 
- GitHub (continuación)
   - Colaboración
    - Proyectos
      - Tableros (Boards)
      - issues y proyectos; milestones
    - Wikis
    - Gists
  - GitHub CLI
  - GitHub Pages
    - Configuración y uso
    - Práctica: publicar una web estática generada con Astro
  - Releases

- Integración continua / Entrega continua (CI/CD)

  - GitHub Actions
    - Introducción
    - Workflow. Partes y sintaxis
    - Configuración y ejecución de un workflow
    - Ejemplo de CI (build y test) de una aplicación JS -->

- [Descanso]

<!-- 

- Integración continua / Entrega continua (CI/CD)
  - GitHub Actions (continuación)
    - CD: despliegues
      - Secretos
      - Despliegue en GitHub Pages

  - GitLab
    - Similitudes y diferencias con GitHub. Merge Request
    - CI/CD en GitLab
      - Introducción a CI/CD
      - Configuración de un pipeline: stages y jobs
      - Artefactos
      - Variables
      - Despliegues: environments
  - GitHub Actions (continuación)
    - CD: despliegues de Astro en GitHub Pages 

-->
